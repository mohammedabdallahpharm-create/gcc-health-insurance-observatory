# Signal 010 — Patient Data Flow and Decision Power in UAE Healthcare

**Record ID:** UAE-HI-010  
**Market:** United Arab Emirates; emirate-specific implementation boundaries retained  
**Signal type:** Health-information infrastructure / data governance / clinical operations / insurance decision interfaces  
**Primary radar:** Digital Health & AI  
**Connected radars:** Regulatory, payer, provider, reimbursement  
**Primary systems / authorities:** Riayati / NUMR, Malaffi, NABIDH, MOHAP, DoH Abu Dhabi, DHA  
**Observation date:** 27 November 2026  
**Evidence status:** National platform integration, selected platform functions, Abu Dhabi 2026 data-standardisation requirements, clinical-use requirements and the 10 November integration of an AI Physician Assistant into Malaffi are verified from official sources. Cross-emirate completeness, uniform access and insurer/TPA access to full clinical records are not established.  
**Confidence:** High that a connected national health-information architecture and material Abu Dhabi data-governance requirements exist; moderate that data is increasingly embedded in clinical workflows, including an AI-assisted clinical information-retrieval use case; low / unverified for any claim that a single actor controls the complete patient-data journey or that insurers/TPAs have general access to full clinical records.

## 1. External Signal Detection

The UAE patient-data environment is not a single undifferentiated database. It is a connected architecture involving emirate-level health-information exchanges and the National Unified Medical Record (NUMR):

- **Malaffi** is the Abu Dhabi Health Information Exchange (HIE), operating within the Department of Health Abu Dhabi framework.
- **NABIDH** is Dubai Health Authority's HIE.
- **Riayati** delivers the National Unified Medical Record (NUMR) programme under MOHAP and is integrated with Malaffi and NABIDH.
- MOHAP separately describes the **e-Claims Post Office** as a system for secure exchange of health-insurance claims and related data between providers and payers in the Northern Emirates.

The distinction is strategically important: clinical-record exchange and insurance-claims exchange are connected parts of the healthcare information environment, but they are not the same data product, transaction, permission model or decision process.

The emerging question is not simply who stores patient data. It is who creates it, standardises it, connects it, is authorised to access it, uses it in a clinical or administrative workflow, and can translate it into a decision that affects care, coverage, reimbursement or payment.

## 2. Primary-source evidence

### A. National integration of the three HIE platforms

On 31 January 2023, MOHAP, DoH Abu Dhabi and DHA announced the successful integration of Riayati, Malaffi and NABIDH. The announcement described the integration as supporting access to patient health information by healthcare providers across the UAE and continuity of care.

**Evidence boundary:** this confirms the announced integration architecture. It does not prove that every data category, every facility, every user role or every record is universally available across all platforms at the same time.

Source:
- [DoH Abu Dhabi — UAE health authorities announce integration between Riayati, Malaffi and NABIDH (31 January 2023)](https://www.doh.gov.ae/en/news/uae-health-authorities-announce-successful-integration-between-riayati-malaffi-and-nabidh)

### B. Riayati / NUMR and the separate e-Claims Post Office

MOHAP describes Riayati as the platform delivering the National Unified Medical Record. Its public page lists connected systems and facilities, secure exchange, interoperability and real-time access. It also identifies the e-Claims Post Office as a separate exchange system for health-insurance claims and related data between providers and payers in the Northern Emirates.

The same MOHAP page reports 4.00 billion connected medical records, 14 million unique patients, 116,071 connected clinicians and 4,952 connected healthcare facilities. However, the page labels its information as last updated October 2024. These figures are therefore historical published platform metrics, not verified November 2026 live totals.

The page states that access to medical records is limited to authorised users such as doctors, nurses and allied-health clinicians, and describes security checks controlling access.

Sources:
- [MOHAP — Riayati](https://mohap.gov.ae/en/riayati)
- [MOHAP — About NUMR](https://mohap.gov.ae/en/riayati/about-numr)

### C. Malaffi: data availability, phased capture and role-based access

Malaffi's end-user FAQ lists available categories including demographics, laboratory results, procedures, vital signs, encounters, radiology reports and images, diagnoses, immunisations, allergies, medications, clinical documents, appointments, family/social history and genomics data.

The FAQ also states:
- data sets are captured in phases and some data may not yet be available;
- correct demographic matching is important for linking a facility's EMR record to a patient's Malaffi record;
- access is governed by role-based permissions and organisational security protocols;
- access is monitored and logged;
- only Level 1 users have authority to break the privacy seal and access all patient data, including sensitive information;
- patients can view their information through Sahatna.

Malaffi's FAQ describes Riayati as the HIE for the Northern Emirates and NABIDH as the HIE for Dubai, while describing the scope of cross-platform integration and future integration plans. This detail should be read as a platform-specific operational statement, not as proof of unrestricted or symmetrical access across all systems.

Sources:
- [Malaffi — Frequently Asked Questions for End Users](https://www.malaffi.ae/frequently-asked-questions-end-users/)
- [Malaffi — Policies and patient-data privacy](https://www.malaffi.ae/what-is-malaffi/policies/)

### D. Abu Dhabi 2026: data standardisation, minimum data sets and auditability

DoH Abu Dhabi's Health Information Exchange Standards page describes 2026 data standards and mandates specific coding standards, units of measurement, data classification protocols and a minimum data set for information transmitted from source EMR systems and reference laboratory information systems to Malaffi.

DoH Circular 2026/212, dated 27 October 2026, requires healthcare providers to:
- use specified standards when capturing and recording patient demographic and clinical data;
- capture and transmit a minimum data set from source EMR and reference LIS systems to Malaffi; and
- maintain appropriate audit logs for creation, modification and deletion of patient demographic and clinical data.

This is a material operational signal: data quality, standardisation, completeness and traceability are being formalised as provider obligations, not left solely to voluntary interoperability.

Sources:
- [DoH Abu Dhabi — Health Information Exchange Standards 2026](https://www.doh.gov.ae/en/resources/HIE)
- [DoH Abu Dhabi — Circular 2026/212, Data Standardization (27 October 2026)](https://www.doh.gov.ae/-/media/Feature/Resources/Circulars/2026/212--2026.ashx)

### E. Abu Dhabi 2026: data is being embedded into clinical workflow

DoH Circular 2026/30, dated 19 February 2026, mandates clinicians, including doctors and nursing staff, to use Malaffi before requesting laboratory or radiology examinations. The circular says this is intended to let clinicians review existing clinical data and previous examinations, avoid unnecessary repeat tests and improve patient safety and treatment outcomes.

This establishes a direct workflow connection between access to longitudinal clinical information and a clinical action. It does not, by itself, establish a measured reduction in testing, cost or claims expenditure.

Source:
- [DoH Abu Dhabi — Circular 2026/30, Mandatory Use of Malaffi by Clinicians (19 February 2026)](https://www.doh.gov.ae/-/media/04C7CDE980824E4C8AAB804F07823AE3.ashx)

### F. Federal legal and privacy boundary

The executive regulation under the federal health ICT law provides conditions for using the central system and exchanging health data. It requires authorised users to undertake confidentiality obligations, restricts disclosure to parties without patient consent except where permitted by applicable legislation, provides for emergency access in specified circumstances, and requires suspicious confidentiality incidents to be reported. The legislation also recognises a person's ability to request restrictions on access subject to applicable requirements and controls.

These provisions do not mean every healthcare use requires a separate consent workflow; applicable legal bases, exceptions and sector-specific rules must be examined for each purpose and jurisdiction.

Source:
- [UAE Legislation — Cabinet Resolution concerning the Executive Regulations of the Federal Law on Health ICT (2020), Article 6](https://uaelegislation.gov.ae/en/legislations/1444/download)

### G. Abu Dhabi 2026: AI Physician Assistant integrated into Malaffi

On 10 November 2026, DoH Abu Dhabi and M42's Abu Dhabi Health Data Services (ADHDS) announced that an AI Physician Assistant had been integrated into Malaffi and made available to physicians across Abu Dhabi. The assistant is powered by Ossi, M42's AI Clinical Platform, and hosted on Microsoft Azure infrastructure in the UAE.

The announced functions are information retrieval from authorised patient records, concise summaries of health histories and responses to physicians' queries. The announcement describes Malaffi as containing information on more than 14 million patients and over four billion clinical records. These are figures reported in the announcement, not independently audited measures in this record.

The announcement identifies distinct roles:
- **DoH Abu Dhabi:** health-sector regulator and partner in the initiative.
- **ADHDS / M42:** operates Malaffi and is responsible for integrating the assistant into the platform.
- **M42 / Ossi:** supplies the AI clinical platform powering the assistant.
- **Microsoft Azure:** provides the UAE-hosted cloud infrastructure identified in the announcement.
- **Physicians:** retain responsibility for clinical assessment and decisions.

The implementation is to be evaluated, with findings and physician feedback informing future improvements.

**Evidence boundary:** this is evidence of an AI information-retrieval and summarisation capability embedded in a live clinical information environment and made available to physicians. It does not establish autonomous diagnosis, treatment selection, prescribing, claims adjudication, insurer/TPA access, or transfer of clinical decision authority to the AI system. The public announcement does not disclose detailed model evaluation results, error rates, usage volumes, clinical outcomes or the complete operational accountability framework.

Sources:
- [Malaffi — Abu Dhabi Integrates AI Physician Assistant into Malaffi (10 November 2026)](https://www.malaffi.ae/abu-dhabi-integrates-ai-physician-assistant-into-malaffi-to-support-physicians-and-enable-more-time-for-patient-care/)
- [Emirates News Agency (WAM) — Department of Health – Abu Dhabi integrates AI physician assistant into Malaffi (10 November 2026)](https://www.wam.ae/en/article/c36osyl-department-health-abu-dhabi-integrates-physician)

## 3. Patient Data Journey — working map

| Stage | Typical data / action | Potential control points | Evidence status |
|---|---|---|---|
| 1. Generation | Encounter, diagnosis, medication, lab, imaging, procedure, allergy | Provider and clinician; source EMR / LIS / RIS | Established as the source-system model |
| 2. Capture and identity matching | Patient identifiers, demographics, record matching | Provider registration workflow; data standards; EMR vendor | Malaffi documents the importance of correct demographics and matching |
| 3. Standardisation and transmission | Coding, units, minimum data set, audit trail | Regulator requirements; provider IT and data-governance teams | Abu Dhabi 2026 requirements verified |
| 4. Exchange and longitudinal view | HIE / NUMR connectivity across participating systems | Malaffi, NABIDH, Riayati and their authorised connections | National integration announced; availability varies by data set and permission |
| 5. Clinical use | Review prior results, history, medications and imaging | Clinician role, facility access policy, HIE access controls | Abu Dhabi pre-test use requirement verified |
| 6. Administrative / insurance use | Eligibility, authorisation, claim documentation and adjudication | Insurer / TPA systems and contractually authorised data flows | Exact clinical-data access scope requires further evidence |
| 7. Analytics and secondary use | Quality, population health, planning, risk models, AI | Legal basis, governance, de-identification or other safeguards, access permissions | Use cases exist; actor-by-actor permissions and datasets require verification |
| 8. Retention, correction and audit | Amendments, access logs, retention and incident handling | Data controller / custodian, provider, platform and regulator | Selected Abu Dhabi audit-log and federal privacy requirements verified |

This is a functional map, not a claim that every data item follows one linear route or is accessible to every participant.

## 4. Interpretation — what the evidence suggests

### Finding 1: The UAE has a connected national direction, but not proof of one universally uniform record

The official integration announcement and MOHAP's NUMR description support a national interoperability architecture. Platform-specific FAQs and phased data capture show why national integration must not be confused with identical data completeness, access or operational permissions in every emirate and facility.

### Finding 2: Data quality and traceability are becoming operational obligations

DoH's 2026 standards and Circular 2026/212 move the discussion beyond connectivity. Standardised capture, minimum data sets and audit logs create obligations at the source-system and provider level. This makes data quality and governance material operating capabilities.

### Finding 3: Patient data is being used closer to the point of clinical decision

Circular 2026/30 makes Malaffi review part of the workflow before selected lab and radiology requests. This is evidence of clinical workflow integration, not merely passive record storage.

### Finding 4: AI is beginning to operate as an intelligence interface over connected clinical data\n\nThe 10 November Malaffi integration moves beyond data exchange alone: an AI assistant is now described as helping authorised physicians retrieve and summarise information within an existing clinical workflow. The disclosed architecture separates the HIE operator/integrator, AI platform, cloud infrastructure, regulator and physician decision-maker. This is evidence of an emerging intelligence layer, not proof that one participant controls all layers or that the assistant makes clinical decisions.\n\n### Finding 5: The information infrastructure and the financial infrastructure intersect, but remain distinct

Riayati's e-Claims Post Office is explicitly described as exchanging claims and related data between providers and payers in the Northern Emirates. That should not be conflated with the clinical NUMR record. The patient-data-to-payment relationship therefore needs to be mapped through the specific claims and authorisation interfaces, contracts and data permissions, not assumed from HIE connectivity.

## 5. Competing hypotheses

**Hypothesis A — Infrastructure leverage:** organisations that operate or integrate critical data infrastructure may gain influence by shaping data availability, standardisation, identity matching and workflow integration. This is a hypothesis about infrastructure influence, not proof of ownership of patient data or authority over clinical decisions.

**Hypothesis B — Provider-originated control:** healthcare providers may retain decisive influence because they create source records, determine clinical context and operate the EMR workflows that transmit data. HIE connectivity may distribute access without transferring source-data control.

**Hypothesis C — Regulatory orchestration:** regulators may hold the strongest system-level influence by defining mandatory data sets, interoperability standards, permitted purposes, security controls and audit obligations, even though they do not operate every clinical workflow.

**Hypothesis D — Fragmented permission model:** access may remain deliberately distributed across roles, organisations, emirates, contracts and legal purposes. In this model, no single actor can see or control the complete patient-data journey.

**Hypothesis E — Financial decision boundary:** insurers and TPAs may receive the clinical and administrative information necessary for defined insurance functions, but this does not imply general access to the full longitudinal clinical record. The exact datasets, interfaces, legal basis and delegated roles must be established before attributing broader power.

## 6. What this signal does NOT establish

- It does not establish that all UAE patient records are complete, synchronised or universally accessible across all three HIEs.
- It does not establish that every facility or every data category is connected and transmitting in real time.
- It does not establish that insurers or TPAs have unrestricted access to Malaffi, NABIDH or Riayati clinical records.
- It does not establish that an HIE operator owns the underlying patient data or can use it for any purpose.
- It does not establish that AI systems autonomously make clinical, coverage or claims decisions.
- It does not establish a quantified reduction in duplicate testing, healthcare expenditure, claims cost or fraud.
- It does not establish that the 2024 MOHAP platform metrics are current November 2026 totals.
- It does not establish that Abu Dhabi-specific requirements apply identically in Dubai or the Northern Emirates.

## 7. Cross-radar connections

| Existing record / radar | Connection to UAE-HI-010 | Why it matters |
|---|---|---|
| UAE-HI-001 — Dubai claims and health-data exchange | Digital / reimbursement | Keeps clinical interoperability distinct from payer-provider claims exchange |
| UAE-HI-003 — UAE digital health infrastructure | Digital / regulatory | Connects patient-data infrastructure to the wider digital-health architecture |
| UAE-HI-004 — Daman AI document intelligence | Payer / digital | Tests the boundary between structured clinical information and insurance-document processing |\n| UAE-HI-007 — AI agent operational ownership | Digital / payer / workforce | Compares clinical AI integration with the unresolved ownership of live AI workflows |\n| UAE-HI-012 — Predictive health and insurance economics | Digital / reimbursement / payer | Tests whether population-health intelligence can connect to cost and insurance decisions |
| UAE-HI-009 — PureHealth, Daman and claims decision control | Payer / provider / capital / digital | Examines whether vertical integration changes access, orchestration or decision influence |
| UAE-HI-008 — ADOC market readiness | Regulatory / reimbursement | Links data and claims requirements to provider operational readiness |

## 8. Follow-up research tests

1. **Dubai:** retrieve and compare current DHA/NABIDH interoperability standards, data-sharing policies, user roles and audit requirements with the Abu Dhabi framework.
2. **Northern Emirates:** map Riayati NUMR clinical exchange separately from the e-Claims Post Office, including the data elements, participants and transaction boundaries.
3. **Insurer / TPA interfaces:** find primary evidence for what clinical information is exchanged for eligibility, prior authorisation, medical necessity, claims adjudication and appeals; identify the legal basis and delegated roles.
4. **Provider source systems:** map the responsibilities of EMR, LIS, RIS and provider data-governance teams for data quality, correction, matching and transmission.
5. **AI use:** identify the exact datasets, user roles, human checkpoints, auditability and intended purposes of AI systems that consume patient data. For the Malaffi Physician Assistant, seek deployment metrics, evaluation design, error/omission monitoring, clinician feedback, escalation procedures and the named operational owner for ongoing performance.
6. **Economic impact:** seek measured evidence for duplicate-test reduction, authorisation turnaround, claims rework, payment-cycle effects and cost outcomes. Do not infer savings from connectivity alone.
7. **Cross-emirate comparability:** verify which standards and access capabilities are genuinely national versus emirate-specific.

## 9. Working conclusion

The strongest evidence-backed conclusion is that the UAE has a connected national health-information direction, while implementation, data completeness and access remain governed by platform, facility, role and jurisdictional boundaries. Abu Dhabi's 2026 standards and clinician-use circulars show that patient data is becoming more deeply embedded in both provider data operations and clinical workflows.

The strategic power question is therefore not simply “who owns the data?” It is:

**Who sets the rules, creates the source record, controls data quality, operates the exchange, authorises access, and converts permitted information into a clinical or financial decision?**

The public evidence reviewed does not yet justify naming one actor as the controller of the complete patient-data journey. That is the next investigation, particularly at the boundary between clinical HIE data and insurance claims / authorisation data.

**Method note:** AI may assist with source discovery, comparison and synthesis. Evidence verification, interpretation and final judgement remain human responsibilities.
