# Changelog

All notable changes to the Data Engineer Development Assistant plugin will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [2.0.0] - 2025-12-28

### Added
- marketplace.json for plugin marketplace compatibility
- SASMP v1.3.0 compliance for all agents
- Template v2.1.0 README format (18 required sections)
- Verified Installation notice
- Available Skills table with `Skill("...")` invoke syntax
- Usage Examples section with before/after code
- Plugin Structure directory tree
- Technology Coverage table

### Changed
- plugin.json completely restructured to new format
  - Agents as paths (not objects)
  - Author as object format
  - Repository as string (not object)
  - License field updated
- README updated to template v2.1.0
- Quick Start commands fixed (`/plugin add marketplace` format)
- Version bump from 1.0.0 to 2.0.0

### Fixed
- E307: plugin.json repository format (object to string)
- E303: marketplace.name differs from plugin.name
- Quick Start commands now use proper `/plugin` format

---

## [1.0.0] - 2024-12-01

### Added
- Initial release
- 6 specialized agents (Data Engineer, Backend, DevOps, Data Scientist, Cloud, ML/AI)
- 21 core skills covering data engineering fundamentals
- 7 interactive commands
- 800+ hours of structured learning content
- Career guidance and interview preparation

---

## Version History Summary

| Version | Date | Description |
|---------|------|-------------|
| 2.0.0 | 2025-12-28 | SASMP v1.3.0 + Template v2.1.0 compliance |
| 1.0.0 | 2024-12-01 | Initial release |

---

## Contributors

- **Dr. Umit Kacar** - Senior AI Researcher & Engineer
- **Muhsin Elcicek** - Senior Software Architect

---

*Last Updated: 2025-12-28*
