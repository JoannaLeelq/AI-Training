# AI and Clinical Safety Governance

## Draft intended use — review before external use

careKind AI assists authorised aged care workers to prepare draft care records from lawfully captured shift audio and worker-provided information. It can process an eight-hour recording session, organise supported facts by resident and maintain a source-linked event timeline. Capture windows, resident identity evidence and unresolved attribution must be explicit; uncertain content cannot become a signed resident record. It helps structure and edit documentation. It does not independently assess a resident, diagnose, triage urgency, recommend treatment, determine medication, or replace the provider's formal record system or professional judgement.

This is a working scope, not a determination that the product is outside TGA regulation. Actual functionality, intended purpose and marketing claims require qualified Australian regulatory review.

## Human review requirements

1. Clearly label output as an AI-assisted draft.
2. Show source input alongside the draft where practical.
3. Require authorised user verification of resident identity, facts, time, negations, quantities, observations, medication references and actions.
4. Require an explicit human approval before export or submission. Never auto-sign, auto-submit or silently overwrite a record.
5. Preserve version history and identify the reviewer/submitter.
6. Make edit, discard, retry and escalation easy. Unclear input must be surfaced, not guessed.
7. Never invent normal findings, consent, actions or negative statements.

## Hazards to evaluate

Wrong-resident attribution or tenant leakage; invented or omitted facts/actions; errors in negation, names, dates, units or medication; missed deterioration, falls, pain, wounds, food/fluid, medication or safeguarding details; accents, speech impairment, dementia, multilingual speech, noise and overlapping speakers; automation bias, fatigue and poor accessibility; recording authority and bystander capture; outage, duplicate/lost notes, wrong-chart export and loss of audit trail.

## Assurance lifecycle

- Trace user need → hazard → control → verification evidence → release criterion.
- Use synthetic or appropriately authorised/de-identified data for development and early testing.
- Validate with representative nurses and real workflows; measure critical errors, omissions/inventions, correction time and subgroup performance, not just average transcription quality.
- Set acceptance and stop thresholds with the clinical safety lead before pilots.
- Test uncertainty, adverse edge cases and whether the system fabricates missing details.
- Monitor corrections, near misses, complaints, vendor/model drift and subgroup disparities after release.
- Version models, prompts, templates and rules; require impact review and regression evidence before changes.
- Maintain a visible manual fallback and unsafe-output reporting route.

## Claims and stop rules

Keep an approved claims register. Claims about clinical outcomes, error reduction, compliance, quantified time savings or TGA status need substantiation and legal/regulatory review. Pause a feature or pilot after wrong-resident output, credible serious-harm risk, systematic unsafe omission/invention, uncontrolled disclosure, unknown data flow, loss of auditability, or inability to review and correct.

References: [TGA CDSS regulation](https://www.tga.gov.au/resources/guidance/understanding-clinical-decision-support-system-software-regulation), [TGA software medical devices](https://www.tga.gov.au/resources/health-professional-information-and-resources/software-based-medical-devices-health-professionals), [Aged Care Quality Standards](https://www.agedcarequality.gov.au/providers/quality-standards/strengthened-aged-care-quality-standards), [OAIC AI privacy guidance](https://www.oaic.gov.au/privacy/privacy-guidance-for-organisations-and-government-agencies/guidance-on-privacy-and-the-use-of-commercially-available-ai-products).
