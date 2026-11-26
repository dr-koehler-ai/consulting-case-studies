# Business Analysis Matrix: Healthcare AI Strategy Case

## Purpose and business context

This matrix supports an initial strategic discussion for a **hypothetical 300-bed German hospital** seeking to improve care and operational performance through digital investment. It adapts the IBM Business Analysis Matrix to four opportunities already assessed in the healthcare AI case.

## Evaluation methodology

Each opportunity retains the case's existing scores on two dimensions:

- **Impact:** potential contribution to patient care, experience, operational performance, and strategic capabilities, from 1 (very limited) to 5 (very high).
- **Feasibility:** relative practicality of implementation given anticipated resources, integration, workforce, governance, and other constraints, from 1 (very difficult) to 5 (relatively feasible).

## Summary of scored opportunities

| Strategic opportunity | Impact | Feasibility | Matrix position |
|---|---:|---:|---|
| EHR modernization | 5/5 | 4/5 | High impact / high feasibility |
| AI-powered clinical deterioration prediction | 3/5 | 3/5 | Lower impact / lower feasibility |
| Telemedicine | 4/5 | 4/5 | High impact / high feasibility |
| Automated appointment scheduling | 4/5 | 4/5 | High impact / high feasibility |

## Impact × feasibility matrix

| Feasibility ↓ / Impact → | High impact (4–5) | Lower impact (1–3) |
|---|---|---|
| **High feasibility (4–5)** | EHR modernization (5, 4); telemedicine (4, 4); automated scheduling (4, 4) | No case opportunity assessed in this quadrant |
| **Lower feasibility (1–3)** | No case opportunity assessed in this quadrant | AI deterioration prediction (3, 3) |

## Critical rationale and feasibility caveats

- **EHR modernization — 5 / 4:** Better access to reliable, interoperable clinical information could support multiple workflows and future digital initiatives. A feasibility score of 4 assumes an achievable scope and sufficient resources; legacy interfaces, data migration, cybersecurity, procurement, staff capacity, and downtime may make implementation harder. Modernization can mean targeted improvements to existing systems; a full EHR replacement is not assumed necessary.
- **Telemedicine — 4 / 4:** Remote consultations could improve access and convenience for appropriate services. Feasibility depends on clinical suitability, patient access and digital literacy, staff capacity, interoperability, privacy, reimbursement, and workflow design. Benefits and demand require local validation.
- **Automated scheduling — 4 / 4:** Scheduling could reduce administrative friction and improve access if the solution fits real booking processes. Integration, complex appointment rules, exception handling, accessibility, and maintaining non-digital access may limit benefits or raise costs.
- **AI deterioration prediction — 3 / 3:** Earlier identification of deterioration is a potential benefit, not an established outcome in this hospital. Data quality and availability, local clinical validation, alert burden, integration, human oversight, regulatory and approval readiness, and ongoing monitoring all affect feasibility. The case's **hypothetical, undiscounted three-year AI base-case ROI of −44.6%** (−€174,000 net benefit divided by €390,000 total costs) does not support an assumed positive financial return; clinical value and alternative scenarios also remain unvalidated. Clinicians retain responsibility for decisions.

## Ranking and decision implications

1. **Prioritize assessment and delivery of targeted EHR prerequisites** where they address confirmed needs and enable multiple initiatives. The 5/4 score indicates the strongest assessed impact, but investment and scope require a separate business case.
2. **Evaluate scheduling and telemedicine separately.** Both score 4/4, but serve different users and workflows. Compare each against its own baseline, costs, benefits, capacity, risks, and dependencies; their tied scores do not determine an order.
3. **Keep deterioration prediction conditional.** Its 3/3 placement and negative hypothetical AI base-case ROI argue against assuming a rollout or financial return. Consider only a capped, decision-gated evaluation after safety and applicable approval readiness are established.

## Dependencies and open validation items

| Area | Questions to validate before commitment |
|---|---|
| Clinical and operational baseline | What are current deterioration outcomes, appointment delays, administrative workload, access barriers, and relevant patient and staff needs? Which services and populations are in scope? |
| EHR and data | What capabilities already exist? Are data quality, timeliness, access, interoperability, and interfaces adequate? Which targeted upgrades are necessary for each opportunity? |
| Safety and governance | Who owns clinical safety, decisions, escalation, incidents, oversight, and monitoring? For AI, can local validation, acceptable alert performance, and workflow safeguards be demonstrated? |
| Legal, privacy, and approvals | What privacy, security, procurement, medical-device and other applicable requirements and approvals apply to the actual solution and intended use? Obtain qualified local review. |
| Economics and delivery | What are the full implementation and recurring costs, staffing needs, benefits, funding, timelines, and opportunity costs? Reassess the AI ROI assumptions and sensitivity; establish separate business cases for the other opportunities. |
| Adoption and equity | Can staff and patients use each service effectively? Test accessibility, training needs, change capacity, and alternatives for people unable or unwilling to use digital channels. |
| Evaluation and decision gates | Define owners, measurable outcomes, budget and time caps, evidence thresholds, stop criteria, and a decision date before any conditional AI evaluation. |

### AI evaluation: requirements and unresolved definitions

The case proposes a **12-week pilot on two internal medicine wards**, with comparison wards and prespecified evaluation, only after clinical, technical, governance, and funding prerequisites are met. This is a proposed supervised patient-facing evaluation, not an approved or completed pilot. The working requirements below are proposals to be approved by the relevant owners, and are distinct from the four strategic opportunities scored above.

- **Safe data and model:** validate patient identity, data mapping, freshness, delivery, and local model performance; freeze and version the model; test missing-data signaling and fallback. Automated retraining is excluded during the baseline evaluation; controlled changes require review and approval.
- **Clinical response and access:** assign a responsible team, escalation and backup; provide relevant alert context; test role-based access, audit logs, and incident procedures. Train staff and rehearse the response and downtime pathways. A timely alert alone does not demonstrate patient benefit.
- **Measurement:** establish baselines, a protocol, comparison approach, resource and cost capture, subgroup analysis, and safety pause criteria. Review false negatives and false positives independently; assess workload and nonactionable alerts separately. Avoidable ICU transfers require clinical adjudication: a lower raw transfer count alone is not evidence of benefit.
- **Reconcile timing proposals:** the draft ≤5-minute system latency target runs from required EHR data availability to a visible alert; it is not clinical response time and requires clinical and technical approval. The baseline clinical measure is median time from alert delivery to first documented doctor contact, with illustrative bands of ≤10, >10–30, and >30 minutes. A later proposal of ≤20 minutes to first doctor–patient contact remains unreconciled; clarify population, episode, statistic, denominator, and threshold before adoption. None is a validated clinical standard.
- **Financial comparability:** keep pilot costs and the extrapolated three-year model distinct. The later −12% figure has no documented bridge to the −44.6% base case; do not compare or substitute it until scope, costs, benefits, and horizon are reconciled. The suggested 30% cost-reduction goal is unvalidated.

## Strategic recommendation

Start by validating the hospital's needs and prioritizing targeted EHR and data prerequisites that provide value in their own right or enable clearly justified initiatives. Assess automated scheduling and telemedicine as separate investments, with independently validated business cases and implementation plans. Consider a strictly budget- and time-capped AI deterioration prediction evaluation only once safety governance and applicable approval readiness are in place; proceed beyond it only if predefined clinical, operational, regulatory, and economic criteria are met. The hypothetical negative base-case ROI should remain visible in that decision.

This is an **illustrative, hypothetical case associated with Coursera IBM coursework**. 
