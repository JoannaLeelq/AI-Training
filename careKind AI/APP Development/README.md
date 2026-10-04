# APP Development

Dedicated workspace for the careKind AI application.

Shared product definition: [careKind AI PRD](../docs/PRD_careKind_AI.md) — product strategy, authorised eight-hour shift recording, resident attribution, care-event timelines, nurse-reviewed documentation drafts and workflows. Product requirements are maintained in `docs/`; implementation and technical materials remain here.

## Suggested structure

- `../docs/` — shared product needs, PRD, workflows and acceptance criteria
- `architecture/` — system design, integrations and data flows
- `security/` — threat models, secure development and technical controls
- `quality/` — verification evidence, usability and clinical safety validation
- `releases/` — release notes, change approvals and rollback plans

## Product boundary at project start

The concept is a documentation assistant for aged care nurses that processes authorised shift recordings (for example, eight hours), organises information by resident and creates editable care-record drafts. Uncertain resident attribution must remain pending confirmation. A nurse must verify and approve any draft before it becomes a formal record. See the PRD for capture limits, source traceability and review requirements. Do not implement autonomous diagnosis, triage, treatment or medication recommendations without a fresh clinical safety and Australian TGA regulatory assessment.

Do not put identifiable resident data in development, demos or test systems unless the privacy, contract and security launch gates have been completed and approved.
