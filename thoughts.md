# Thoughts
<!-- scored notes are added here over time -->

- [75] SETUP.md is the single-source installer — handles both INSTALL and UPDATE modes; RESSURECT=TRUE forces UPDATE path
- [70] SKILL.md is fetched remotely at session start; local copy is just a bootstrap pointer with FETCH and EXECUTE directive
- [65] Version check compares line 2 (timestamp) of install.version and skill.version against local copies to trigger auto-update
- [60] @brain stores user-editable YAML config (MAX_NOTES, MIN_RATING, FOLLOW, AVOID) — must be preserved across updates
- [55] SLUG derivation: last URL path segment → strip .git → lowercase → replace non-alphanum (except - _) with -
