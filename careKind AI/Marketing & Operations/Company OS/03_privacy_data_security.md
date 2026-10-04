# Privacy and Data Security Baseline

Applies to founders, staff, contractors, systems and suppliers that can access careKind AI information. Customer agreements may require stronger controls. Do not accept identifiable resident data until the pilot/release gate is complete.

## Rules for information

- Collect only the information needed for a defined, approved workflow.
- Keep identity and working data separate where practical; enforce customer-tenant isolation and least privilege.
- Do not use real resident information in development, demonstrations, support cases or analytics unless specifically authorised, contractually permitted and access-controlled.
- Do not use customer data to train a shared or general model by default.
- Use only approved vendors and environments. Before offshore processing or support access, assess APP 8, customer terms, notice and security implications.
- Define retention and deletion separately for audio, transcripts, drafts, logs, exports and backups. Do not invent a blanket period: customer and state recordkeeping duties differ.
- Audit access, generation, edits, export, approval, deletion and administrative changes without putting unnecessary clinical details in logs.

## Before a real-data pilot

- Named privacy and security owners, current data-flow map and privacy impact assessment.
- Privacy notice and customer agreement explain purpose, AI processing, roles, recipients, locations, retention, rights and complaint channel.
- Approved model, transcription and cloud suppliers reviewed for training, retention, subprocessors, geography, incident terms, deletion, access controls and security evidence.
- Encryption in transit and at rest; MFA; role-based access; tenant isolation; secrets management; separate production and development.
- No production resident data in test environments.
- Monitor privileged access, unusual downloads and authentication anomalies; protect audit logs.
- Encrypted, access-controlled backups and documented restoration procedure.
- Supported software, security updates, vulnerability intake, secure development review and dependency tracking.
- Workforce confidentiality/privacy training and joiner/mover/leaver access process; periodic access review.
- Tested incident response, customer contacts and supplier escalation paths.
- Demonstrated data deletion and customer exit process, including supplier copies and backup expiry.

## Requests and complaints

Route access, correction, deletion, consent withdrawal and complaints to the privacy owner. Verify identity and authority, log the request and applicable deadline, coordinate with the customer, and preserve clinical-record history. Never silently rewrite a signed care record.

## Supplier register fields

For each AI, cloud, analytics, support and integration supplier record: purpose; data sent; training and retention terms; processing countries; subprocessors; security evidence; breach notice timeline; deletion method; continuity/exit plan; contract owner; review date.

References: [OAIC APP 11](https://www.oaic.gov.au/privacy/australian-privacy-principles/australian-privacy-principles-guidelines/chapter-11-app-11-security-of-personal-information), [OAIC AI privacy guidance](https://www.oaic.gov.au/privacy/privacy-guidance-for-organisations-and-government-agencies/guidance-on-privacy-and-the-use-of-commercially-available-ai-products), [ACSC small-business guide](https://www.cyber.gov.au/business-government/small-business-cyber-security/small-business-hub/small-business-cyber-security-guide).
