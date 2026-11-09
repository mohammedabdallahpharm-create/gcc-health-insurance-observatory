# Signal 003 — Formalisation of human oversight in AI-enabled healthcare and health-insurance operations

**Record ID:** UAE-HI-003  
**Market:** UAE — federal financial-sector guidance, with Abu Dhabi healthcare requirements recorded within their stated jurisdiction  
**Signal type:** Regulatory / AI governance  
**Primary sector:** Health insurance  
**Connected sector:** Healthcare  
**Primary regulatory lens:** CBUAE — licensed financial institutions, including insurance providers  
**Related regulatory lens:** Department of Health — Abu Dhabi  
**Status:** Regulatory direction verified; market-wide implementation and use-case-level human-oversight practice remain unverified
**Confidence:** High for the existence and stated scope of the cited regulatory instruments; low / not assessed for market-wide implementation
**Event date:** 11 February 2026 (CBUAE Guidance Note publication)  
**Observation date:** 9 November 2026  
**Related signal:** [Signal 004 — AI Document Intelligence in UAE Health Insurance Operations](./signal-004-ai-document-intelligence-uae-health-insurance.md) — separate institutional deployment record; no causal relationship is implied

## 1. External Signal Detection

On 11 February 2026, the Central Bank of the UAE published guidance on consumer protection and the responsible adoption and use of artificial intelligence and machine learning by Licensed Financial Institutions (LFIs). The guidance expressly includes insurance providers within its scope and sets out a risk-based approach to human oversight and consumer protection.

A particularly material point for health insurance is that the CBUAE's definition of a **high-impact decision** includes decisions that materially affect a customer's access to a financial service, giving an **insurance claim** as an example.

The signal is therefore not simply that AI is becoming relevant to insurance. It is that the UAE's federal financial-sector regulator has articulated specific expectations for how human authority, intervention, review and accountability should relate to AI/ML use by regulated institutions.

The healthcare connection is supported by Abu Dhabi Department of Health instruments: its 2018 AI policy expressly includes healthcare insurers and billing/insurance processing, while its 2025 Responsible AI Standard establishes human-oversight requirements for AI systems used by licensed healthcare entities in Abu Dhabi.

## 2. Signal Documentation & Evidence

### A. Federal financial-sector guidance — CBUAE

| Evidence | What it supports | Scope / grade |
|---|---|---|
| CBUAE, *Guidance Note on the Consumer Protection and Responsible Adoption and Use of AI and ML by Licensed Financial Institutions in the UAE*, published 11 February 2026 | Formal guidance for LFIs, expressly including insurance providers; identifies insurance claims as an example of a high-impact decision | UAE federal financial-sector regulator / primary |
| CBUAE Guidance Note, Section 7 — Human Oversight and Consumer Protection | Describes HITL, HOTL and HOOTL approaches; links the degree of human oversight to potential consumer harm; addresses human review, explanation, complaints and alternative arrangements | UAE federal financial-sector regulator / primary |
| CBUAE Guidance Note, governance, monitoring and third-party risk provisions | Retains institutional governance and accountability; addresses ongoing monitoring, third-party AI risk and the institution's ability to stop AI use through human intervention | UAE federal financial-sector regulator / primary |

**Operational reading of the CBUAE oversight models**

- **Human-in-the-loop (HITL):** a human has authority to accept or reject AI outputs.
- **Human-on-the-loop (HOTL):** AI performs routine tasks while a human monitors the process and can intervene.
- **Human-out-of-the-loop (HOOTL):** no direct human intervention in the individual process; the guidance indicates this should be limited to low-risk, non-material operations with appropriate controls.

These are oversight models, not a declaration that every insurance workflow may freely choose any level of autonomy. The appropriate degree of oversight is risk-dependent.

The guidance also addresses the consumer's ability to seek human review or an explanation of an AI-supported decision, alongside complaints, correction and appropriate alternative arrangements. Governance responsibility remains with the regulated institution and its senior leadership; outsourcing or using a third-party AI provider does not transfer the institution's accountability.

**Important interpretation limit:** the Guidance Note is regulatory guidance, not a standalone statute. Its provisions should be described according to their wording and regulatory status; do not rewrite every use of “should” or “expected” as a universal statutory command. The instrument does not establish a blanket rule that every claim denial must receive human approval before it is issued. It establishes a risk-based oversight and consumer-protection framework.

### B. Abu Dhabi healthcare policy and standard — DoH

| Evidence | What it supports | Scope / grade |
|---|---|---|
| DoH Abu Dhabi, *Policy on Use of Artificial Intelligence (AI) in the Healthcare Sector of the Emirate of Abu Dhabi*, published 30 April 2018 | Includes healthcare insurers and billing/insurance processing; frames AI as supportive technology and calls for clear governance, defined AI roles and boundaries, transparency and accountability | Abu Dhabi / primary |
| DoH Abu Dhabi, *Responsible AI Standard*, DoH/ST/DDGO/RAI/V1/2025, October 2025 | Applies to DoH and licensed healthcare entities in Abu Dhabi developing, procuring or deploying AI; requires HITL or HOTL and human oversight, with escalation protocols proportionate to risk | Abu Dhabi / primary |
| DoH Responsible AI Standard, human accountability provisions | Addresses human responsibility, escalation review, override processes, logging and audit trails; states that clinicians should retain ultimate decision-making authority in AI-assisted healthcare scenarios | Abu Dhabi / primary |

**Jurisdictional limit:** the 2025 Responsible AI Standard applies to DoH and licensed healthcare entities in Abu Dhabi within its stated scope. It must not be presented as a UAE-wide rule for every insurer or TPA. The 2018 DoH policy expressly mentions healthcare insurers; the CBUAE guidance is the principal federal financial-sector reference for licensed insurers.

### C. Connected development — AI Clinician Framework

In October 2026, DoH published an AI Clinician Framework / guide examining the conditions under which AI systems may undertake specified clinical activities that have traditionally required a licensed practitioner. The framework uses activity-specific capability assessment and safeguards including physician oversight, accountability and referral to a physician where needed.

This is a connected healthcare development, not evidence that AI systems have been authorised to independently adjudicate health-insurance claims. Its relevance is the wider regulatory examination of task-specific AI capability and the boundaries of human clinical authority.


### D. Institutional deployment evidence — separate record

Institutional AI deployment is documented separately. See [Signal 004 — AI Document Intelligence in UAE Health Insurance Operations](./signal-004-ai-document-intelligence-uae-health-insurance.md) for the Daman / PureHealth case, disclosed functions, evidence boundaries and unresolved questions about operational ownership and decision authority.

No causal relationship between the CBUAE guidance and that deployment is asserted. The deployment was reported for Q3 2025, before the CBUAE Guidance Note published on 11 February 2026.

### Source links

1. [CBUAE Rulebook — Guidance Note, full section](https://rulebook.centralbank.ae/en/entiresection/6967)
2. [CBUAE Rulebook — Section 7: Human Oversight and Consumer Protection](https://rulebook.centralbank.ae/en/rulebook/7-human-oversight-and-consumer-protection)
3. [DoH Abu Dhabi — Policy on Use of Artificial Intelligence in the Healthcare Sector (2018)](https://www.doh.gov.ae/-/media/E9C1470A575146B18015DEBE57E47F8D.ashx)
4. [DoH Abu Dhabi — Responsible AI Standard (October 2025)](https://www.doh.gov.ae/-/media/B84FF5DD027846699C51F36C439A580F.ashx)
5. [WAM — DoH publishes AI Clinician Framework guide (October 2026)](https://www.wam.ae/en/article/17hh7ki-doh-publishes-clinician-framework-guide)

## 3. Cross-sector Connections

The documented regulatory signal connects several parts of the UAE healthcare and health-insurance ecosystem. The connections below are analytical pathways to investigate, not proof that every organisation has implemented them.

| Connection | Why it matters | Current evidence status |
|---|---|---|
| CBUAE ↔ health insurers | Federal financial-sector guidance explicitly covers insurance providers and identifies insurance claims as a high-impact decision example | Regulatory connection verified |
| Insurers ↔ TPAs | Claims workflows may involve delegated administration, external platforms or AI vendors; the regulated institution's governance and third-party controls remain relevant | Operational arrangements require institution-level verification |
| TPAs ↔ claims adjudication | AI may support document processing, coding, eligibility checks, fraud indicators or claim triage; the decision authority and escalation path need to be identified for each workflow | Use cases are investigation questions, not verified adoption claims |
| DoH ↔ healthcare providers | Abu Dhabi's Responsible AI Standard applies to licensed healthcare entities within its scope and addresses human oversight in AI-enabled healthcare | Regulatory connection verified within Abu Dhabi scope |
| AI vendors ↔ regulated institutions | Procurement and outsourcing create questions about model transparency, auditability, monitoring, intervention and the ability to stop use | Governance expectation documented; vendor deployments not established |
| Human oversight ↔ consumer protection | Human review, explanation, complaints and correction mechanisms connect AI governance to the customer's ability to challenge consequential outcomes | Guidance documented; actual customer journey implementation not assessed |
| Clinical decision authority ↔ insurance decision authority | Clinical decisions and insurance coverage/adjudication decisions are distinct, even where they rely on overlapping data or AI tools | Distinction required; no assumption of shared authority |

### Core analytical distinction

**Agent autonomy ≠ decision authority ≠ accountability.**

An AI agent may plan and execute multiple tasks, coordinate tools or prepare a recommendation. That does not, by itself, establish that it has authority to make a consequential clinical or insurance decision, nor does it transfer institutional accountability.

The research must therefore distinguish:

1. **Task execution:** what the system can perform.
2. **Decision authority:** who or what is authorised to make, approve, reject or override the decision.
3. **Accountability:** which licensed institution and accountable human roles remain responsible for the outcome.

## 4. Impact & Opportunity Monitoring

### What is evidenced

- The CBUAE has published a federal financial-sector guidance framework on responsible AI/ML use by LFIs, including insurance providers.
- The CBUAE identifies an insurance claim as an example of a high-impact decision.
- The CBUAE describes different human-oversight approaches and links oversight intensity to risk and potential consumer harm.
- DoH Abu Dhabi's 2018 AI policy expressly includes healthcare insurers and billing/insurance processing.
- DoH Abu Dhabi's 2025 Responsible AI Standard requires HITL or HOTL and human oversight for AI systems within its stated healthcare-entity scope.
- Institutional governance and accountability remain central even where AI systems or third-party providers are involved.

### What is not established

- That TPAs have deployed AI agents in live claims operations.
- That any insurer or TPA in the UAE operates claims workflows under HOTL or HOOTL.
- That AI systems currently make final coverage, medical-necessity or payment decisions without human review.
- That every claim denial must legally receive human approval before communication.
- That the guidance has already caused a measurable change in staffing, job titles, outsourcing or workforce demand.
- That the Abu Dhabi healthcare standard applies to every insurer or healthcare entity across the UAE.

### Opportunity hypotheses to test

- Insurers and TPAs may need clearer AI governance, model oversight and operational-control responsibilities.
- Claims teams may evolve toward exception handling, escalation review, evidence validation and oversight of AI-assisted workflows.
- Third-party AI procurement may increase the importance of vendor due diligence, audit rights, monitoring and intervention controls.
- New or changing responsibilities may emerge across claims operations, compliance, risk, clinical governance, data and technology teams.

These are hypotheses only. They must not be presented as current hiring demand or established market outcomes without dated employer disclosures, procurement evidence, operating documentation or job-posting analysis.

### Follow-up monitoring tests

1. **Insurer adoption:** collect dated, attributable disclosures from UAE insurers about AI in claims, underwriting, customer service or fraud operations; distinguish document processing from adjudication and decision automation.
2. **TPA implementation:** identify named AI tools and live workflows, distinguishing pilots, vendor announcements and production deployment.
3. **Decision authority:** identify, for each verified live AI use case, the formally designated operational owner and the documented authority to approve, reject, override, suspend or stop outputs; see Signal 004 for the Daman-specific investigation.
4. **Human review in practice:** examine customer-facing review, explanation, complaint and appeal routes, without assuming that policy text proves operational effectiveness.
5. **Third-party governance:** track AI procurement, outsourcing arrangements, model inventories, audit provisions and vendor-control disclosures.
6. **Workforce implications:** sample dated vacancies and role descriptions for AI governance, claims oversight, exception handling, compliance and operational risk; distinguish explicit requirements from inferred demand.
7. **Jurisdictional comparison:** investigate whether and how comparable requirements apply in Dubai and other emirates, using the relevant authority's own instruments.
8. **Clinical versus insurance authority:** keep clinical decision-making and insurance claim adjudication as separate decision domains unless a specific workflow documents their relationship.

### Central research question

**Are institutions automating tasks, or transferring decision authority itself to AI systems?**

The observatory will track evidence of both separately. An announcement of automation is not proof of autonomous decision-making; a human-oversight policy is not proof of how a live workflow operates.

**Public-facing summary:** UAE regulatory instruments articulate risk-based human-oversight expectations for AI use across financial services and, within Abu Dhabi's stated jurisdiction, healthcare. The instruments establish regulatory direction; they do not by themselves demonstrate how individual live workflows implement human review, escalation or intervention. Institutional deployments are documented in separate signal records.

**Method note:** AI may assist discovery, comparison and evidence organisation. Source verification, interpretation, accountability and final judgement remain human responsibilities.
