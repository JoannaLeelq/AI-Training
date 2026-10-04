# Shared skills scope

This directory is the shared skill source used by Claude/Codex native routing adapters.

- Each skill has SKILL.md with a precise name/description and a relevant workflow reference.
- Keep substantial procedures in `../workflows/`, common rules in `../rules/`, and product definitions in `../docs/`; avoid duplicating those bodies in skills.
- Preserve narrow selection criteria, raw-feedback restrictions and actual user authorisation boundaries.
- Validate manifest names and references when editing. Native adapters under `.agents/skills/` and `.claude/skills/` at the company root should remain equivalent routers.
