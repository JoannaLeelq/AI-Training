# Company rules setup

Date: 4 October 2026 (Australia/Sydney)  
Executor: Codex  
Status: complete — documentation and agent/workflow routing

Created `rules/` with company, operations, product/legal-reference and SOLID/DRY/KISS coding standards plus a legal-reference mapping template. Connected rules to the shared AGENTS.md, product skill, product/operations workflows and project README. Existing CLAUDE.md imports AGENTS.md, so both tool entrypoints receive the same rule routing.

Added Joanna's indentation preference: real tabs, width/indent size 4, with project `.editorconfig` and explicit YAML/Markdown formatting exceptions. Shared docs README also points product/PRD authors to the local legal-reference requirements.

Added Joanna's 15 engineering rules as CR-01–CR-15, an initially empty any/Any exception whitelist, `.env` Git ignore patterns and workflow checks. Boundary validation remains distinct from access/state invariants; synthetic test fixtures cannot masquerade as real data; synchronous interactive targets and asynchronous shift processing have separate performance criteria. No actual secrets or any exceptions were created.

Rules distinguish mandatory local review from actual legal approval. Downloaded originals remain unchanged, and raw feedback was not read or edited. Checked new document links and required routing references. No app code, legal determinations, actual tool-session enforcement or production configuration was changed.
