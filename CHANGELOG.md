# Release log

Significant changes to Ambitious Prompt are recorded here. Dates use Singapore time.

Versions follow `MAJOR.MINOR.PATCH`: incompatible workflow changes increment MAJOR, compatible capabilities increment MINOR, and fixes increment PATCH. Meaningful releases include what changed, why it matters, and any action existing users need to take. Small documentation corrections may be grouped into the next release.

## Unreleased

No changes recorded yet.

## 1.0.2 — 2026-10-27

### Documentation

- Reworked the public README to explain the problems the skill addresses, its workflow, and observable expectations.
- Added an illustrative before-and-after prompt, examples across domains, guidance on when to use the skill, and practical tradeoffs.
- Made versioned ZIP installation easier to find and retained source attribution, LinkedIn creator links, and the corrected professional titles.
- Clarified that the Karpathy-inspired guidelines are a community adaptation, not an official Karpathy skill.

### Existing users

The skill's execution and approval behavior are unchanged. Updating is optional; install v1.0.2 for the revised documentation.

## 1.0.1 — 2026-10-27

### Changed

- Removed personal website references from the creator profile, documentation, and skill.
- Creator and permission-inquiry links now use Joven’s LinkedIn profile.
- Recorded the creator-link preference in repository maintenance instructions.

### Existing users

Update your Git checkout or replace the uploaded skill with the v1.0.1 ZIP to receive the corrected profile and links. Prompt rewriting and approval behavior are unchanged.

## 1.0.0 — 2026-10-27

### Added

- Domain-informed prompt rewriting with research proportional to the request, explicit assumptions, and model-capability fallbacks.
- Calibrated speed, altitude, depth, and range, using Felix Rieseberg’s article as a design reference.
- Four Karpathy-inspired disciplines: think before acting, simplicity first, surgical changes, and goal-driven execution.
- A prompt approval step before task execution, with continuation after approval.
- Installation and invocation guidance for Claude Code, Claude chat/Cowork, and Codex.
- Joven’s creator profile, LinkedIn byline, source credits, and authorship notice.
- Versioned release notes and a GitHub release workflow that attaches an installable skill ZIP.

### Corrected before the first release

- Creator titles: Chief Research & Revenue Officer of Cookiy Labs; President of Cookiy AI.
- Removed the mistakenly added MIT declaration. The creator notice identifies authorship and permission inquiries; no reuse license is granted.

### Existing users

This is the first versioned release. Users who installed an earlier unversioned copy should update their Git checkout or replace their uploaded skill with the ZIP attached to this release. Review NOTICE.md before reuse or redistribution.

[1.0.0]: https://github.com/jovenleewj-png/ambitious-prompt/releases/tag/v1.0.0

[1.0.1]: https://github.com/jovenleewj-png/ambitious-prompt/releases/tag/v1.0.1

[1.0.2]: https://github.com/jovenleewj-png/ambitious-prompt/releases/tag/v1.0.2
