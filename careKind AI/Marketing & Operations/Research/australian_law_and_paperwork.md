# Australian aged-care law and paperwork research

**Prepared:** 4 October 2026 (Australia/Sydney)  
**For:** careKind AI, an Australian startup building AI-assisted nursing documentation for aged-care settings  
**Scope:** Official-source research for product discovery and reference. This is not legal advice. Check the current legislation, provider category, service model, jurisdiction, contract, and product claims before launch.

## Executive summary

- The Commonwealth's **Aged Care Act 2024 (Cth)** and **Aged Care Rules 2025** commenced on **1 November 2025**. They regulate government-funded aged care across Australia. The strengthened Aged Care Quality Standards also took effect on that date. The standards apply according to registered service category; the Commission says the strengthened standards/audit process do not apply to categories 1–3 in the same way as categories 4–6. Always check the applicable standard and service type.
- A provider's records have to support person-centred assessment and care planning, continuity, clinical governance, safe medicines, incident and complaint management, quality indicators, access by the older person and authorised supporters, and auditability. For a registered provider, multiple classes of records—including clinical records/progress notes, care and services plans, incident records, worker records and QI data—have **7-year retention requirements** under the Rules. That is a provider duty; a SaaS vendor should contractually support retention, export, access, correction, audit trail and secure deletion without becoming the provider's record custodian by accident.
- A software vendor handling identifiable health records is likely to handle **sensitive health information**. Private-sector health service providers are covered by the Commonwealth Privacy Act nationwide; the software company may also be an APP entity depending on its operations and turnover, and its customer remains accountable for its own handling. NSW, Victoria and ACT have additional private-sector health-information rules. State public-sector privacy/records laws affect government providers and public hospitals.
- Whether a note-taking/voice product is a TGA-regulated medical device depends on its **intended purpose and claims**. Pure transcription/record-management may fall outside the medical-device definition; clinical interpretation, monitoring, diagnosis, risk prediction, or recommendations may bring it into scope. Current TGA guidance says AI-enabled clinical decision support will not meet the conditional CDSS exemption criteria. Obtain a documented TGA classification assessment before making clinical claims or supplying decision-support functionality.
- State and territory differences matter most for **health privacy (NSW/VIC/ACT), consent and substitute decision-making (all jurisdictions), restrictive practices (state law expressly interacts with Commonwealth rules), public records, medicines/poisons, mandatory reporting, surveillance/audio capture and workers checks**. The Commonwealth aged-care framework is national, but workflows cannot assume that a family member automatically has authority to consent.

## 1. Commonwealth aged-care framework and documentation implications

### Main current framework

| Instrument / guidance | Start / current status | Relevance to careKind AI |
|---|---|---|
| [Aged Care Act 2024 (Cth)](https://www.legislation.gov.au/C2024A00104/latest/text) | Commenced 1 Nov 2025 | Rights-based framework for funded aged care; duties attach primarily to registered providers and others specified in the Act. The Act includes provider registration conditions, records/privacy, access, incidents, complaints, restrictive practices, and enforcement provisions. |
| [Aged Care Rules 2025](https://www.legislation.gov.au/F2025L01173/latest/text) | In force from 1 Nov 2025; check the current compilation before relying on a section | Detailed operational requirements including record types and retention, care and services plans, worker records, incidents, QI reporting, information access and restrictive-practice safeguards. The current official compilation should be used; section numbering and requirements can be amended. |
| [Strengthened Aged Care Quality Standards](https://www.agedcarequality.gov.au/providers/quality-standards/strengthened-aged-care-quality-standards) | Effective 1 Nov 2025 | Seven standards: individual; organisation; care and services; environment; clinical care; food and nutrition; residential community. Scope depends on registration/service category. |
| [Aged Care Code of Conduct](https://www.agedcarequality.gov.au/providers/standards/code-conduct-aged-care) | Began 1 Dec 2022; carried into new Act | Applies to providers, governing persons and aged-care workers. Generated notes must not obscure who observed, decided, checked, signed or acted. |
| [Serious Incident Response Scheme (SIRS)](https://www.agedcarequality.gov.au/providers/serious-incident-response-scheme) | Current; reporting obligations continue under the new Act | Providers need an incident management system and Commission notifications. Priority 1: within 24 hours after awareness; Priority 2: within 30 days. Criminal conduct may also need police notification. System should capture incident facts, awareness time, priority/reason, immediate protection, escalation, actions, investigation, outcome and report status. |
| [National Aged Care Quality Indicator Program](https://www.health.gov.au/our-work/qi-program/about) | Rules under the 2024 Act; current program reporting | Residential aged-care providers report 14 indicators quarterly. Product data structures should preserve source observations/assessments and support validated export; an AI-generated summary cannot substitute for the required measurement method. Support at Home QI settings may differ. |

### Required recordkeeping: direct statutory baseline

The Rules prescribe provider records and commonly require retention for **7 years from the date made/received**. Examples include:

- Records for continuity of funded services: assessment/classification records not transmitted electronically, service agreement, care and services plan, relevant assessments/measurements and related items (Rules s 154-1000; verify current text and scope).
- Records enabling subsidy claims to be verified, expressly including service agreements, **medical records, progress notes and other clinical records**, invoices and worker attendance (s 154-1205).
- Incident details recorded in the provider's incident management system (s 154-150), complaint/feedback records and quality-indicator reports/collection records (relevant Part 7 subdivisions).
- Worker and responsible-person screening/qualification records (ss 154-900–154-915); retention period runs from the later of creation or latest update for specified files.
- Compliance evidence and records that support a proper assessment of the provider's compliance.

This list is illustrative, not exhaustive. The Rules also require providers to provide or explain specified information and facilitate individuals' access to records. Other Commonwealth/state laws, professional standards, funding contracts, litigation holds and clinical context can require longer or different retention. A product must allow configurable retention and legal holds; do not hard-code a universal deletion date.

### Documentation workflows indicated by the strengthened Standards

Commission guidance is not a prescriptive form set, but shows useful workflow requirements:

1. **Person-centred assessment and plan:** record the older person's needs, goals, preferences, risks, agreed options, supporter involvement and decision authority. Update when needs change and review the plan with the person. See [Comprehensive care](https://www.agedcarequality.gov.au/strengthened-quality-standards/clinical-care/comprehensive-care) (Outcome 5.4) and [Care and services](https://www.agedcarequality.gov.au/strengthened-quality-standards/care-and-services).
2. **Clinical record and handover:** make clinical assessments, risks, treatment options as agreed, care delivered, response, escalation and transition information accessible to authorised workers at the right time. The provider remains responsible for qualified assessment and clinical decisions. See [Clinical care](https://www.agedcarequality.gov.au/strengthened-quality-standards/clinical-care).
3. **Information governance:** maintain accurate, current, complete, understandable and confidential information; manage consent for collection/use/storage/disclosure and record withdrawal; give people/supporters/authorised clinicians appropriate access; control roles and access. See [Outcome 2.7 Information management](https://www.agedcarequality.gov.au/strengthened-quality-standards/organisation/information-management).
4. **Clinical governance:** identify the author/reviewer, use appropriate national terminology and health identifiers where applicable, log access and changes, support coordination of care, and provide security and access controls. See [Outcome 5.1 Clinical governance](https://www.agedcarequality.gov.au/strengthened-quality-standards/clinical-care/clinical-governance).
5. **Incidents and complaints:** preserve the original account, timestamps, reporter, subsequent edits, clinical escalation, investigation, actions, notifications and review. AI must not silently change a factual record or classify a SIRS event without accountable human review.
6. **Restrictive practices:** residential provider must treat them as last resort, use least restrictive/shortest duration, obtain valid informed consent, have and implement a Behaviour Support Plan (BSP), monitor/review and meet state/territory law. Record alternatives tried, assessment, rationale, decision-maker authority, practice, duration, consent, monitoring, review and notifications. See [Commonwealth restrictive-practices guidance](https://www.health.gov.au/topics/aged-care/providing-aged-care-services/training-and-guidance/restrictive-practices-in-aged-care-a-last-resort).

### Documentation is not the same as the AI vendor's legal duty

The aged-care provider is generally the regulated party for care delivery and recordkeeping. careKind AI can separately have Privacy Act, contract, consumer, cybersecurity, TGA, employment, and potentially health-service obligations depending on what it does and represents. A business associate/vendor contract should clearly define controller-like decisions, permitted processing, sub-processors, model-training prohibition/permissions, Australian/overseas hosting, breach response, access/correction, export, retention/deletion, audit and service continuity. Do not assume the provider's consent to care automatically authorises ambient audio recording, model training, or unrelated secondary use.

## 2. Privacy, consent, AI and audio capture

### Federal privacy baseline

- The [Privacy Act 1988 (Cth)](https://www.legislation.gov.au/C2004A03712/latest/text) and Australian Privacy Principles (APPs) regulate APP entities' collection, use, disclosure, security and access/correction for personal information. Health information is sensitive information. Aged-care and nursing providers are generally health service providers and covered even if small businesses; the exact status of a separate software startup depends on its activities and statutory coverage.
- Useful OAIC material: [Health privacy guide](https://www.oaic.gov.au/privacy/privacy-guidance-for-organisations-and-government-agencies/health-service-providers/guide-to-health-privacy), [APP 8 cross-border disclosure](https://www.oaic.gov.au/privacy/australian-privacy-principles/australian-privacy-principles-guidelines/chapter-8-app-8-cross-border-disclosure-of-personal-information) and [Notifiable Data Breaches scheme](https://www.oaic.gov.au/privacy/notifiable-data-breaches).
- Collect only what is reasonably necessary, give a collection notice, use/disclose for the primary purpose or a permitted exception, secure data, destroy/de-identify when no longer needed unless retention is legally required, and support access/correction. Assess every LLM/transcription subcontractor, retention setting, telemetry/logging and training use. APP 8 may make the Australian entity accountable for overseas recipients; “Australian region” hosting alone does not answer all access/subprocessor questions.
- My Health Record is separately governed by the [My Health Records Act 2012](https://www.legislation.gov.au/C2012A00063/latest/text) and Rules. Do not imply integration or access unless the organisation is an eligible participant and the product meets applicable registration, identity, security and access obligations.

### Consent and recordings

Consent for care, consent to share clinical information, consent to use a restrictive practice, and consent/authority for voice recording are distinct. A person may have capacity for one decision but not another; a relative is not automatically the legal substitute decision-maker. Rules for appointment/recognition differ by jurisdiction. Record who decided, capacity/authority basis, what was explained, purpose, scope, date/time, limitations, withdrawal and the people notified.

Ambient voice capture can trigger state/territory listening-device or surveillance-device laws, workplace surveillance rules, privacy obligations and employment/industrial requirements. The application of these laws depends on location, who is speaking/recording, the setting, notice/consent, and exceptions. Before product pilots, obtain jurisdiction-specific advice. Safer product defaults include explicit session start/stop, visible recording indicator, no background capture, ability to pause, no retention of raw audio by default, separate opt-in for audio retention/training, a clear notice for residents/visitors/workers, and accessible ways to decline without disrupting care. These are design mitigations, not a legal conclusion.

## 3. State and territory comparison matrix

The Commonwealth Act and Rules are national for funded aged care. The matrix highlights overlays likely to affect the product; it is not an exhaustive statute inventory. Private aged-care operators are usually governed by Commonwealth privacy, while public-sector operators also have state/territory public-record and information laws. Check laws where the consumer and service are located, not only the vendor's headquarters.

| Jurisdiction | Private-provider health privacy overlay (OAIC summary) | Guardianship / substitute decision-making anchor | Practical product implication |
|---|---|---|---|
| NSW | **Yes:** Health Records and Information Privacy Act 2002 (NSW) and Health Privacy Principles apply to private health service providers, alongside federal law. | Guardianship Act 1987 (NSW); consent authority can depend on the specific decision and appointment. | Maintain NSW-specific privacy notices/access handling. Do not treat “person responsible” or next of kin as blanket authority for restrictive practices. Audio/workplace surveillance and public records need separate NSW review. |
| Victoria | **Yes:** Health Records Act 2001 (Vic), Health Privacy Principles; applies to private and public records of health/aged-care services. | Guardianship and Administration Act 2019 (Vic); Medical Treatment Planning and Decisions Act 2016; Aged Care Restrictive Practices Substitute Decision-maker Act 2024 (Vic) may be relevant. | Provide Victorian HPP handling/access path; specific aged-care restrictive-practice substitute decision-maker pathway. Verify commencement/current amendments and delegated authority. |
| Queensland | **No general private-sector health privacy statute identified by OAIC;** Privacy Act applies to private health providers. State privacy law covers public sector. | Guardianship and Administration Act 2000 (Qld); Powers of Attorney Act 1998 (Qld); QCAT/Public Guardian role for some restrictive-practice decisions. | Public providers have state privacy overlay. QLD Public Guardian may require a specific QCAT-authorised function for restrictive practices; do not infer ordinary guardianship authority. |
| Western Australia | **No specific general privacy statute identified by OAIC**; Privacy Act applies to private health providers; state public-sector records/privacy settings still matter. | Guardianship and Administration Act 1990 (WA), including state-specific authority pathways. | Map authority per decision and document it; check WA listening-device, medicines/poisons, mandatory-reporting and public-record requirements. |
| South Australia | **No specific general privacy statute identified by OAIC**; Privacy Act applies to private health providers; public-sector obligations apply to SA government bodies. | Guardianship and Administration Act 1993 (SA); Advance Care Directives Act 2013 (SA). | SA has distinct advance care directive and restrictive-practice approval considerations; design explicit authority/document fields. |
| Tasmania | **No private-sector health privacy overlay identified by OAIC;** Information Privacy Act 2009 (Tas) covers public sector. | Guardianship and Administration Act 1995 (Tas); state advance care directive and consent rules require local checking. | Federal APP baseline for private provider/vendor, state privacy for public sector. Confirm any recent commencement/reform affecting guardianship and substitute decision-making before rollout. |
| ACT | **Yes:** Health Records (Privacy and Access) Act 1997 (ACT) / Territory Privacy Principles; ACT Information Privacy Act 2014 also applies to public sector. | Guardianship and Management of Property Act 1991 (ACT); Powers of Attorney Act 2006 (ACT); advance consent instruments may apply. | Dual federal + territory requirements for private health records; assess public record laws and local consent/recording requirements. |
| Northern Territory | **No private-sector overlay identified by OAIC;** Information Act 2002 (NT) privacy provisions apply to public sector. | Guardianship of Adults Act 2016 (NT); Advance Personal Planning Act 2013 (NT). | Public provider overlay; validate adult guardianship/advance personal plan status and local surveillance/consent rules. |

**Privacy comparison source:** [OAIC state and territory privacy legislation](https://www.oaic.gov.au/privacy/privacy-legislation/state-and-territory-privacy-legislation) (updated 1 Dec 2025).  
**State-specific aged-care overlay sources:** [Commission legislation index](https://www.agedcarequality.gov.au/providers/standards/legislation) and [Department restrictive-practices overview](https://www.health.gov.au/topics/aged-care/providing-aged-care-services/training-and-guidance/restrictive-practices-in-aged-care-a-last-resort). These list jurisdictional guardianship and related laws. They do not replace checking current consolidated legislation.

### What differs in restrictive-practice consent

The Commonwealth Rules prescribe a national safeguards baseline, but the Aged Care Rules require compliance with the law in the State/Territory where the practice is used. The 2025 Rules contain an authority hierarchy for cases where local law has no appointment route, but should not be treated as a universal family-consent hierarchy. The official [Rules compilation](https://www.legislation.gov.au/F2025L01173/latest/text) includes a jurisdiction-by-jurisdiction table of medical-treatment authorities; verify the current section/schedule when implementing a workflow. The official [Consent for restrictive practices FAQ](https://www.health.gov.au/resources/publications/consent-for-restrictive-practices-frequently-asked-questions) (9 Feb 2026) is useful operational reading.

## 4. TGA: AI documentation and clinical decision support

TGA status turns on manufacturer **intended purpose**, including instructions, interface, marketing and claims—not just the label “administrative tool.” Official [TGA software-device guidance](https://www.tga.gov.au/resources/guidance/understanding-how-we-regulate-software-based-medical-devices) (published 24 Feb 2026) says software/AI is regulated if it meets the medical-device definition; it includes AI and cloud SaaS. [CDSS guidance](https://www.tga.gov.au/resources/guidance/understanding-clinical-decision-support-system-software-regulation), updated 29 Jan 2026, says certain low-risk CDSS exemptions are conditional, but AI-enabled CDSS will not meet the exemption criteria described there. A medical device not excluded/exempt generally needs ARTG inclusion before supply.

For careKind AI, assess separately each feature and release:

- **Lower-risk hypothesis (not a ruling):** faithful speech-to-text, formatting, summarising what a nurse said, organising a note, and routing it for clinician review, without diagnosing, predicting, monitoring disease, proposing clinical actions, or changing the record autonomously. Intended-use claims and errors still matter; not automatically outside TGA.
- **Higher TGA-risk functions:** detect deterioration, calculate/interpret clinical scores, infer diagnoses, recommend treatment/escalation, generate alerts from clinical data, or analyse medical images/signals. These can be medical-device functions; determine classification, evidence, quality system and ARTG path before supply.
- If an AI function is intended to support clinical decisions, the TGA guidance states AI-enabled CDSS does not meet its specified exemption criteria. Obtain a specialist regulatory opinion and document the classification rationale before pilot claims.
- Keep a human accountable for review, edits, signature and escalation. Preserve what was spoken/entered, AI output, edits, author, reviewer, time, model/version, prompt/template version and final signed record. Have a correction workflow; never represent a draft as a nurse's signed observation.

## 5. Official reference templates and downloadable material

These are official working references, not universal mandatory care forms. Tailor them to service category, provider policy, the new Act/Rules and local law. The government may replace files; retain the date/version and re-check links before adoption.

| Reference | What it is useful for | Official file/source |
|---|---|---|
| QI Program data recording template (published 4 Aug 2026) | Current residential quality-indicator collection and reporting structure; single home workbook. | [Download page](https://www.health.gov.au/resources/publications/qi-program-data-recording-templates?language=en) (Excel, 2 MB) |
| National Aged Care QI Program Manual, Part A (published 29 Sep 2026) | Definitions, measurement and submission methods. | [Download page](https://www.health.gov.au/resources/publications/national-aged-care-quality-indicator-program-manual-part-a-0) (PDF and Word) |
| National Aged Care QI Program Manual, Part B (Oct 2025) | Clinical practice guidance and examples, including pressure injury/falls documentation. | [PDF](https://www.health.gov.au/sites/default/files/2025-10/national-aged-care-quality-indicator-program-manual-part-b.pdf) |
| GP in Aged Care Incentive care-plan contribution template | Six-page example for GP contributions/review for residential aged-care residents; useful to compare common structured fields, not a whole-provider nursing template. | [Download page](https://www.health.gov.au/resources/publications/care-plan-contribution-template?language=en) (PDF) |
| QI quick reference guides | Examples of data capture for pressure injuries, falls and other QIs. | [Official collection](https://www.health.gov.au/resources/collections/qi-program-quick-reference-guides?language=en) |
| Consent for restrictive practices FAQ (9 Feb 2026) | Current consent model and operational questions. | [Download page](https://www.health.gov.au/resources/publications/consent-for-restrictive-practices-frequently-asked-questions) (PDF/Word) |
| NSW private health-service retention/storage guide | Local rules and practice for NSW private providers. | [IPC NSW resource page](https://www.ipc.nsw.gov.au/privacy/private-nsw-health-service-providers) (includes guide and access checklist) |
| Queensland Public Guardian restrictive-practice request form | Only relevant where seeking a decision for a client of the QLD Public Guardian; not a general consent form. | [Official form page](https://www.publicguardian.qld.gov.au/understanding-guardianship/request-a-decision/restrictive-practices-aged-care-resident) |
| Commission strengthened Standards guidance tool | Provider-category and outcome-specific guidance; can print pages. | [Guidance tool](https://www.agedcarequality.gov.au/strengthened-quality-standards) |

**Downloaded official files:** four current/source-version references have been saved in [`References`](References/README.md): the QI recording workbook (August 2026), QI Manual Part A (September 2026), GP care-plan contribution template (August 2024), and restrictive-practices consent FAQ (February 2026). Their use and limitations are described in the folder README. Re-check the government source pages for replacements before use. No third-party materials have been copied.

## 6. Suggested product requirements to validate with counsel and provider users

1. Support configuration by provider category, delivery setting (residential/home/community), state/territory and record type.
2. Keep draft, reviewed and signed states distinct; require identity, role, timestamp, amendment history and reason for correction.
3. Preserve provenance: dictated text, transcript if retained, generated note, edits, final approved note, model/version and template version. Default to least audio retention.
4. Build explicit consent/authority capture: person, decision, capacity/authority basis, appointed instrument, jurisdiction, scope, date/time, who witnessed/explained, expiry/review, and withdrawal.
5. Make records exportable and readable for the provider/consumer; include access logs, break-glass events, retention holds, deletion certificates and data portability.
6. Separate operational notes from SIRS reports and regulated QI measures. Provide prompts/checklists with human confirmation, not autonomous incident priority or clinical determination.
7. Assess hosting, LLM provider and all subprocessors for APPs, APP 8, security, retention/training and breach notification. Do not put identifiable care data into consumer AI services.
8. Run a documented intended-purpose/TGA classification review for each feature and marketing claim; repeat after material functionality/model updates.
9. Test templates and workflow with nurses and older people, including cognitive/sensory/communication access needs, cultural safety, Aboriginal and Torres Strait Islander data governance, and refusal/recording alternatives.

## 7. Primary official sources

- [Aged Care Act 2024 (latest compilation)](https://www.legislation.gov.au/C2024A00104/latest/text)
- [Aged Care Rules 2025 (latest compilation)](https://www.legislation.gov.au/F2025L01173/latest/text)
- [New Act overview and commencement](https://www.health.gov.au/our-work/aged-care-act/about?language=en)
- [Commission strengthened Standards and guidance](https://www.agedcarequality.gov.au/providers/quality-standards/strengthened-aged-care-quality-standards)
- [Rules of records retention and provider obligations](https://www.legislation.gov.au/F2025L01173/latest/text) (Part 7, Division 1; in particular ss 154-900 onward)
- [OAIC state and territory privacy laws](https://www.oaic.gov.au/privacy/privacy-legislation/state-and-territory-privacy-legislation)
- [OAIC health privacy guide](https://www.oaic.gov.au/privacy/privacy-guidance-for-organisations-and-government-agencies/health-service-providers/guide-to-health-privacy)
- [TGA software-based medical-device regulation](https://www.tga.gov.au/resources/guidance/understanding-how-we-regulate-software-based-medical-devices)
- [TGA CDSS regulation](https://www.tga.gov.au/resources/guidance/understanding-clinical-decision-support-system-software-regulation)

**Review reminder:** laws and ministerial rules change. Before deployment, have Australian aged-care/privacy/TGA counsel review intended use, customer agreement, audio workflows, consent/authority, security/hosting, retention, data flows and provider-specific requirements. This memo is a research starting point, not advice.
