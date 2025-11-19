# Architecture Documentation

## System Design

The Data Engineer Plugin is structured as a Claude Code plugin with the following architecture:

### Directory Structure

```
custom-plugin-data-engineer/
├── .claude-plugin/
│   └── plugin.json              # Main plugin manifest
├── agents/                       # 6 specialized learning agents
│   ├── 01-data-engineer.md      # PRIMARY: 40 weeks
│   ├── 02-backend-developer.md  # 36 weeks
│   ├── 03-devops-engineer.md    # 40 weeks
│   ├── 04-data-scientist.md     # 40 weeks
│   ├── 05-cloud-engineer.md     # 36 weeks
│   └── 06-ml-ai-engineer.md     # 40 weeks
├── commands/                     # 7 interactive commands
│   ├── start-learning.md
│   ├── choose-role.md
│   ├── skill-deep-dive.md
│   ├── project-ideas.md
│   ├── roadmap-status.md
│   ├── interview-prep.md
│   └── assessment.md
├── skills/                       # 21 core skills
│   ├── python-programming/
│   ├── sql-databases/
│   └── ... (19 more skills)
├── hooks/
│   └── hooks.json               # Automation hooks
├── README.md                     # Main documentation
├── CONTRIBUTING.md              # Contribution guidelines
├── ARCHITECTURE.md              # This file
└── LICENSE                       # MIT License
```

## Component Details

### 1. Plugin Manifest (.claude-plugin/plugin.json)

**Purpose:** Define plugin metadata, agents, skills, and commands

**Key Fields:**
- `name`: Plugin identifier
- `version`: Semantic versioning
- `displayName`: User-friendly name
- `description`: Brief overview
- `agents`: Array of agent definitions
- `skills`: Array of skill definitions with agent associations
- `commands`: Array of command definitions
- `keywords`: For discoverability
- `hooks`: Automation trigger hooks

**Agent Definition:**
```json
{
  "id": "data-engineer",
  "name": "Data Engineer",
  "description": "Master data pipelines..."
}
```

**Skill Definition:**
```json
{
  "id": "python-programming",
  "name": "Python Programming",
  "description": "Master Python...",
  "agents": ["data-engineer", "data-scientist", ...]
}
```

### 2. Agents

**Structure:** Each agent is a markdown file (2000+ words)

**YAML Frontmatter:**
```yaml
---
name: agent-id
displayName: Agent Name
description: Full description
expertise: [list of 10+ capabilities]
salaryRange:
  entry: "$XXK-$XXK"
  mid: "$XXK-$XXK"
  senior: "$XXK-$XXK"
  staff: "$XXK-$XXK+"
timelineMonths:
  complete_beginner: 12-18
  programming_background: 9-12
  full_time_accelerated: 6-9
---
```

**Content Structure:**
1. Executive Overview (100 words)
2. "Who Should Choose This Path" (50 words)
3. Complete Learning Path (8-10 phases, 2000+ words)
4. Technology Stack (30+ tools)
5. Career Progression (salary + career path)
6. Real-World Specializations (5-7 options)
7. Success Checklists (3 levels)
8. Next Steps (10 actionable items)

**Phases in Agent:**
- Phase 1: Foundations (4 weeks)
- Phase 2-6: Specialization (varies)
- Phase 7-8: Advanced/Production (varies)

### 3. Commands

**Structure:** Each command is a markdown file (200-400 words)

**Key Components:**
- `# Command Title` (H1)
- Usage section with examples
- What the command does
- Available options/parameters
- Output/response format
- Related commands
- FAQ section

**Command Types:**
- `/start-learning` - Interactive assessment
- `/choose-role [name]` - Role selection
- `/skill-deep-dive [skill]` - Skill mastery guide
- `/project-ideas [level]` - Project recommendations
- `/roadmap-status` - Progress tracking
- `/interview-prep [role]` - Interview preparation
- `/assessment [skill]` - Knowledge evaluation

### 4. Skills

**Structure:** Each skill has SKILL.md in its own directory

**Path:** `skills/{skill-name}/SKILL.md`

**YAML Frontmatter:**
```yaml
---
name: skill-id
description: Full description of skill
---
```

**Standard Sections:**
1. Quick Start (code example)
2. Key Concepts (3-5 bullet points)
3. Tools & Technologies (list)
4. Learning Path:
   - Foundations (weeks)
   - Intermediate (weeks)
   - Advanced (weeks)
   - Mastery (weeks)
5. Resources (official docs, courses, communities)
6. Best Practices (5-7 tips)
7. Next Steps (related skills)

### 5. Hooks Configuration

**File:** `hooks/hooks.json`

**7 Automation Hooks:**
1. `user-prompt-submit-hook` - Progress tracking
2. `skill-mastery-hook` - Completion recognition
3. `project-guidance-hook` - Project matching
4. `interview-readiness-hook` - Interview prep
5. `resource-recommendation-hook` - Smart recommendations
6. `knowledge-gap-hook` - Gap identification
7. `motivation-hook` - Milestone celebration

**Hook Structure:**
```json
{
  "id": "hook-id",
  "trigger": "trigger-event",
  "name": "Display Name",
  "description": "What it does",
  "enabled": true,
  "conditions": {},
  "actions": []
}
```

## Data Flow

### User Learning Journey

```
1. /start-learning
   ↓
2. Assessment + Personalized roadmap
   ↓
3. /choose-role (if needed)
   ↓
4. /skill-deep-dive for each technology
   ↓
5. /project-ideas for hands-on learning
   ↓
6. /roadmap-status to track progress
   ↓
7. /assessment to identify gaps
   ↓
8. /interview-prep when job hunting
```

### Component Interactions

- **Agents** define learning paths
- **Commands** implement user interactions
- **Skills** provide detailed technical content
- **Hooks** automate recommendations and tracking
- **Plugin.json** coordinates everything

## Content Standards

### Size Guidelines

| Component | Size | Count |
|-----------|------|-------|
| Agent | 2000-3000 words | 6 |
| Command | 200-400 words | 7 |
| Skill | 300-500 words | 21 |
| Total | 10,000+ words | 34 |

### Quality Metrics

✅ **Readability:** Clear, accessible language
✅ **Accuracy:** Technically correct information
✅ **Completeness:** All major topics covered
✅ **Freshness:** Annual updates for salaries/trends
✅ **Interoperability:** Components reference each other

## Technologies in Plugin

### Languages

- **Markdown:** All content
- **YAML:** Frontmatter metadata
- **JSON:** Configuration (plugin.json, hooks.json)

### External Tools Referenced

- **Development:** Python, SQL, Git, Docker, Kubernetes
- **Data:** Spark, Kafka, Airflow, Snowflake, BigQuery
- **ML/AI:** PyTorch, TensorFlow, LangChain
- **Cloud:** AWS, GCP, Azure
- **DevOps:** Terraform, Jenkins, GitHub Actions

## Scalability Considerations

### Growth Areas

1. **More Specializations:** Add new agent types
2. **Additional Skills:** Expand skill catalog
3. **Project Library:** Grow project ideas
4. **Localization:** Translate to other languages
5. **Community Content:** User-contributed projects

### Current Limits

- 6 agents (designed for expansion)
- 21 skills (comprehensive but not exhaustive)
- 7 commands (covers main workflows)
- JSON-based hooks (easily extensible)

## Security Considerations

✅ **No sensitive data storage** - Plugin doesn't store credentials
✅ **Educational content only** - No code execution
✅ **MIT Licensed** - Open source
✅ **Community reviewed** - Pull request based updates

## Maintenance

### Regular Updates Needed

- **Annually:** Update salary ranges
- **Bi-annually:** Review technology recommendations
- **Quarterly:** Fix broken links/resources
- **On-demand:** Typo fixes, clarifications

### Version Management

Uses semantic versioning: `MAJOR.MINOR.PATCH`

Example: `1.0.0` → `1.1.0` (new skill) → `1.1.1` (fix)

## Integration Points

### Claude Code Integration

- Agents trigger learning paths
- Commands provide interactive guidance
- Skills enable deep-dive learning
- Hooks automate recommendations

### External Resources

- Links to documentation
- Course recommendations
- GitHub project references
- Community resources

## Future Enhancements

Potential improvements:

1. **Video Integration:** Embedded learning videos
2. **Quiz System:** Knowledge verification
3. **Progress Tracking:** Persistent learning state
4. **Peer Learning:** Community features
5. **Certification:** Skill verification badges
6. **Practice Labs:** Interactive coding environments

---

## Questions?

For architectural questions, open an issue or discussion in the repository.

**Maintainers:** Data Engineer Plugin Team