# Affinity Chart: Healthcare AI Clinical Deterioration Evaluation

## Purpose and scope

This chart organizes working needs for a hypothetical 300-bed German hospital considering an AI-supported clinical deterioration prediction system. The proposed scope is a supervised 12-week evaluation on two internal medicine wards, with comparison wards and a specified protocol, only after clinical, technical, governance, legal and funding prerequisites are met. 

## Classification and reading guide

- **Business (B):** an outcome or organizational objective the initiative is intended to support. An objective is not guaranteed by a feature.
- **Functional (F):** a behavior or capability the system or defined workflow should provide.
- **Non-functional (NF):** a quality, performance or constraint applying to a capability or service.
- **Transition (T):** an activity or temporary capability needed to prepare, validate or move into the evaluation.

Each row has one primary classification, although a theme can contain several types and some needs could be decomposed further. IDs beginning **AC** are identifiers for this chart, not new IDs in the source requirements documents. Where a source ID is shown, it identifies the related working item rather than a claim of exact one-to-one equivalence. Priorities and thresholds require approval; the pilot's “Won't” status applies only to the baseline evaluation.

## Affinity chart

### 1. Clinical recognition and action

| Chart ID | Working need or requirement | Type | Trace to case / indicative stakeholders | Status and validation |
|---|---|---|---|---|
| AC-01 | Improve timely recognition and appropriate clinical response without increasing harm. | Business | BR-01; clinical lead, nurses, patients | Must objective in the working requirements; outcome not established. |
| AC-02 | Display an alert to the responsible authorized clinical team when required valid EHR inputs support risk above an approved threshold. | Functional | FR-01; clinical and informatics leads | Must proposal; threshold and response ownership require clinical approval and local validation. |
| AC-03 | Show authorized staff the relevant observed inputs, timestamp and appropriate risk context for an alert. | Functional | FR-02; clinicians, nurses | Must minimum proposal; richer explanation is Should in the baseline and must not imply causal certainty. |
| AC-04 | Provide an assigned alert owner, acknowledgement, visible status and backup escalation through a tested workflow. | Functional | Case study R3; ward and rapid-response teams | Must proposal; acknowledgement is not assessment or treatment. |
| AC-05 | Make a qualifying alert visible within five minutes of the last required valid data becoming available in the EHR. | Non-functional | NFR-01; clinical and technical owners | Draft acceptance target, not an approved clinical standard; measure EHR and delivery delays separately. |

### 2. Trustworthy data and delivery

| Chart ID | Working need or requirement | Type | Trace to case / indicative stakeholders | Status and validation |
|---|---|---|---|---|
| AC-06 | Integrate the required EHR observations with the evaluation system and associate them with the correct patient. | Functional | Case study R1; IT and clinical informatics | Must proposal; validate identity, mapping, units, timestamps and completeness. Targeted EHR changes may suffice; replacement is not assumed. |
| AC-07 | Signal missing or stale required data and follow an approved fallback instead of displaying a misleading reassuring result. | Functional | FR-01 / NFR-02 negative test; IT and clinical safety | Proposed behavior; exact tolerances, indication and fallback need specification and testing. |
| AC-08 | Define and test data freshness, availability, secure delivery and safe failure behavior under agreed operating conditions. | Non-functional | NFR-02; IT, safety and clinical owners | Safe fallback is a Must; numeric availability and freshness targets remain unresolved. |
| AC-09 | Validate source-to-display data mapping and local model performance before live use; freeze and version the model. | Transition | TR-01; data science, IT and clinical leads | Must entry proposal; retrospective validation and prospective evaluation are distinct. |

### 3. Privacy and accountability

| Chart ID | Working need or requirement | Type | Trace to case / indicative stakeholders | Status and validation |
|---|---|---|---|---|
| AC-10 | Protect patient records and meet applicable data protection obligations. | Business | BR-03; patients, privacy and legal leads | Must objective; applicable obligations and controls require local review. |
| AC-11 | Restrict patient-specific records, alerts and context to roles authorized for the relevant patient, and log access attempts. | Functional | FR-03; privacy, security and clinical owners | Must proposal; test both authorized and unauthorized cases and approved reporting procedures. |
| AC-12 | Maintain attributable records of alerts, acknowledgements, actions and configuration changes, subject to approved access and retention rules. | Functional | Case study R7; clinical safety and security | Must proposal; verify log retrieval, access restrictions and local retention requirements. |
| AC-13 | Define and test security and privacy controls proportionate to the intended use. | Non-functional | NFR-02 / BR-03; privacy, security and legal leads | Control specifications and applicable approvals remain open; independent local review is needed. |

### 4. Safe adoption and controlled change

| Chart ID | Working need or requirement | Type | Trace to case / indicative stakeholders | Status and validation |
|---|---|---|---|---|
| AC-14 | Train staff and rehearse alert response, escalation, handover and fallback across relevant shifts before live use. | Transition | TR-02; nursing, clinical and training leads | Must proposal; define completion, competency and drill criteria. |
| AC-15 | Establish clinical safety governance, accountable response ownership and incident escalation before live alerts. | Transition | Case study decision conditions and safety gates; safety and project leads | Proposed entry condition; designate authority and test pause and return-to-usual-care procedures. |
| AC-16 | Exclude automated model retraining during the baseline evaluation; review and approve any controlled change. | Non-functional | FR-04 and case study R8; evaluation, safety and vendor leads | Won't for automated retraining in this pilot; the frozen model and change control require verification. Classified here as a constraint, although FR-04 is labeled functional in the source. |

### 5. Value and learning

| Chart ID | Working need or requirement | Type | Trace to case / indicative stakeholders | Status and validation |
|---|---|---|---|---|
| AC-17 | Determine whether a sustainable investment case is credible using clinical, operational and financial evidence. | Business | Case study financial objective; sponsor and finance | Working objective, not a promise of positive ROI. |
| AC-18 | Explore whether avoidable ICU transfer costs can be reduced without discouraging clinically necessary escalation. | Business | BR-02; clinicians and finance | Could objective in the working requirements; the 30% cost-reduction goal is unvalidated. Clinical adjudication and a comparator are needed. |
| AC-19 | Establish baseline measures, a prespecified evaluation protocol and reproducible cost capture before live use. | Transition | TR-03; evaluation, clinical and finance leads | Must proposal; define comparison, subgroup analysis, uncertainty, data ownership and review. |
| AC-20 | Update the three-year financial model using validated incremental costs and a plausible range of extrapolated benefits. | Transition | Case study KPI 3; finance and evaluation leads | Proposed decision-gate activity; distinguish pilot costs and outcomes from extrapolated scale economics. |

## Category summary

| Requirement type | Items | What the group captures |
|---|---|---|
| Business | AC-01, AC-10, AC-17, AC-18 | Desired clinical, privacy and financial outcomes; none is guaranteed by technology. |
| Functional | AC-02, AC-03, AC-04, AC-06, AC-07, AC-11, AC-12 | Alert, data, response, access and audit behavior. |
| Non-functional | AC-05, AC-08, AC-13, AC-16 | Proposed latency, reliability, security and controlled-change constraints. |
| Transition | AC-09, AC-14, AC-15, AC-19, AC-20 | Validation, readiness, training, governance and decision-gate activities. |


## Overview

**Central goal:** Evaluate whether AI-supported alerts and an accountable clinical response pathway can improve timely recognition and appropriate care without increasing harm, while establishing whether further investment is credible.

| Business — why the initiative matters | Functional — what the system or workflow does |
|---|---|
| AC-01: timely recognition and response without increased harm<br>AC-10: protect records and meet applicable obligations<br>AC-17: assess a credible investment case<br>AC-18: explore avoidable transfer cost reduction | AC-02: alert on approved criteria<br>AC-03: display context<br>AC-04: assign and escalate alerts<br>AC-06: integrate and correctly associate data<br>AC-07: signal missing or stale data<br>AC-11: restrict and log access<br>AC-12: maintain attributable audit records |
| **Non-functional — qualities and constraints** | **Transition — preparation and movement into evaluation** |
| AC-05: proposed alert delivery latency<br>AC-08: freshness, availability and safe failure<br>AC-13: privacy and security controls<br>AC-16: no automated retraining during baseline evaluation | AC-09: validate data and model; freeze version<br>AC-14: train and rehearse<br>AC-15: establish safety governance<br>AC-19: establish baseline, protocol and cost capture<br>AC-20: update the financial model at the decision gate |

## Traceability examples and unresolved decisions

| Objective | Enabling requirements | Verification / decision needed |
|---|---|---|
| Timely and safe response (AC-01) | AC-02–05, AC-06–09, AC-14–15 | Test qualifying alerts, ownership and missing-data fallback. Measure technical latency separately from clinical response and appropriate action. Review harms, missed events and alert burden. |
| Protect records (AC-10) | AC-11–13 | Test authorized and unauthorized access, log retrieval and incident procedures; complete applicable privacy, security and legal review. |
| Credible investment assessment (AC-17–18) | AC-19–20, supported by clinical and operational evidence | Clinically adjudicate avoidable transfers, capture incremental costs and compare plausible scenarios. Do not infer causality from raw transfer counts. |

- **Timing:** the proposed ≤5-minute technical target runs from the last required EHR data becoming available to a visible alert. The baseline clinical metric is median time from alert delivery to first documented doctor contact, with illustrative bands of ≤10, >10–30 and >30 minutes. A later ≤20-minute doctor–patient contact proposal is unreconciled; clarify population, episode, statistic and denominator. None is a validated clinical standard.
- **Alert burden and safety:** distinguish independently reviewed nonactionable alerts per 100 occupied patient-days from false positives and staff minutes. Specify review and denominators; review false negatives, workload, subgroup outcomes and safety pause criteria.
- **Financial evidence:** the hypothetical undiscounted three-year base case is **−44.6% ROI**; the −12% figure in a later exercise has no documented bridge. Reconcile scope, costs, benefits and horizon before comparison. Do not claim a positive pilot ROI or treat the 30% target as validated.
- **Approval and feasibility:** define accountable owners, acceptance tests, resource availability, data access, applicable approvals and safe fallback before live use. EHR modernization does not automatically require replacement. A financial dashboard is excluded from the baseline pilot; reproducible financial analysis remains required.
