<div align="center">

# Data Engineer Development Assistant

### Complete Data Engineering Mastery for Claude Code

**Master data pipelines, ETL, databases, cloud platforms, and MLOps with 6 specialized agents and 21 production-ready skills**

[![Verified](https://img.shields.io/badge/Verified-Working-success?style=flat-square&logo=checkmarx)](https://github.com/pluginagentmarketplace/custom-plugin-data-engineer)
[![License](https://img.shields.io/badge/License-Custom-yellow?style=flat-square)](LICENSE)
[![Version](https://img.shields.io/badge/Version-2.0.0-blue?style=flat-square)](https://github.com/pluginagentmarketplace/custom-plugin-data-engineer)
[![Status](https://img.shields.io/badge/Status-Production_Ready-brightgreen?style=flat-square)](https://github.com/pluginagentmarketplace/custom-plugin-data-engineer)
[![Agents](https://img.shields.io/badge/Agents-6-orange?style=flat-square)](#agents-overview)
[![Skills](https://img.shields.io/badge/Skills-21-purple?style=flat-square)](#skills-reference)
[![SASMP](https://img.shields.io/badge/SASMP-v1.3.0-blueviolet?style=flat-square)](#)

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](skills/python-programming/)
[![Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)](skills/big-data/)
[![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)](skills/etl-tools/)
[![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)](skills/cloud-platforms/)

[Quick Start](#quick-start) | [Agents](#agents-overview) | [Skills](#skills-reference) | [Commands](#commands)

</div>

---

## Verified Installation

> **This plugin has been tested and verified working on Claude Code.**
> Last verified: December 2025

---

## Quick Start

### Option 1: Install from GitHub (Recommended)

```bash
# Step 1: Add the marketplace from GitHub
/plugin add marketplace pluginagentmarketplace/custom-plugin-data-engineer

# Step 2: Install the plugin
/plugin install data-engineer-development-assistant@pluginagentmarketplace-data-engineer

# Step 3: Restart Claude Code to load new plugins
```

### Option 2: Clone and Load Locally

```bash
# Clone the repository
git clone https://github.com/pluginagentmarketplace/custom-plugin-data-engineer.git

# Navigate to the directory in Claude Code
cd custom-plugin-data-engineer

# Load the plugin
/plugin load .
```

After loading, restart Claude Code.

### Verify Installation

After restarting Claude Code, verify the plugin is loaded. You should see these agents available:

```
custom-plugin-data-engineer:01-data-engineer
custom-plugin-data-engineer:02-backend-developer
custom-plugin-data-engineer:03-devops-engineer
custom-plugin-data-engineer:04-data-scientist
custom-plugin-data-engineer:05-cloud-engineer
custom-plugin-data-engineer:06-ml-ai-engineer
```

---

## Available Skills

Once installed, these 21 skills become available:

| Skill | Invoke Command | Golden Format |
|-------|----------------|---------------|
| Python Programming | `Skill("custom-plugin-data-engineer:python-programming")` | python-patterns.yaml |
| SQL & Databases | `Skill("custom-plugin-data-engineer:sql-databases")` | sql-optimization.yaml |
| NoSQL & Data Stores | `Skill("custom-plugin-data-engineer:nosql-databases")` | nosql-patterns.yaml |
| Data Engineering Core | `Skill("custom-plugin-data-engineer:data-engineering")` | pipeline-template.yaml |
| ETL Tools | `Skill("custom-plugin-data-engineer:etl-tools")` | airflow-dag.yaml |
| Big Data | `Skill("custom-plugin-data-engineer:big-data")` | spark-config.yaml |
| Data Warehousing | `Skill("custom-plugin-data-engineer:data-warehousing")` | warehouse-schema.yaml |
| Statistics & Math | `Skill("custom-plugin-data-engineer:statistics-math")` | statistical-methods.yaml |
| Machine Learning | `Skill("custom-plugin-data-engineer:machine-learning")` | ml-pipeline.yaml |
| Deep Learning | `Skill("custom-plugin-data-engineer:deep-learning")` | neural-network.yaml |
| LLMs & Generative AI | `Skill("custom-plugin-data-engineer:llms-generative-ai")` | rag-system.yaml |
| API Development | `Skill("custom-plugin-data-engineer:api-development")` | fastapi-template.yaml |
| Cloud Platforms | `Skill("custom-plugin-data-engineer:cloud-platforms")` | aws-data-stack.yaml |
| Containerization | `Skill("custom-plugin-data-engineer:containerization")` | docker-compose.yaml |
| Infrastructure as Code | `Skill("custom-plugin-data-engineer:iac-automation")` | terraform-module.yaml |
| CI/CD Pipelines | `Skill("custom-plugin-data-engineer:cicd-pipelines")` | github-actions.yaml |
| MLOps | `Skill("custom-plugin-data-engineer:mlops")` | mlflow-config.yaml |
| Monitoring | `Skill("custom-plugin-data-engineer:monitoring-observability")` | prometheus-rules.yaml |
| Git & Version Control | `Skill("custom-plugin-data-engineer:git-version-control")` | git-workflow.yaml |
| Testing & Quality | `Skill("custom-plugin-data-engineer:testing-quality")` | pytest-config.yaml |
| Career Growth | `Skill("custom-plugin-data-engineer:career-growth")` | career-roadmap.yaml |

---

## What This Plugin Does

This plugin provides **6 specialized agents** and **21 production-ready skills** for data engineering mastery:

| Agent | Purpose |
|-------|---------|
| **Data Engineer** | Data pipelines, ETL/ELT, Spark, Airflow, Kafka |
| **Backend Developer** | APIs for data applications, microservices |
| **DevOps Engineer** | Infrastructure automation, CI/CD, reliability |
| **Data Scientist** | ML models, statistics, experimentation |
| **Cloud Engineer** | AWS/GCP/Azure data services, cost optimization |
| **ML/AI Engineer** | Deep learning, LLMs, production ML systems |

---

## Agents Overview

### 6 Implementation Agents

Each agent is designed to **do the work**, not just explain:

| Agent | Capabilities | Example Prompts |
|-------|--------------|-----------------|
| **Data Engineer** | ETL pipelines, Spark jobs, data modeling | `"Build Airflow DAG"`, `"Create Spark pipeline"` |
| **Backend Developer** | FastAPI, data APIs, microservices | `"Create data API"`, `"Build ingestion service"` |
| **DevOps Engineer** | Docker, K8s, Terraform, monitoring | `"Containerize pipeline"`, `"Set up Prometheus"` |
| **Data Scientist** | ML models, Pandas, feature engineering | `"Train classifier"`, `"Analyze dataset"` |
| **Cloud Engineer** | AWS Glue, BigQuery, Redshift, Snowflake | `"Design data lake"`, `"Optimize cloud costs"` |
| **ML/AI Engineer** | PyTorch, TensorFlow, LLMs, RAG systems | `"Build RAG pipeline"`, `"Deploy ML model"` |

---

## Commands

7 interactive commands for data engineering workflows:

| Command | Usage | Description |
|---------|-------|-------------|
| `/start-learning` | `/start-learning` | Begin personalized learning journey |
| `/choose-role` | `/choose-role` | Select specialization to focus on |
| `/skill-deep-dive` | `/skill-deep-dive sql` | Master a specific technology |
| `/project-ideas` | `/project-ideas intermediate` | Get hands-on project ideas |
| `/roadmap-status` | `/roadmap-status` | Check learning progress |
| `/interview-prep` | `/interview-prep data-engineer` | Prepare for technical interviews |
| `/assessment` | `/assessment python` | Evaluate knowledge and find gaps |

---

## Skills Reference

Each skill includes **Golden Format** content:
- `assets/` - YAML templates and configurations
- `scripts/` - Automation and validation scripts
- `references/` - Methodology guides and best practices

### All 21 Skills by Category

| Category | Skills |
|----------|--------|
| **Fundamentals** | python-programming, sql-databases, git-version-control |
| **Data Engineering** | data-engineering, etl-tools, big-data, data-warehousing, monitoring-observability |
| **Databases** | nosql-databases |
| **ML & AI** | statistics-math, machine-learning, deep-learning, llms-generative-ai |
| **Cloud & Infrastructure** | cloud-platforms, containerization, iac-automation, cicd-pipelines |
| **Production** | mlops, api-development, testing-quality |
| **Professional** | career-growth |

---

## Usage Examples

### Example 1: Create ETL Pipeline with Airflow

```python
# Before: Manual data processing

# After (with Data Engineer agent):
Skill("custom-plugin-data-engineer:etl-tools")

# Generates:
# - Airflow DAG with proper scheduling
# - Data quality checks
# - Error handling and retry logic
# - Monitoring and alerting
```

### Example 2: Build Data API with FastAPI

```python
# Before: Basic Flask endpoint

# After (with Backend Developer agent):
Skill("custom-plugin-data-engineer:api-development")

# Provides:
# - FastAPI async endpoints
# - Pydantic validation
# - Database connection pooling
# - Rate limiting and caching
```

### Example 3: Deploy to Cloud Data Platform

```yaml
# Before: Manual cloud setup

# After (with Cloud Engineer agent):
Skill("custom-plugin-data-engineer:cloud-platforms")

# Creates:
# - AWS Glue jobs for ETL
# - S3 data lake structure
# - Redshift warehouse schema
# - IAM policies and roles
```

---

## Plugin Structure

```
custom-plugin-data-engineer/
├── .claude-plugin/
│   ├── plugin.json           # Plugin manifest
│   └── marketplace.json      # Marketplace config
├── agents/                   # 6 specialized agents
│   ├── 01-data-engineer.md
│   ├── 02-backend-developer.md
│   ├── 03-devops-engineer.md
│   ├── 04-data-scientist.md
│   ├── 05-cloud-engineer.md
│   └── 06-ml-ai-engineer.md
├── skills/                   # 21 skills (Golden Format)
│   ├── python-programming/
│   │   ├── SKILL.md
│   │   ├── assets/
│   │   ├── scripts/
│   │   └── references/
│   ├── sql-databases/
│   ├── data-engineering/
│   ├── etl-tools/
│   ├── big-data/
│   └── ... (16 more skills)
├── commands/                 # 7 slash commands
│   ├── start-learning.md
│   ├── choose-role.md
│   ├── skill-deep-dive.md
│   ├── project-ideas.md
│   ├── roadmap-status.md
│   ├── interview-prep.md
│   └── assessment.md
├── hooks/hooks.json
├── README.md
├── CHANGELOG.md
├── CONTRIBUTING.md
├── ARCHITECTURE.md
└── LICENSE
```

---

## Technology Coverage

| Category | Technologies |
|----------|--------------|
| **Languages** | Python, SQL, Scala, Go, Bash |
| **Big Data** | Apache Spark, Hadoop, Flink, Dask, Presto |
| **Streaming** | Apache Kafka, AWS Kinesis, Google Pub/Sub |
| **Orchestration** | Apache Airflow, Prefect, Dagster, Temporal |
| **Warehousing** | Snowflake, BigQuery, Redshift, Delta Lake |
| **Databases** | PostgreSQL, MongoDB, Redis, Cassandra, DynamoDB |
| **Cloud** | AWS (S3, Glue, EMR), GCP (BigQuery, Dataflow), Azure (Synapse) |
| **ML Frameworks** | TensorFlow, PyTorch, Scikit-learn, XGBoost |
| **Infrastructure** | Docker, Kubernetes, Terraform, Ansible |
| **Monitoring** | Prometheus, Grafana, Datadog, ELK Stack |

---

## Learning Paths

| Path | Duration | Focus |
|------|----------|-------|
| Data Engineer | 40 weeks | ETL, Spark, Airflow, warehousing |
| Backend + Data | 36 weeks | APIs, data services, microservices |
| DevOps + Data | 40 weeks | Infrastructure, CI/CD, reliability |
| ML Engineer | 40 weeks | Deep learning, LLMs, production ML |
| Cloud Data | 36 weeks | AWS/GCP/Azure data services |

---

## Security Notice

This plugin is designed for **authorized development use only**:

**USE FOR:**
- Learning data engineering
- Building data pipelines
- Cloud data platform development
- ML/AI system implementation

**SECURITY TOPICS:**
- Data encryption at rest and in transit
- Access control and IAM
- Data privacy compliance (GDPR, CCPA)
- Secure credential management

---

## Metadata

| Field | Value |
|-------|-------|
| **Last Updated** | 2025-12-28 |
| **Maintenance Status** | Active |
| **SASMP Version** | 1.3.0 |
| **Support** | [Issues](../../issues) |

---

## License

Custom License - See [LICENSE](LICENSE) for details.

Copyright (c) 2025 Dr. Umit Kacar & Muhsin Elcicek

---

## Contributing

Contributions are welcome:

1. Fork the repository
2. Create a feature branch
3. Follow the Golden Format for new skills
4. Submit a pull request

See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

---

## Contributors

**Authors:**
- **Dr. Umit Kacar** - Senior AI Researcher & Engineer
- **Muhsin Elcicek** - Senior Software Architect

---

<div align="center">

**Master data engineering with AI assistance!**

[![Made for Data](https://img.shields.io/badge/Made%20for-Data%20Engineering-3776AB?style=for-the-badge&logo=python)](https://github.com/pluginagentmarketplace/custom-plugin-data-engineer)

**Built by Dr. Umit Kacar & Muhsin Elcicek**

*Based on [roadmap.sh/data-engineer](https://roadmap.sh/data-engineer)*

</div>
