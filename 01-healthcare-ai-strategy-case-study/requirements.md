# AI-Assisted Requirements, Activity Plan and Risks: Healthcare AI Case

## Sponsor overview and evidence status

This working draft adapts the AI-assisted planning exercise to the **hypothetical 300-bed German hospital** considering AI-supported clinical deterioration prediction. The existing case proposes a supervised **12-week evaluation on two internal medicine wards**, with comparison wards and a prespecified protocol. Patient-facing use is conditional on clinical, technical, safety, privacy, legal and funding readiness. 

## 1. Categorized requirements overview

Business items describe intended outcomes; functional items describe what the system or workflow does; non-functional items describe quality or constraints; transition items cover preparation and evaluation. Source IDs below are working requirements from the supplied documents, not newly approved specifications.

| Type | Requirement or objective | Source / status and measure or open question |
|---|---|---|
| Business | Support timely recognition and appropriate clinical response without increasing harm. | BR-01, Must objective; evaluate response and safety rather than assuming benefit. |
| Business | Protect patient records and meet applicable data protection obligations. | BR-03, Must objective; applicability and controls require local review. |
| Business | Explore whether avoidable ICU transfer costs can be reduced. | BR-02, Could objective; the 30% cost-reduction target is unvalidated. Appropriate escalation takes priority. |
| Business | Assess whether a sustainable investment case is credible. | Case study financial objective; update the three-year model, not a claim of positive pilot ROI. |
| Functional | Display a qualifying alert to the responsible authorized team when required valid EHR inputs support risk above the approved threshold. | FR-01, Must proposal; threshold and ownership require approval and validation. |
| Functional | Show authorized staff relevant inputs, timestamp and appropriate risk context. | FR-02, Must minimum; richer explanation is Should and must not imply causality. |
| Functional | Provide alert ownership, acknowledgement, visible status and backup escalation. | Case study R3, Must proposal; test no-response and handover scenarios. |
| Functional | Restrict patient-specific records, alerts and context by authorized role and log access attempts. | FR-03, Must proposal; test permitted and denied access. |
| Functional | Signal missing or stale required inputs and follow the approved fallback rather than giving misleading reassurance. | Working negative acceptance test; exact behavior and tolerances remain to be specified. |
| Functional | Record alert, assessment, action and disposition safely in the patient record through an approved workflow. | Case study R5, Must minimum; automated integration is Should if a safe tested alternative exists. |
| Non-functional | Make a qualifying alert visible within five minutes of required data availability in the EHR. | NFR-01, draft target subject to clinical and technical approval; measure delivery and EHR delays separately. |
| Non-functional | Define and test availability, security, freshness and safe failure behavior. | NFR-02; safe fallback is Must, numeric availability and freshness targets unresolved. |
| Non-functional | Freeze and version the model for evaluation and control any changes. | Case study R8 / TR-01; automated retraining is excluded during the baseline pilot, while approved controlled changes require review. |
| Transition | Validate local data mapping and model performance before live use. | TR-01, Must proposal; retrospective validation and prospective evaluation are distinct. |
| Transition | Train staff and rehearse response, escalation and fallback. | TR-02, Must proposal; define role-specific readiness and coverage. |
| Transition | Establish baseline, evaluation protocol and cost capture. | TR-03, Must proposal; prespecify comparison, outcomes, uncertainty and subgroup analysis. |
| Transition | Review safety, privacy, security, applicable approvals and funding before live use. | Case study decision conditions; identify accountable decision makers and applicable local requirements. |

## 2. Proposed activity timeline

Durations are **illustrative planning estimates**, not case commitments. Weeks below show a hypothetical sequence from project initiation; work can overlap only where dependencies allow. The actual pilot remains 12 weeks. 

| Phase / activity | Illustrative timing and duration | Dependencies and output |
|---|---|---|
| Planning: appoint leads, confirm funding, scope, stakeholders and governance | Weeks 1–2; 2 weeks | Sponsor mandate; named clinical, safety, IT, evaluation, privacy and finance owners and decision rights. |
| Planning and design: baseline and evaluation protocol | Weeks 2–4; 3 weeks | Initial scope and clinical participation; define eligible episodes, comparison wards, endpoints, subgroup analysis, cost capture and stop criteria. |
| Design: clinical workflow, safety and legal assessment | Weeks 2–5; 4 weeks | Named clinical and safety leads; define intended use, alert ownership, escalation, privacy and applicable approvals. Review runs alongside protocol design. |
| Technical preparation: data mapping, interfaces and configuration | Weeks 4–9; 6 weeks | Access to source systems and agreed design; validate identity, units, timestamps and data availability. Targeted EHR upgrades only as justified. |
| Testing and local model validation | Weeks 7–10; 4 weeks | Mapped data and available model; test performance, feeds, access, alert delivery, stale data and fallback. Rework can extend this phase. |
| Transition: training, simulations and readiness review | Weeks 9–11; 3 weeks | Clinical pathway and sufficient test results; rehearse response and downtime, confirm staffing, finance and applicable approvals. |
| **Gate: decision on patient-facing evaluation** | End of week 11; decision point | Proceed only when required safety, technical, clinical, governance, legal and funding conditions are met. An unresolved safety gate means stop. If not ready, remediate and reassess; no automatic launch. |
| Supervised evaluation, if approved | Weeks 12–23; 12 weeks | Readiness gate passed; monitor incidents, alert burden, clinical response, workload, subgroup outcomes and costs against the protocol. Pause for safety triggers and return to usual care. |
| Evaluation and decision on next steps | Weeks 24–26; 3 weeks | Completed or stopped evaluation and available evidence; analyze uncertainty, update three-year scenarios and decide whether further evaluation or investment is justified. |

A pilot is an investment in learning. Hospital-wide deployment requires a separate decision and is not an assumed next phase. Maintain the clinical and safety authority to stop or pause immediately throughout live use.

## 3. Principal risk list

Probability and impact are provisional **Low / Medium / High** qualitative estimates for planning, not measured probabilities. Owners should validate them and define triggers and escalation thresholds before use.

| Risk | Probability | Impact | Potential response |
|---|---|---|---|
| Missed deterioration or misleading predictions delay essential care. | Medium | High | Validate locally, retain clinical oversight, independently review false negatives and pause for predefined safety events. |
| Excessive or nonactionable alerts overwhelm staff or lead to ignored alerts. | Medium | High | Set clinically approved thresholds, measure independently reviewed nonactionable alerts and workload, and adjust or pause under governance. |
| Missing, stale, incorrectly mapped or wrong-patient data generate unsafe output. | Medium | High | Validate source-to-display identity and mappings, monitor freshness and test failure signaling and fallback. |
| Alert delivery, system downtime or unowned handovers delay a response. | Medium | High | Test latency, coverage, acknowledgement, backup escalation and downtime drills before live use. |
| Privacy or security failure exposes patient information. | Medium | High | Apply and test role-based access, audit logs, security controls and incident escalation with local privacy review. |
| Biased, underpowered or poorly compared evaluation produces misleading conclusions. | Medium | High | Prespecify comparison, subgroup and uncertainty analyses and avoid causal claims from raw counts. |
| Training gaps and additional workload undermine safe adoption or equitable care. | Medium | High | Involve nursing, physicians and patient representatives, rehearse across shifts and measure staff time and subgroup outcomes. |
| Approvals, procurement or integration dependencies delay the proposed schedule. | Medium | Medium | Identify accountable owners and applicable requirements early, track dependencies and replan before committing to dates. |
| Benefits or costs prove less favorable than assumed. | Medium | High | Capture incremental costs, validate effect assumptions and maintain separate pilot and extrapolated three-year scenarios. |
| Uncontrolled model or configuration changes invalidate evidence or alter risk. | Medium | High | Freeze and version the model, monitor performance and require review, validation and approval before any change. |

## Measures and decision cautions

The proposed **≤5-minute** system-latency criterion measures time from required EHR data availability to visible alert; it is distinct from clinical response. The case's clinical baseline uses median time from alert delivery to first documented doctor contact, with illustrative bands of ≤10, >10–30 and >30 minutes. A later ≤20-minute doctor–patient contact proposal remains unreconciled. None is a validated clinical standard; define population, episode, denominator and statistic before approval.

The case's **−44.6% three-year ROI** is an undiscounted hypothetical base case, not an observed pilot result. A later −12% figure has no documented bridge; reconcile scope, benefits, costs and horizon before comparison. Avoidable ICU transfers need clinical adjudication: reducing raw transfers can reflect unsafe delay, and timely alerts alone do not establish benefit.
