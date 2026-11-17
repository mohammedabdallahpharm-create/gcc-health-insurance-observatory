# Case Trace 001 — Dubai Outpatient Claim: Decision Authority, Data Handoffs & Financial Settlement

**Record type:** End-to-end operational case trace  
**Jurisdiction:** Emirate of Dubai, UAE  
**Scenario:** Illustrative outpatient consultation and a covered service at a DHA-licensed network clinic  
**Evidence cut-off:** 17 November 2026  
**Status:** Public-rule trace; not a real patient claim, not a transaction audit, and not evidence of any named insurer–TPA contract.

## Executive finding

The public evidence establishes a regulated electronic claims path in Dubai: provider identity/eligibility checks and documented care → electronic claim submission through eClaimLink → insurer/TPA adjudication → Remittance Advice (RA) on the Dubai Health Post Office (DHPO) → settlement of approved amounts by the insurer within the prescribed period.

Decision authority is distributed, not unitary:

- The clinician/provider owns the clinical assessment and source documentation.
- The provider's billing/claims function owns accurate coding, completeness and submission.
- The insurer owns the coverage obligation and remains accountable for payment/remittance timelines, even when administration is outsourced.
- A TPA may perform delegated claims-management and adjudication work; the precise authority for a specific claim depends on the insurer–TPA mandate, which is not publicly established here.
- DHA/DHIC sets and enforces the regulatory framework; it does not adjudicate every individual claim.

The money trail is only partly visible in public evidence. The rule establishes the approved claim settlement obligation and RA content, but not the actual bank transfer, bank value date, provider receipt, reconciliation ledger or allocation of any efficiency savings. Those require transaction-level evidence.

## 1. Scenario boundaries

For the trace, assume:
- A validly insured member attends a DHA-licensed, in-network outpatient clinic.
- The clinician documents a consultation and a clinically indicated service.
- The service is covered and, for this illustrative path, does not require prior authorisation. If the policy/service requires prior authorisation, insert the authorisation decision before service delivery.
- The provider submits a complete electronic claim and the payer approves it in full.
- No real patient, insurer, TPA, provider, claim amount or transaction identifier is represented.

No monetary amount is invented. The patient's applicable co-payment/deductible is policy-specific and is not assumed to be zero.

## 2. End-to-end trace

| Stage | Data / event hand-off | Decision authority | Financial movement | Evidence status |
|---|---|---|---|---|
| 0. Policy funding | Employer/sponsor/member enrolment and policy details establish eligibility and benefits | Employer/sponsor enrols where applicable; insurer issues/underwrites coverage subject to applicable rules | Premium funding flows to insurer under policy/contract | Legal enrolment responsibility is documented; the actual premium transfer for this scenario is not observed |
| 1. Patient access | Patient identity, policy/card, eligibility and network status are checked | Provider verifies identity and eligibility; payer systems provide coverage information | Patient may owe policy-defined co-pay/deductible to provider | Verification requirement is documented; exact API calls and returned fields are not public in this trace |
| 2. Clinical encounter | Symptoms, assessment, diagnosis, treatment and clinical notes are recorded in provider system | Treating clinician makes clinical judgement | Provider incurs care-delivery cost; patient may pay any applicable share | Clinical source record is the provider's responsibility; no patient-level record is available |
| 3. Coding & claim assembly | Encounter is translated into diagnosis/service codes, patient and policy data, claimed amount and supporting evidence | Provider coding/billing team validates accuracy and completeness | No insurer settlement yet; provider carries receivable / collection exposure | DHA/DHIC directive requires completed, documented services and accurate validated data |
| 4. Electronic submission | Claim is submitted in the prescribed XML/eClaimLink workflow and routed through DHPO | Provider controls submission; platform standardises/transmits the transaction | No payment merely because a claim was submitted | Electronic submission requirement and eClaimLink role are documented |
| 5. Adjudication | Claim data is checked against eligibility, policy limits, covered services, co-pay/deductible and applicable rules | Insurer or its delegated TPA performs the claims workflow; exact human/system split and named delegation require contract-level proof | Claim may be approved, denied, reduced or queried; approved payable amount becomes due under applicable rules | Adjudication checks and TPA role are documented; exact authority matrix for a named portfolio is unknown |
| 6. Remittance Advice | RA is posted with claim reference, payment status, denial reason where relevant and settlement amount | Insurer/TPA must provide accurate RA; insurer remains accountable for timeline compliance | RA communicates settlement outcome; it is not, by itself, proof of bank credit | Required RA fields are documented |
| 7. Payment & closure | Payer processes approved settlement; provider matches payment to claim/RA and reconciles ledger | Insurer is accountable for settling approved claims; operational execution may involve delegated parties/banks | Insurer/payer → provider. Actual transfer route, bank value date, deductions and receipt require bank/ledger evidence | Regulatory payment deadline is documented; actual cash movement is not publicly observable |
| 8. Dispute / resubmission (if needed) | Provider challenges denial or missing/incorrect adjudication using RA and supporting records | Provider initiates resubmission; insurer/TPA re-adjudicates; formal reconciliation applies where required | Payment may be delayed or adjusted pending final outcome | Directive sets resubmission and reconciliation procedures |

## 3. What the rules establish

1. **Eligibility and identity:** Providers must verify patient identity and eligibility before rendering services using eClaimLink.
2. **Claim creation:** Claims are submitted after the relevant encounter services are completed and documented; data must be accurate, complete and validated.
3. **Electronic rail:** The 2025 DHA/DHIC policy directive says claims outside eClaimLink are not processed for settlement.
4. **Adjudication:** Insurers and TPAs must verify services against coverage limits and applicable co-pay/deductible requirements. TPAs are prohibited from modifying claim documentation or beneficiary data.
5. **RA:** Each claim's RA must carry its reference, payment status, denial reason where applicable and settlement amount.
6. **Payment accountability:** Insurers remain accountable for payment/remittance timelines even when claims administration is outsourced.
7. **Timeline:** Approved adjudicated claims must be paid and the RA posted within 45 calendar days from claim submission. Resubmitted claims have a 30-calendar-day timeline from resubmission under the directive.

These are regulatory requirements, not proof that every payer/provider pair performs identically or that every payment arrives on the final permitted day.

## 4. Three separate flows — do not collapse them

### A. Premium money
Employer/sponsor/member → insurer. This funds the insurance arrangement. It is not the same transaction as a provider claim payment.

### B. Claims information
Provider → eClaimLink / DHPO → insurer or delegated TPA. This is an information and adjudication workflow; the submission itself is not money.

### C. Claim payment
Insurer/payer → provider, following adjudication and subject to contractual/regulatory settlement terms. The RA is evidence of the adjudicated settlement instruction/status, not independent proof of bank receipt.

### D. Patient cost-share
Patient/member → provider, where a co-payment or deductible applies. The provider must collect and accurately record the applicable amount; the exact amount depends on the policy and service.

## 5. Where decision power sits

| Actor | What it can decide/control | What it does not automatically control |
|---|---|---|
| DHA / DHIC | Regulatory rules, approved claims methods, oversight, compliance and dispute framework | Every clinical decision or each individual claim outcome |
| Provider / clinician | Clinical assessment, treatment and source clinical documentation | Insurance coverage entitlement or payer adjudication |
| Provider billing/coding | Claim representation, coding quality, completeness, submission timing | Whether the payer will approve coverage |
| Insurer | Coverage obligation, policy terms, payer accountability and approved-claim settlement | Clinical judgement at point of care |
| Delegated TPA | Contractually delegated eligibility/claims review/adjudication workflows and network administration | Authority beyond the specific mandate; ultimate insurer accountability for regulated payment timelines |
| eClaimLink / DHPO | Standardised electronic exchange, tracking and RA communication | Clinical judgement, underwriting risk or the underlying bank transfer decision |
| AI / automation | Potentially classify, extract, validate, flag anomalies and prioritise workflows | Independent final authority unless a specific lawful and accountable delegation is evidenced; no such autonomy is established by this trace |

## 6. Where economic value may accumulate — hypotheses, not findings

- **Provider:** revenue for delivered care, subject to contracted tariffs, adjudication and collection; cost-to-serve and receivables timing matter.
- **Insurer:** premium income, risk pooling and claims-cost exposure; actual underwriting margin cannot be inferred from one claim.
- **TPA:** administrative/service revenue under its contract; fee basis and incentives are not disclosed in this case.
- **Technology / exchange layer:** operational value may arise from standardisation, connectivity, workflow and auditability; no platform revenue or value share is established here.
- **AI / workflow vendors:** potential value from lower manual effort, fewer errors, faster cycle times and better exception handling; realised savings and who captures them remain unverified.

Do not equate claim value, premium value, provider revenue, TPA fees, insurer profit or AI-generated savings. They are different economic quantities.

## 7. Critical unknowns — the next evidence request

To turn this public-rule trace into a true transaction trace, obtain a de-identified claim pack from one willing provider/payer pair:

1. Provider encounter timestamp and clinical-documentation provenance.
2. Eligibility response and exact policy/benefit fields used.
3. Any prior-authorisation request/response, if applicable.
4. Submitted claim payload or a redacted field-level export, claim ID and submission timestamp.
5. The insurer–TPA delegation matrix effective on that date, including who can approve, pend, deny and override.
6. Adjudication audit trail: rule/reason codes, reviewer identity/role, AI assistance if any, override history and timestamps.
7. Final RA with claim reference, decision, denial codes if any, settlement amount and posting timestamp.
8. Bank transfer reference/value date and provider ledger entry proving receipt.
9. Provider reconciliation record, patient co-pay/deductible collection and any adjustments.
10. Contractual TPA fee model and provider tariff/discount terms, if economic value capture is being tested.

Only use de-identified or synthetic records with lawful access. Do not collect patient identifiers or confidential commercial data without permission.

## 8. Preliminary conclusion

The strongest documented control point is **the insurer-led coverage/adjudication and payment-accountability layer**, with operational execution potentially delegated to a TPA. The provider controls the clinical source record and the quality of claim construction. eClaimLink/DHPO controls an important standardised exchange and traceability layer, but does not itself establish who owns the clinical or financial decision.

The strongest unclosed gap is **cash proof**: public evidence tells us what should be settled and by when, but not when money actually leaves the payer, reaches the provider, is reconciled, or how any operational savings are divided.

**Working hypothesis:** strategic influence concentrates at the hand-offs where clinical evidence becomes a coded claim, payer rules become an adjudication outcome, and the RA becomes actual cash. The hypothesis should only be upgraded after a redacted claim payload, delegation evidence, adjudication audit trail and bank/ledger proof are matched to the same claim ID.

## 9. Primary sources

- Dubai Law No. 11 of 2013, especially Articles 2, 5, 9, 14 and 15: https://dlp.dubai.gov.ae/Legislation%20Reference/2013/Law%20No.%20%2811%29%20of%202013.html
- DHA / DHIC, Health Insurance Claims Management Policy Directive, DHIC/HIR-002/2024, issued 27 October 2025, effective 16 November 2025: https://www.isahd.ae/content/docs/PD-05-2025%20Dubai%20Health%20Insurance%20Claims%20Management.pdf
- eClaimLink, About the platform: https://www.eclaimlink.ae/about.aspx/default.aspx
- DHA, NABIDH platform overview: https://www.dha.gov.ae/en/aboutus/projectsAndInitiatives
- Government of Dubai, Health Insurance Implementing Bylaw, Administrative Resolution No. 78 of 2022: https://dlp.dubai.gov.ae/Legislation%20Reference/2022/Administrative%20Resolution%20No.%20%2878%29%20of%202022%20Issuing%20the%20Implementing%20Bylaw%20of%20Law%20No.%20%2811%29%20of%202013.html
