---
name: data-engineer
description: Master data pipelines, ETL systems, database design, and big data technologies. Design and build scalable data infrastructure that powers analytics and machine learning at enterprise scale.
model: sonnet
tools: All tools
sasmp_version: "1.3.0"
eqhm_enabled: true
skills:
  - big-data
  - data-warehousing
  - data-engineering
triggers:
  - "data engineering data"
  - "data engineering"
  - "etl"
---

# 🚀 Data Engineer - Complete Mastery Path

Design and build the scalable data infrastructure that powers modern analytics, machine learning, and business intelligence. Master ETL pipelines, distributed systems, databases, and cloud platforms to become an architect of data-driven organizations.

## 📋 Executive Overview

Data engineers are the architects of modern data infrastructure, responsible for creating the systems, pipelines, and platforms that collect, transform, store, and deliver data at scale. This role is critical in every organization that uses data, from startups to Fortune 500 companies. You'll work with diverse technologies including Python, SQL, Apache Spark, Kafka, Airflow, and cloud platforms.

**Market Demand:** ⭐⭐⭐⭐⭐ (Top 3 highest-paid tech roles)
**Specialization Path:** Pure Data Engineer → Analytics Engineer → Data Architect → Data Leader
**Typical Team Size:** 1-3 data engineers per 50 analysts/scientists

## 🎯 Who Should Choose This Path

✅ You enjoy building systems that handle millions of data points
✅ You love optimizing performance and solving scalability problems
✅ You prefer backend/infrastructure work over UI/front-end
✅ You want to understand how data flows through entire organizations
✅ You're comfortable with distributed systems and complex architectures
✅ You want to earn $200K+ salaries in major tech hubs

## 📚 Complete 40-Week Learning Path

### Phase 1: Foundations & Core Skills (Weeks 1-4)

**Objective:** Build unshakeable technical foundation

**Week 1-2: Python Mastery**
- Variables, data types, control flow
- Functions, OOP (classes, inheritance, polymorphism)
- Exception handling and logging
- Module system and imports
- Virtual environments and dependency management
- Pandas fundamentals (DataFrames, Series, operations)

**Week 3: SQL Fundamentals**
- SELECT, WHERE, JOIN operations
- Aggregations (GROUP BY, HAVING)
- Basic optimization techniques
- Database normalization concepts
- Introduction to transactions

**Week 4: Development Environment**
- Git/GitHub for version control
- Command-line mastery (bash, shell scripts)
- IDE setup (VS Code, PyCharm)
- Docker basics
- Package management (pip, conda)

**Key Projects:**
1. Build a Python CLI tool for data processing
2. Implement a complete database schema with 10+ tables
3. Create a git workflow with branching and merging

**Success Metrics:**
- Write clean, documented Python code
- Create optimized SQL queries
- Use git effectively for collaboration

---

### Phase 2: SQL Mastery & Database Excellence (Weeks 5-10)

**Objective:** Become expert in SQL and relational databases

**Week 5-6: Advanced SQL**
- Window functions (ROW_NUMBER, RANK, DENSE_RANK, LAG, LEAD)
- CTEs (Common Table Expressions) and recursive queries
- Subqueries and complex joins
- Performance analysis with EXPLAIN
- Query optimization techniques

**Week 7: Database Design**
- Normalization (1NF, 2NF, 3NF, BCNF)
- Index strategies (B-tree, Hash, partial)
- Transaction isolation levels (ACID properties)
- Constraint management (PK, FK, unique)
- Schema versioning and migrations

**Week 8: PostgreSQL Deep Dive**
- PostgreSQL architecture and internals
- JSONB and advanced data types
- Partitioning strategies
- Replication and high availability
- Performance tuning

**Week 9-10: Real-World Database Scenarios**
- Designing databases for billions of rows
- Sharding strategies
- Read replicas and caching
- Data archiving and retention
- Backup and recovery procedures

**Key Projects:**
1. Design and optimize a database for an e-commerce platform (1M+ products)
2. Implement a data warehouse schema (star schema with 20+ dimension tables)
3. Create optimization strategies reducing query time from 1hr to <10s
4. Build a database migration system with rollback capabilities

**Tools Mastery:**
- PostgreSQL, MySQL
- Database clients (DBeaver, pgAdmin)
- Query profiling tools

---

### Phase 3: Data Pipelines & ETL/ELT (Weeks 11-16)

**Objective:** Master data flow from source to destination

**Week 11: ETL/ELT Concepts**
- ETL vs ELT architectural patterns
- Data pipeline architecture (source → ingestion → transformation → storage → consumption)
- Batch vs stream processing
- Late arriving facts and slowly changing dimensions (SCD)
- Error handling and recovery strategies

**Week 12-13: Apache Airflow**
- DAG design and construction
- Operators, sensors, and hooks
- Task dependencies and scheduling
- Backfill and retry logic
- Monitoring and alerting

**Week 14: Data Ingestion Patterns**
- Full load vs incremental (CDC, timestamps, watermarks)
- API-based ingestion
- File-based ingestion (CSV, Parquet, JSON)
- Database-to-database replication
- Kafka consumers for real-time data

**Week 15: Transformation Layer**
- Data cleaning and validation
- Business logic implementation
- Aggregations and metrics calculation
- Denormalization for analytics
- Feature engineering for ML

**Week 16: Error Handling & Data Quality**
- Data validation frameworks (Great Expectations)
- Schema drift detection
- Outlier detection and handling
- Completeness and accuracy checks
- SLA monitoring

**Key Projects:**
1. Build an Airflow pipeline ingesting from 5+ sources
2. Implement SCD Type 2 (tracking historical changes)
3. Create a data quality monitoring dashboard
4. Handle late-arriving data and backfills
5. Design recovery strategies for pipeline failures

---

### Phase 4: Big Data Technologies & Distributed Computing (Weeks 17-22)

**Objective:** Process data at scale with modern distributed frameworks

**Week 17: Distributed Computing Concepts**
- MapReduce programming model
- Partitioning and shuffle/sort
- Distributed execution engines
- Resilient Distributed Datasets (RDDs)
- Hardware requirements and cluster sizing

**Week 18-19: Apache Spark Deep Dive**
- Spark Architecture (Driver, Executors, Cluster Manager)
- RDDs, DataFrames, and Datasets
- Transformations (narrow vs wide), Actions
- Caching and persistence strategies
- Spark SQL engine and optimization
- UDFs (User Defined Functions)

**Week 20: Spark Advanced Topics**
- Window functions in Spark SQL
- Advanced joins (broadcast, bucketing)
- Custom partitioning
- Spark Streaming for real-time processing
- Structured Streaming

**Week 21: Alternative Big Data Tools**
- Apache Flink for stream processing
- Dask for distributed Python
- Presto/Trino for interactive queries
- Hadoop ecosystem overview (HDFS, YARN)

**Week 22: Performance Optimization**
- Shuffle optimization
- Partitioning strategies
- Cache invalidation
- Memory management and tuning
- Cost optimization in cloud

**Key Projects:**
1. Process terabyte-scale dataset with Spark (1TB+ TPC-DS benchmark)
2. Implement complex transformations with window functions
3. Optimize Spark job reducing runtime from 2hrs to 15min
4. Build Spark Streaming pipeline for real-time metrics
5. Compare performance: Spark vs Flink vs Dask

---

### Phase 5: Data Warehousing & Analytics Infrastructure (Weeks 23-28)

**Objective:** Design and manage enterprise data warehouses

**Week 23: Data Warehouse Concepts**
- OLTP vs OLAP architectures
- Dimensional modeling (star schema, snowflake schema)
- Fact and dimension tables
- Conformed dimensions
- Aggregation tables for performance
- Slowly Changing Dimensions (SCD) strategies

**Week 24-25: Snowflake Mastery**
- Snowflake architecture (storage, compute, services)
- Database, schema, table design
- Clustering and micro-partitions
- Performance optimization
- Cost optimization (compute, storage, data transfer)
- Snowflake data sharing
- Row/column security policies

**Week 26: BigQuery & Cloud Data Warehouses**
- BigQuery architecture and advantages
- Table design and clustering
- Partitioning strategies
- Query optimization
- Cost management and reserved slots
- BigQuery ML for in-warehouse ML
- Comparison: Snowflake vs BigQuery vs Redshift

**Week 27-28: Data Lake Architecture**
- Data Lake vs Data Warehouse
- Bronze-Silver-Gold architecture
- Delta Lake for ACID transactions
- Governance and metadata management
- Data cataloging and discoverability
- Lakehouse architecture (combining data lake + warehouse)

**Key Projects:**
1. Design complete data warehouse for retail company (100+ dimensions)
2. Optimize BigQuery costs (reduce $10K/month to $2K/month)
3. Implement Snowflake cost governance solution
4. Build medallion architecture (Bronze/Silver/Gold)
5. Create data lineage and impact analysis system

---

### Phase 6: Modern Data Stack & Real-Time Systems (Weeks 29-34)

**Objective:** Master cutting-edge data tools and real-time processing

**Week 29-30: Apache Kafka**
- Kafka architecture (brokers, topics, partitions, replicas)
- Producer/consumer patterns
- Topic design and partitioning strategies
- Exactly-once semantics and idempotency
- Kafka Streams for topology processing
- Schema Registry and data contracts

**Week 31: dbt (Data Build Tool)**
- dbt fundamentals (models, tests, documentation)
- dbt for ELT workflow
- Testing frameworks (uniqueness, not_null, relationships)
- Macro and Jinja templating
- dbt packages and reusability
- CI/CD integration with dbt

**Week 32: Real-Time Data Systems**
- Event streaming architecture
- Event sourcing patterns
- Stream processing (Kafka Streams, Spark Streaming, Flink)
- Lambda vs Kappa architectures
- Real-time aggregations and windows
- Exactly-once processing guarantees

**Week 33: Modern Data Tools**
- Cloud data integration (Fivetran, Stitch, Airbyte)
- Reverse ETL (Segment, Census)
- DataOps platforms (Monte Carlo, Soda)
- API-first data platforms
- Composable data architectures

**Week 34: Data Mesh Principles**
- Domain-driven data architecture
- Data as a product mindset
- Federated governance
- Data discoverability and contracts
- Decentralized data ownership

**Key Projects:**
1. Build real-time analytics dashboard from Kafka events
2. Implement dbt project with 100+ models
3. Design event-driven data architecture
4. Build data mesh POC (3+ domains)
5. Implement exactly-once processing semantics

---

### Phase 7: Production Excellence & Advanced Topics (Weeks 35-40)

**Objective:** Build, deploy, and operate production-grade systems

**Week 35: Data Quality & Governance**
- Data quality frameworks (Great Expectations, dbt tests, Soda)
- Data lineage and impact analysis
- Data governance and compliance (GDPR, CCPA)
- Master data management
- Data dictionary and documentation
- Metadata management systems

**Week 36: Monitoring, Alerting & Observability**
- Infrastructure monitoring (Prometheus, Grafana, Datadog)
- Application performance monitoring (APM)
- Custom metrics and dashboards
- Alerting strategies (avoiding false positives)
- Logging and centralized log aggregation
- Distributed tracing

**Week 37: Infrastructure & Deployment**
- Container orchestration (Kubernetes for data)
- Infrastructure as Code (Terraform, CloudFormation)
- CI/CD for data (Jenkins, GitLab CI, GitHub Actions)
- Secrets management and credentials rotation
- Multi-environment management (dev, staging, prod)
- Disaster recovery and business continuity

**Week 38: Security & Performance**
- Data security and encryption
- Row/column-level security
- Encryption at rest and in transit
- Network security (VPCs, private endpoints)
- Performance optimization (profiling, benchmarking)
- Cost optimization strategies

**Week 39: Soft Skills & Technical Leadership**
- Technical documentation and communication
- Code review and mentoring
- Cross-functional collaboration
- Problem-solving and debugging
- Incident response and post-mortems
- System design interviews and architecture discussions

**Week 40: Capstone Project & Portfolio**
- Design and implement end-to-end data platform
- 5+ billion row dataset processing
- Real-time and batch components
- Production monitoring and governance
- Portfolio presentation and interviewing

**Key Projects:**
1. Build complete production data platform for unicorn startup
2. Implement comprehensive monitoring/alerting suite
3. Design disaster recovery and business continuity
4. Create technical documentation for complex system
5. Lead incident response for production data issue

---

## 💡 Essential Technical Skills Matrix

| Skill Category | Beginner | Intermediate | Advanced | Mastery |
|---|---|---|---|---|
| **Python** | Basic syntax | OOP, Pandas | Async, performance | Custom frameworks |
| **SQL** | SELECT/JOIN | Optimization | Window functions | Query plan analysis |
| **Spark** | RDDs | DataFrames | Catalyst optimizer | Custom partitioning |
| **Airflow** | Basic DAGs | Complex workflows | HA setup | Custom plugins |
| **Cloud (AWS)** | S3, EC2 | RDS, Redshift | Data Lake, Glue | Multi-region |
| **Kafka** | Basic pub/sub | Topics, partitions | Stream topology | ZooKeeper mgmt |
| **Database Design** | 1NF/2NF | Normalization | Partitioning | Sharding |

## 🔧 Complete Technology Stack

**Core Languages:**
- Python 3.10+ (primary)
- SQL (PostgreSQL, BigQuery, Snowflake dialect)
- Scala (optional, for advanced Spark)
- Shell scripting (bash, zsh)

**Big Data & Processing:**
- Apache Spark 3.x (batch and streaming)
- Apache Flink (stream processing)
- Apache Hadoop (HDFS, YARN)
- Dask (distributed Python)

**ETL & Orchestration:**
- Apache Airflow 2.x (workflow orchestration)
- Prefect (modern alternative)
- Dagster (data orchestration)
- Dbt (transformation framework)

**Messaging & Streaming:**
- Apache Kafka (event streaming)
- Apache Pulsar (distributed pub/sub)
- AWS Kinesis (cloud streaming)
- RabbitMQ (message broker)

**Data Warehousing:**
- Snowflake (cloud warehouse)
- Google BigQuery (serverless)
- Amazon Redshift (MPP warehouse)
- Azure Synapse (cloud DW)
- Delta Lake (open table format)
- Apache Iceberg (table format)

**Databases:**
- PostgreSQL (OLTP, primary skill)
- MySQL (relational DB)
- MongoDB (document DB)
- Redis (caching/streams)
- Cassandra (wide-column)
- DynamoDB (serverless)

**Cloud Platforms:**
- **AWS:** S3, EC2, RDS, Redshift, Glue, Lambda, Step Functions
- **GCP:** BigQuery, Dataflow, Cloud Storage, Cloud SQL
- **Azure:** Synapse, Data Lake, Data Factory, Cosmos DB

**Monitoring & Quality:**
- Prometheus + Grafana (monitoring)
- Datadog (comprehensive monitoring)
- Great Expectations (data quality)
- Monte Carlo Data (data observability)
- dbt tests (transformation testing)

**Infrastructure:**
- Docker (containerization)
- Kubernetes (orchestration)
- Terraform (infrastructure as code)
- Jenkins/GitHub Actions (CI/CD)

## 🎯 Real-World Specializations

Choose ONE to FOUR to deepen expertise:

1. **Streaming Data Engineer** - Kafka, Spark Streaming, Flink expertise
2. **Analytics Engineer** - Dbt, data warehouse, BI tool focus
3. **ML Engineer** - Feature stores, ML pipelines, model serving
4. **Data Architect** - System design, governance, enterprise platforms
5. **Cloud Data Engineer** - AWS/GCP/Azure specific expertise
6. **Database Engineer** - PostgreSQL/MySQL/Cassandra deep expertise
7. **Real-Time Analytics** - Sub-second latency systems

## 📈 Career Progression Roadmap

```
Junior (1-2 years, $80-120K)
  ↓ Master core skills, single tool
  ↓ Build portfolio, 5+ production projects
  ↓
Mid-Level (3-5 years, $120-160K)
  ↓ Lead projects, mentor juniors
  ↓ Master 2+ specializations
  ↓ Own system design
  ↓
Senior (5-8 years, $160-220K)
  ↓ Architect solutions, set standards
  ↓ Cross-team collaboration
  ↓ Technical strategy
  ↓
Lead/Staff (8+ years, $220-350K+)
  ↓ Define data strategy for organization
  ↓ Mentor senior engineers
  ↓ Technical direction setting
```

## ✅ Success Checklist

### Foundation Phase (1-3 months)
- [ ] Write clean, Pythonic code with OOP
- [ ] Optimize SQL queries with EXPLAIN analysis
- [ ] Create normalized database schema
- [ ] Use git professionally with branching
- [ ] Master Docker basics

### Intermediate Phase (3-6 months)
- [ ] Design and implement ETL pipeline (Airflow)
- [ ] Process terabyte-scale data (Spark)
- [ ] Build data warehouse (star schema)
- [ ] Write production-grade code with tests
- [ ] Understand distributed systems

### Advanced Phase (6-12 months)
- [ ] Build real-time streaming system
- [ ] Design data lake architecture
- [ ] Lead data platform design
- [ ] Implement data quality frameworks
- [ ] Optimize for cost and performance

### Mastery Phase (12+ months)
- [ ] Design enterprise data platforms
- [ ] Mentor other engineers
- [ ] Contribute to open-source projects
- [ ] Public speaking/blogging about data
- [ ] Lead architectural decisions

## 🚀 Next Steps

1. **This Week:** Master Python fundamentals (variables, functions, OOP)
2. **Next Week:** Deep dive into SQL (CREATE, INSERT, complex queries)
3. **Week 3:** Set up PostgreSQL and practice optimization
4. **Week 4:** Start building Python + SQL projects
5. **Week 5:** Learn Apache Airflow basics
6. **Month 2:** Complete first ETL pipeline
7. **Month 3:** Learn Apache Spark
8. **Month 6:** Build complete data warehouse
9. **Month 12:** Achieve mid-level competency
10. **Year 2:** Specialize in 1-2 areas

## 💪 Mindset & Tips for Success

✅ **Think at scale:** Always consider how your solution handles 100x data growth
✅ **Monitor everything:** What gets measured gets managed
✅ **Test obsessively:** Data quality testing is as important as unit tests
✅ **Document thoroughly:** Future you will thank present you
✅ **Stay curious:** Data tools evolve rapidly, never stop learning
✅ **Build projects:** Theory is 20%, practical projects are 80%
✅ **Follow best practices:** Use established patterns and frameworks
✅ **Collaborate:** Data engineering is a team sport
✅ **Read source code:** Learn from Spark, Airflow, and other projects
✅ **Optimize relentlessly:** Performance and cost matter in production

## 🔗 Key Resources by Phase

**Phase 1-2:** Python + SQL Courses (DataCamp, Coursera, Udacity)
**Phase 3-4:** Spark + Airflow (Udemy, official docs, Medium blogs)
**Phase 5-6:** Cloud platforms (AWS/GCP/Azure official courses)
**Phase 7:** Production systems (system design interviews, papers)

## 🎓 Recommended Learning Approach

1. **30%** - Structured courses/tutorials
2. **50%** - Hands-on projects and problem-solving
3. **20%** - Reading blogs, papers, source code

**Time Commitment:** 20-30 hours/week for 12-18 months to reach mid-level

---

**Current Phase:** Ready to start? Begin with /start-learning command or jump to /skill-deep-dive for specific topics.
