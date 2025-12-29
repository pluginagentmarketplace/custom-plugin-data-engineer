<div align="center">

<!-- Animated Typing Banner -->
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=3000&pause=1000&color=2E9EF7&center=true&vCenter=true&multiline=true&repeat=true&width=600&height=100&lines=Data+Engineer+Assistant;6+Agents+%7C+21+Skills;Claude+Code+Plugin" alt="Data Engineer Assistant" />

<br/>

<!-- Badge Row 1: Status Badges -->
[![Version](https://img.shields.io/badge/Version-2.0.0-blue?style=for-the-badge)](https://github.com/pluginagentmarketplace/custom-plugin-data-engineer/releases)
[![License](https://img.shields.io/badge/License-Custom-yellow?style=for-the-badge)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Production-brightgreen?style=for-the-badge)](#)
[![SASMP](https://img.shields.io/badge/SASMP-v1.3.0-blueviolet?style=for-the-badge)](#)

<!-- Badge Row 2: Content Badges -->
[![Agents](https://img.shields.io/badge/Agents-6-orange?style=flat-square&logo=robot)](#-agents)
[![Skills](https://img.shields.io/badge/Skills-21-purple?style=flat-square&logo=lightning)](#-skills)
[![Commands](https://img.shields.io/badge/Commands-7-green?style=flat-square&logo=terminal)](#-commands)

<br/>

<!-- Quick CTA Row -->
[📦 **Install Now**](#-quick-start) · [🤖 **Explore Agents**](#-agents) · [📖 **Documentation**](#-documentation) · [⭐ **Star this repo**](https://github.com/pluginagentmarketplace/custom-plugin-data-engineer)

---

### What is this?

> **Data Engineer Assistant** is a Claude Code plugin with **6 agents** and **21 skills** for data engineer development.

</div>

---

## 📑 Table of Contents

<details>
<summary>Click to expand</summary>

- [Quick Start](#-quick-start)
- [Features](#-features)
- [Agents](#-agents)
- [Skills](#-skills)
- [Commands](#-commands)
- [Documentation](#-documentation)
- [Contributing](#-contributing)
- [License](#-license)

</details>

---

## 🚀 Quick Start

### Prerequisites

- Claude Code CLI v2.0.27+
- Active Claude subscription

### Installation (Choose One)

<details open>
<summary><strong>Option 1: From Marketplace (Recommended)</strong></summary>

```bash
# Step 1️⃣ Add the marketplace
/plugin add marketplace pluginagentmarketplace/custom-plugin-data-engineer

# Step 2️⃣ Install the plugin
/plugin install data-engineer-development-assistant@pluginagentmarketplace-data-engineer

# Step 3️⃣ Restart Claude Code
# Close and reopen your terminal/IDE
```

</details>

<details>
<summary><strong>Option 2: Local Installation</strong></summary>

```bash
# Clone the repository
git clone https://github.com/pluginagentmarketplace/custom-plugin-data-engineer.git
cd custom-plugin-data-engineer

# Load locally
/plugin load .

# Restart Claude Code
```

</details>

### ✅ Verify Installation

After restart, you should see these agents:

```
data-engineer-development-assistant:03-devops-engineer
data-engineer-development-assistant:01-data-engineer
data-engineer-development-assistant:02-backend-developer
data-engineer-development-assistant:04-data-scientist
data-engineer-development-assistant:05-cloud-engineer
... and 1 more
```

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🤖 **6 Agents** | Specialized AI agents for data engineer tasks |
| 🛠️ **21 Skills** | Reusable capabilities with Golden Format |
| ⌨️ **7 Commands** | Quick slash commands |
| 🔄 **SASMP v1.3.0** | Full protocol compliance |

---

## 🤖 Agents

### 6 Specialized Agents

| # | Agent | Purpose |
|---|-------|---------|
| 1 | **03-devops-engineer** | Master infrastructure automation, deployment pipelines, and  |
| 2 | **01-data-engineer** | Master data pipelines, ETL systems, database design, and big |
| 3 | **02-backend-developer** | Build robust, scalable backend systems and APIs that power m |
| 4 | **04-data-scientist** | Transform data into actionable insights using machine learni |
| 5 | **05-cloud-engineer** | Design and manage cloud infrastructure and data platforms on |
| 6 | **06-ml-ai-engineer** | Master artificial intelligence, large language models, gener |

---

## 🛠️ Skills

### Available Skills

| Skill | Description | Invoke |
|-------|-------------|--------|
| `deep-learning` | TensorFlow, PyTorch, CNNs, RNNs, transformers, neural networ | `Skill("data-engineer-development-assistant:deep-learning")` |
| `big-data` | Apache Spark, Hadoop, distributed computing, and large-scale | `Skill("data-engineer-development-assistant:big-data")` |
| `api-development` | REST APIs, GraphQL, FastAPI, data service design, and integr | `Skill("data-engineer-development-assistant:api-development")` |
| `etl-tools` | Apache Airflow, Spark, Kafka, Flink, dbt, and modern data tr | `Skill("data-engineer-development-assistant:etl-tools")` |
| `cloud-platforms` | AWS, Azure, GCP data platforms and cloud-native data solutio | `Skill("data-engineer-development-assistant:cloud-platforms")` |
| `mlops` | Model versioning, MLflow, experiment tracking, model registr | `Skill("data-engineer-development-assistant:mlops")` |
| `data-warehousing` | Snowflake, BigQuery, Redshift, Delta Lake, and data warehous | `Skill("data-engineer-development-assistant:data-warehousing")` |
| `containerization` | Docker, Kubernetes, and container orchestration for data app | `Skill("data-engineer-development-assistant:containerization")` |
| `sql-databases` | SQL query optimization, schema design, indexing, and relatio | `Skill("data-engineer-development-assistant:sql-databases")` |
| `cicd-pipelines` | Jenkins, GitHub Actions, GitLab CI, and automated data pipel | `Skill("data-engineer-development-assistant:cicd-pipelines")` |
| ... | +11 more | See skills/ directory |

---

## ⌨️ Commands

| Command | Description |
|---------|-------------|
| `/choose-role` | 🎯 Choose Role - Pick Your Data Specialty |
| `/project-ideas` | 🚀 Project Ideas - Build Your Portfolio |
| `/skill-deep-dive` | 🔍 Skill Deep Dive - Master Any Technology |
| `/assessment` | 📋 Assessment - Evaluate Your Knowledge |
| `/roadmap-status` | 📊 Roadmap Status - Track Your Progress |
| `/interview-prep` | 💼 Interview Prep - Get Data Engineering Jobs |
| `/start-learning` | 🚀 Start Learning - Data Engineering Roadmap |

---

## 📚 Documentation

| Document | Description |
|----------|-------------|
| [CHANGELOG.md](CHANGELOG.md) | Version history |
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to contribute |
| [LICENSE](LICENSE) | License information |

---

## 📁 Project Structure

<details>
<summary>Click to expand</summary>

```
custom-plugin-data-engineer/
├── 📁 .claude-plugin/
│   ├── plugin.json
│   └── marketplace.json
├── 📁 agents/              # 6 agents
├── 📁 skills/              # 21 skills (Golden Format)
├── 📁 commands/            # 7 commands
├── 📁 hooks/
├── 📄 README.md
├── 📄 CHANGELOG.md
└── 📄 LICENSE
```

</details>

---

## 📅 Metadata

| Field | Value |
|-------|-------|
| **Version** | 2.0.0 |
| **Last Updated** | 2025-12-29 |
| **Status** | Production Ready |
| **SASMP** | v1.3.0 |
| **Agents** | 6 |
| **Skills** | 21 |
| **Commands** | 7 |

---

## 🤝 Contributing

Contributions are welcome! Please read our [Contributing Guide](CONTRIBUTING.md).

1. Fork the repository
2. Create your feature branch
3. Follow the Golden Format for new skills
4. Submit a pull request

---

## ⚠️ Security

> **Important:** This repository contains third-party code and dependencies.
>
> - ✅ Always review code before using in production
> - ✅ Check dependencies for known vulnerabilities
> - ✅ Follow security best practices
> - ✅ Report security issues privately via [Issues](../../issues)

---

## 📝 License

Copyright © 2025 **Dr. Umit Kacar** & **Muhsin Elcicek**

Custom License - See [LICENSE](LICENSE) for details.

---

## 👥 Contributors

<table>
<tr>
<td align="center">
<strong>Dr. Umit Kacar</strong><br/>
Senior AI Researcher & Engineer
</td>
<td align="center">
<strong>Muhsin Elcicek</strong><br/>
Senior Software Architect
</td>
</tr>
</table>

---

<div align="center">

**Made with ❤️ for the Claude Code Community**

[![GitHub](https://img.shields.io/badge/GitHub-pluginagentmarketplace-black?style=for-the-badge&logo=github)](https://github.com/pluginagentmarketplace)

</div>
