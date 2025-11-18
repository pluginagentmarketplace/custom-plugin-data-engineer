---
name: frontend-core-skills
description: Master HTML, CSS, JavaScript fundamentals - the essential building blocks of frontend development. Learn responsive design, DOM manipulation, and modern CSS layouts.
---

# Frontend Core Skills

## Quick Start

Frontend development starts with three core technologies:

```html
<!-- HTML for structure -->
<div class="container">
  <h1>Welcome to Web Development</h1>
  <button id="myButton">Click me!</button>
</div>
```

```css
/* CSS for styling */
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```

```javascript
// JavaScript for interactivity
document.getElementById('myButton').addEventListener('click', () => {
  alert('Hello, Frontend Developer!');
});
```

## HTML Fundamentals

### Semantic Markup
Use semantic HTML for accessibility and SEO:

```html
<header>
  <nav>Navigation</nav>
</header>

<main>
  <article>
    <h1>Article Title</h1>
    <p>Article content</p>
  </article>
</main>

<footer>
  Footer content
</footer>
```

### Forms
Build accessible forms:

```html
<form>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required>

  <label for="message">Message:</label>
  <textarea id="message" name="message"></textarea>

  <button type="submit">Send</button>
</form>
```

## CSS Mastery

### Flexbox Layout
Perfect for one-dimensional layouts:

```css
.flex-container {
  display: flex;
  justify-content: space-between;  /* Align horizontally */
  align-items: center;              /* Align vertically */
  gap: 20px;                        /* Space between items */
}
```

### CSS Grid
Perfect for two-dimensional layouts:

```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;  /* 3 columns */
  grid-gap: 20px;
  grid-auto-rows: minmax(100px, auto);
}
```

### Responsive Design
Mobile-first approach:

```css
/* Mobile first */
.container {
  width: 100%;
  padding: 10px;
}

/* Tablet and up */
@media (min-width: 768px) {
  .container {
    width: 750px;
    padding: 20px;
  }
}

/* Desktop and up */
@media (min-width: 1200px) {
  .container {
    width: 1170px;
  }
}
```

## JavaScript Essentials

### DOM Manipulation
```javascript
// Select elements
const button = document.getElementById('myButton');
const items = document.querySelectorAll('.item');

// Modify DOM
button.textContent = 'Click me!';
button.classList.add('active');
button.style.color = 'red';

// Add event listeners
button.addEventListener('click', () => {
  console.log('Button clicked!');
});

// Create and append elements
const newElement = document.createElement('div');
newElement.textContent = 'Hello!';
document.body.appendChild(newElement);
```

### Async JavaScript
```javascript
// Fetch API
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error(error));

// Async/await (modern approach)
async function getData() {
  try {
    const response = await fetch('https://api.example.com/data');
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

getData();
```

### ES6+ Features
```javascript
// Arrow functions
const add = (a, b) => a + b;

// Destructuring
const { name, age } = user;
const [first, second] = array;

// Template literals
const message = `Hello, ${name}!`;

// Spread operator
const combined = [...array1, ...array2];

// Classes
class User {
  constructor(name) {
    this.name = name;
  }

  greet() {
    return `Hello, ${this.name}!`;
  }
}
```

## Accessibility (A11y)

Make your sites accessible to everyone:

```html
<!-- Use semantic HTML -->
<button>Submit</button>  <!-- Not <div onclick> -->

<!-- Add alt text to images -->
<img src="photo.jpg" alt="Description of the image">

<!-- Label form inputs -->
<label for="username">Username:</label>
<input id="username" type="text">

<!-- Use ARIA when needed -->
<div role="alert" aria-live="polite">
  Important message
</div>
```

## Performance Tips

1. **Minimize CSS and JavaScript** - Reduce file sizes
2. **Use CSS Grid/Flexbox** - More efficient layouts
3. **Lazy load images** - Load only when needed
4. **Debounce/Throttle events** - Reduce function calls
5. **Use modern CSS** - CSS variables, Grid, Flexbox

## Common Patterns

### Component Pattern
```javascript
// Reusable component
function Card({ title, content, onClose }) {
  return `
    <div class="card">
      <h2>${title}</h2>
      <p>${content}</p>
      <button onclick="close()">Close</button>
    </div>
  `;
}
```

### Event Delegation
```javascript
// Listen on parent instead of each child
document.addEventListener('click', (e) => {
  if (e.target.classList.contains('btn')) {
    console.log('Button clicked:', e.target);
  }
});
```

## Testing

```javascript
// Simple test
function test(name, fn) {
  try {
    fn();
    console.log(`✓ ${name}`);
  } catch (error) {
    console.error(`✗ ${name}: ${error.message}`);
  }
}

test('add function', () => {
  const result = add(2, 3);
  if (result !== 5) throw new Error('Expected 5');
});
```

## Next Steps

1. Build a responsive website
2. Learn a frontend framework (React, Vue, Angular)
3. Master state management
4. Implement routing
5. Add testing to your projects
6. Deploy to production

## Resources

- **MDN Web Docs** - Comprehensive reference
- **Can I Use** - Browser compatibility
- **CSS-Tricks** - Advanced techniques
- **JavaScript.info** - In-depth tutorials
- **Frontend Mentor** - Practice projects

## Summary

Master these three core technologies first before moving to frameworks. Practice building projects without frameworks to deeply understand how the web works. This foundation will make learning any framework much easier.
