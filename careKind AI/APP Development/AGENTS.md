# Application development scope

This directory holds implementation, architecture and technical validation. Shared product requirements live in `../docs/PRD_careKind_AI.md`.

- Read relevant PRD requirements and `../rules/coding.md`; follow `../workflows/product-delivery.md`.
- For product design or changed data/clinical behavior, apply `../rules/product-and-legal.md` and read relevant local legal sources before defining the change.
- Preserve tenant/identity boundaries, source traceability, draft/human signature separation and explicit failure states.
- When real feature modules are created or refactored, add scoped AGENTS.md, CLAUDE.md importing it, and README.md under `../rules/documentation.md`.
- No application stack, build or test commands are configured yet. Inspect the actual implementation before choosing commands; do not invent them.
