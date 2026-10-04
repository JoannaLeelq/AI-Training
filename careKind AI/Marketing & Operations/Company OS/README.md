# careKind AI — Company OS

**Starter version 0.1 | Australia | 4 October 2026**

This operating system is for an early-stage Australian startup building AI-assisted paperwork for aged care nurses. It is an operational foundation, not legal advice or a compliance certification. Obtain Australian legal, privacy, aged-care and TGA advice for the actual product and customer context.

## Starting assumptions

- careKind AI is a B2B software supplier; the aged care provider remains responsible for care delivery and its formal clinical records.
- The product processes authorised shift recordings (for example, eight hours) and worker inputs to organise facts by resident and produce editable documentation drafts. Uncertain attribution remains pending human confirmation; capture scope requires explicit privacy/recording review.
- A nurse must review and approve a draft before it is exported or entered into a formal record.
- The product does not independently diagnose, triage, recommend treatment or manage medication.
- Real resident data stays out of pilots until the release gate is complete.

If any assumption changes, review the product safety, privacy, contract and TGA assessments before release.

## How to use this OS

1. Confirm company roles and decision rights in [Company Charter](01_company_charter.md).
2. Assign owners and evidence in the [Australian Compliance Register](02_compliance_register.md).
3. Complete [Privacy and Data Security](03_privacy_data_security.md) before real-data processing.
4. Apply [AI and Clinical Safety Governance](04_ai_clinical_safety.md) to product design, testing and release.
5. Use the [Incident Response](05_incident_response.md) procedure for safety, privacy or security events.
6. Require every applicable item in the [Pilot and Release Gate](06_pilot_release_gate.md) before a real-data pilot.
7. Track unresolved choices in [Decisions and Open Items](07_decisions_and_open_items.md).

## Current hard controls

- AI-generated content is a draft and requires an authorised human review and approval.
- No identifiable resident data in public AI tools or unapproved vendors.
- No customer data used to train a shared model by default.
- No silent overwrite, auto-signature or autonomous clinical action.
- No public claim of aged care provider status, legal compliance or TGA approval unless verified.

## Official Australian references

- [OAIC: Health service providers](https://www.oaic.gov.au/privacy/your-privacy-rights/health-information/what-is-a-health-service-provider)
- [OAIC: Privacy and commercially available AI](https://www.oaic.gov.au/privacy/privacy-guidance-for-organisations-and-government-agencies/guidance-on-privacy-and-the-use-of-commercially-available-ai-products)
- [Strengthened Aged Care Quality Standards](https://www.agedcarequality.gov.au/providers/quality-standards/strengthened-aged-care-quality-standards)
- [TGA: Clinical decision support software regulation](https://www.tga.gov.au/resources/guidance/understanding-clinical-decision-support-system-software-regulation)
- [OAIC: Notifiable Data Breaches](https://www.oaic.gov.au/privacy/notifiable-data-breaches)
- [ACSC: Small business cyber security guide](https://www.cyber.gov.au/business-government/small-business-cyber-security/small-business-hub/small-business-cyber-security-guide)

OS owner: Founder/CEO (to confirm). Review open items monthly, core policies quarterly, and relevant controls whenever laws, product scope, data flows or vendors materially change.
