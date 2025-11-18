---
name: backend-fundamentals
description: Master backend development with databases, APIs, authentication, and server-side programming. Build scalable systems that power applications.
---

# Backend Development Fundamentals

## Quick Start with Node.js/Express

```javascript
// server.js - Basic Express API
const express = require('express');
const app = express();

app.use(express.json());

// Middleware
app.use((req, res, next) => {
  console.log(`${req.method} ${req.path}`);
  next();
});

// Routes
app.get('/api/users', (req, res) => {
  const users = [
    { id: 1, name: 'Alice' },
    { id: 2, name: 'Bob' }
  ];
  res.json(users);
});

app.post('/api/users', (req, res) => {
  const newUser = req.body;
  // Save to database
  res.status(201).json(newUser);
});

app.listen(3000, () => {
  console.log('Server running on port 3000');
});
```

## RESTful API Design

```javascript
// Proper REST endpoints
GET    /api/users              // List all users
GET    /api/users/123          // Get user by ID
POST   /api/users              // Create new user
PUT    /api/users/123          // Update entire user
PATCH  /api/users/123          // Partial update
DELETE /api/users/123          // Delete user
```

## Database Fundamentals

### SQL Query Examples

```sql
-- Create table
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100) NOT NULL,
  email VARCHAR(100) UNIQUE,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- Insert data
INSERT INTO users (name, email)
VALUES ('Alice', 'alice@example.com');

-- Query data
SELECT * FROM users WHERE id = 1;

-- Join tables
SELECT users.name, posts.title
FROM users
INNER JOIN posts ON users.id = posts.user_id;

-- Aggregation
SELECT COUNT(*) as total_users FROM users;
```

### Database Indexing

```sql
-- Create index for faster queries
CREATE INDEX idx_user_email ON users(email);

-- This makes this query fast:
SELECT * FROM users WHERE email = 'alice@example.com';
```

## Authentication with JWT

```javascript
const jwt = require('jsonwebtoken');

const SECRET = 'your-secret-key';

// Generate token
function generateToken(userId) {
  return jwt.sign({ userId }, SECRET, { expiresIn: '24h' });
}

// Verify token
function verifyToken(token) {
  try {
    return jwt.verify(token, SECRET);
  } catch (error) {
    return null;
  }
}

// Middleware to check token
function authenticateToken(req, res, next) {
  const authHeader = req.headers['authorization'];
  const token = authHeader && authHeader.split(' ')[1];

  if (!token) return res.sendStatus(401);

  const decoded = verifyToken(token);
  if (!decoded) return res.sendStatus(403);

  req.userId = decoded.userId;
  next();
}

// Protected route
app.get('/api/profile', authenticateToken, (req, res) => {
  res.json({ userId: req.userId });
});
```

## Error Handling

```javascript
// Global error handler
app.use((error, req, res, next) => {
  console.error(error);

  const status = error.status || 500;
  const message = error.message || 'Internal Server Error';

  res.status(status).json({
    error: {
      status,
      message
    }
  });
});

// Custom error class
class ValidationError extends Error {
  constructor(message) {
    super(message);
    this.status = 400;
  }
}
```

## Database Connections with Prisma

```javascript
// prisma/schema.prisma
model User {
  id    Int     @id @default(autoincrement())
  name  String
  email String  @unique
}

// Usage
const { PrismaClient } = require('@prisma/client');
const prisma = new PrismaClient();

// Query
const user = await prisma.user.findUnique({
  where: { email: 'alice@example.com' }
});

// Create
const newUser = await prisma.user.create({
  data: { name: 'Alice', email: 'alice@example.com' }
});

// Update
const updated = await prisma.user.update({
  where: { id: 1 },
  data: { name: 'Alice Smith' }
});

// Delete
await prisma.user.delete({
  where: { id: 1 }
});
```

## Testing APIs

```javascript
// Using Jest and Supertest
const request = require('supertest');
const app = require('./app');

describe('GET /api/users', () => {
  it('should return all users', async () => {
    const response = await request(app).get('/api/users');
    expect(response.status).toBe(200);
    expect(Array.isArray(response.body)).toBe(true);
  });
});

describe('POST /api/users', () => {
  it('should create a new user', async () => {
    const response = await request(app)
      .post('/api/users')
      .send({ name: 'Test', email: 'test@example.com' });
    expect(response.status).toBe(201);
    expect(response.body.id).toBeDefined();
  });
});
```

## Security Best Practices

```javascript
// Input validation
const { body, validationResult } = require('express-validator');

app.post('/api/users',
  body('email').isEmail(),
  body('password').isLength({ min: 8 }),
  (req, res) => {
    const errors = validationResult(req);
    if (!errors.isEmpty()) {
      return res.status(400).json({ errors: errors.array() });
    }
    // Process valid data
  }
);

// Use environment variables
require('dotenv').config();
const DATABASE_URL = process.env.DATABASE_URL;
const API_KEY = process.env.API_KEY;

// CORS configuration
const cors = require('cors');
app.use(cors({
  origin: 'https://yourdomain.com',
  credentials: true
}));

// Rate limiting
const rateLimit = require('express-rate-limit');
const limiter = rateLimit({
  windowMs: 15 * 60 * 1000, // 15 minutes
  max: 100 // limit each IP to 100 requests per windowMs
});
app.use('/api/', limiter);
```

## Caching Strategy

```javascript
// Redis caching
const redis = require('redis');
const client = redis.createClient();

app.get('/api/users/:id', async (req, res) => {
  const cacheKey = `user:${req.params.id}`;

  // Check cache
  const cached = await client.get(cacheKey);
  if (cached) return res.json(JSON.parse(cached));

  // Get from database
  const user = await User.findById(req.params.id);

  // Store in cache for 1 hour
  await client.setex(cacheKey, 3600, JSON.stringify(user));

  res.json(user);
});
```

## Logging

```javascript
const winston = require('winston');

const logger = winston.createLogger({
  level: 'info',
  format: winston.format.json(),
  transports: [
    new winston.transports.File({ filename: 'error.log', level: 'error' }),
    new winston.transports.File({ filename: 'combined.log' })
  ]
});

app.use((req, res, next) => {
  logger.info(`${req.method} ${req.path}`);
  next();
});

try {
  // Some operation
} catch (error) {
  logger.error('Operation failed', { error: error.message });
}
```

## GraphQL Basics

```javascript
const { graphql, buildSchema } = require('graphql');

const schema = buildSchema(`
  type Query {
    hello: String
    user(id: Int!): User
  }

  type User {
    id: Int
    name: String
    email: String
  }
`);

const rootValue = {
  hello: () => 'Hello World',
  user: ({ id }) => {
    // Fetch from database
    return { id, name: 'Alice', email: 'alice@example.com' };
  }
};

// Query
graphql(schema, '{ user(id: 1) { name email } }', rootValue)
  .then(result => console.log(result));
```

## Deployment Checklist

- [ ] Environment variables configured
- [ ] Database migrations applied
- [ ] HTTPS enabled
- [ ] CORS properly configured
- [ ] Rate limiting enabled
- [ ] Error logging setup
- [ ] Health check endpoint available
- [ ] Database backups configured
- [ ] Monitoring and alerts set up
- [ ] Load balancing configured

## Common Patterns

### Service Layer
```javascript
// Separate business logic from routes
class UserService {
  async getUser(id) {
    // Business logic here
    return User.findById(id);
  }

  async createUser(data) {
    // Validation
    if (!data.email) throw new Error('Email required');
    return User.create(data);
  }
}
```

### Repository Pattern
```javascript
// Abstract data access
class UserRepository {
  async findById(id) { }
  async findAll() { }
  async create(data) { }
  async update(id, data) { }
  async delete(id) { }
}
```

## Next Steps

1. Master one programming language
2. Learn a web framework thoroughly
3. Understand SQL databases
4. Build a complete REST API
5. Implement authentication
6. Add comprehensive testing
7. Deploy to production
8. Monitor and optimize

## Resources

- Express.js Documentation
- MDN - HTTP and APIs
- PostgreSQL Documentation
- Redis Documentation
- Node.js Best Practices
