# Stakeholder Register: Healthcare AI Pilot

## Project and document control

| Field | Working entry |
|---|---|
| Project | Clinical deterioration prediction evaluation |
| Organization | Hypothetical 300-bed German hospital |
| Scope | Proposed, supervised 12-week evaluation on two internal medicine wards, with comparison wards and a prespecified evaluation. Live use is conditional on clinical, technical, governance, legal and funding readiness. |
| Version | 1.1 — working draft |
| Date | 26 November 2026 |
| Owner | Project manager or designated project lead — **to be appointed** |
| Status | Illustrative stakeholder and responsibility proposals; not approved or validated |

## Purpose and approach

This register identifies people and groups who could influence, deliver, oversee or be affected by the proposed evaluation. It supports engagement and clarifies proposed responsibilities; it does not grant authority or approve live use. Names, reporting lines, decision rights, engagement arrangements and appointments must be confirmed with the hospital. Where a group is listed, a named representative and alternate should be recorded before launch. A person may represent more than one role if conflicts and capacity are managed.

The project evaluates whether an alert-supported pathway can improve timely recognition and appropriate response without increasing harm. The case does not establish clinical benefits or savings. The hypothetical three-year base-case ROI is −44.6%; the pilot is intended to reduce uncertainty, not demonstrate a positive pilot ROI.

## Stakeholder register

Influence and interest are **high (H), medium (M), or low (L)** judgments for engagement planning, not assessments of clinical authority. All stakeholders belong to the hypothetical hospital unless otherwise stated.

| ID | Stakeholder / position | Organization | Proposed project role and interests | Influence / interest | Engagement and comments |
|---|---|---|---|---|---|
| S1 | Executive sponsor / hospital management | Hospital | Sponsor the evaluation, secure resources and make the investment decision; interested in safety, value, affordability and delivery. | H / H | Decision gates and concise progress, risk and cost reports. Sponsor approval does not replace clinical, privacy or other required approvals. Name and funding authority to confirm. |
| S2 | Project manager / project lead | Hospital | Coordinate scope, schedule, dependencies, risks, stakeholder engagement and decision records. | H / H | Regular cross-functional meetings; maintain register and escalate blockers. Appointment and mandate to confirm. |
| S3 | Clinical lead / accountable physician | Hospital | Own clinical design, intended use, response pathway and clinical readiness; retain clinical accountability for patient care. | H / H | Co-design and approve clinical protocol and thresholds with nursing and safety leads; review safety signals. Named lead and delegated authority to confirm. |
| S4 | Ward physicians and rapid-response clinicians | Hospital | Assess patients, make and document clinical decisions, escalate as appropriate, and identify workflow effects. | M / H | Include in pathway design, simulation, training and regular feedback; maintain usual-care fallback. Clinical decisions remain with qualified clinicians. |
| S5 | Nursing lead and ward nurses | Hospital | Contribute bedside observations, data capture, alert response, escalation, handover and workload assessment. | H / H | Include in design and threshold setting, shift coverage, drills and weekly feedback. Named nursing representative to confirm. |
| S6 | Clinical safety / patient safety lead | Hospital | Coordinate hazard assessment, safety gates, incident review and pause/fallback procedures. | H / H | Review safety evidence and unresolved hazards before live use; ensure incidents and stop decisions are escalated. Formal authority to pause or stop must be established. |
| S7 | IT and clinical informatics lead | Hospital | Coordinate interfaces, patient identity, data mapping, freshness, access, delivery, cybersecurity and technical fallback. | H / H | Interface tests, source-to-display reconciliation and downtime drills; report readiness and failures. Technical ownership and resources to confirm. |
| S8 | Data science / evaluation lead | Hospital or appointed partner | Design and carry out local validation and prespecified evaluation; monitor model performance, subgroups, alert burden and uncertainty. | M / H | Agree protocol and independent review arrangements with clinical and safety leads. Freeze and version the model; no automated retraining during the baseline evaluation. |
| S9 | Privacy, information security and legal / regulatory leads | Hospital and, where appropriate, external advisers | Assess applicable data protection, security, intended-use and regulatory obligations; advise on permissions, contracts and approvals. | H / H | Consult early and document applicable reviews, role-based access, logs and incident processes. Separate owners and approval rights must be identified; external advice does not replace hospital accountability. |
| S10 | Finance / controlling lead | Hospital | Capture incremental evaluation costs and update the reproducible three-year business case. | H / M | Agree cost scope, assumptions, scenarios and decision reports; distinguish evaluation costs from extrapolated scale economics. |
| S11 | Patients and patient representatives | Hospital patients and representative bodies | Experience potential benefits, harms, access and privacy impacts; contribute patient perspectives to information and evaluation. | M / H | Involve representatives in accessible communication, acceptability, equity and subgroup review; confirm appropriate representation and feedback routes. Patients retain their usual rights and clinical care arrangements. |
| S12 | AI vendor / solution provider | External supplier, if selected | Provide product, documentation, integration support, performance information and agreed maintenance. | M / H | Due diligence, contract and service-level discussions; verify intended use, evidence, change control and responsibilities. Vendor claims require independent assessment. No vendor is assumed selected. |
| S13 | EHR vendor / integration partner | External supplier, if needed | Support existing-system interfaces, data mapping, compatibility and recovery arrangements. | M / M | Confirm technical dependencies, access, costs, service responsibilities and test plans. Modernization may be targeted; full replacement is not assumed. |
| S14 | Training / change management lead | Hospital | Coordinate staff training, rehearsal, adoption support and feedback across shifts. | M / H | Agree training completion and competency evidence with clinical and nursing leads; cover escalation and fallback. Role may be combined with another named lead. |
| S15 | Works council / staff representation | Hospital, where applicable | Represent staff interests relating to workload, working practices and workforce impacts. | H / H | Identify applicable consultation or participation rights early and agree an engagement plan; exact rights require local review. |
| S16 | Relevant regulators or supervisory authorities | External | Oversee applicable legal and regulatory obligations; may have notification or approval roles depending on the solution and intended use. | H / M | Identify actual authorities, requirements and contact route through legal/regulatory review. Do not assume a specific approval or authority applies. |

## Proposed RACI by decision or activity

**R** = responsible for doing or coordinating the work; **A** = accountable for the decision or completed result; **C** = consulted before the result; **I** = informed. Each row has one proposed A. Multiple R roles work together. A blank means no primary assignment in this draft, not exclusion from necessary communication. The sponsor and hospital must confirm these assignments and actual approval rights; RACI does not override professional duties or legal requirements.

| Activity or decision | S1 Sponsor | S2 Project lead | S3 Clinical lead | S4 Physicians | S5 Nursing | S6 Safety | S7 IT | S8 Evaluation | S9 Privacy / legal | S10 Finance | S11 Patients | S12 AI vendor | S13 EHR partner | S14 Training | S15 Staff reps | S16 Authorities |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Approve scope, budget and funding | A | R | C |  | C | C | C | C | C | R | C |  |  |  | C |  |
| Develop clinical protocol and response / escalation pathway | I | C | A | R | R | R | C | C | C |  | C | C |  | C | C |  |
| Validate data feeds, identity, interfaces and technical fallback | I | C | C | C | C | C | A/R | R | C |  |  | R | R |  |  |  |
| Design and execute local validation and evaluation protocol | I | C | A | C | C | C | R | R | C | C | C | C | C |  |  |  |
| Assess privacy, security and applicable regulatory obligations | I | C | C |  |  | C | R | C | A/R |  | C | C | C |  | C | C* |
| Deliver training and rehearse response and downtime | I | C | A | R | R | C | R | C |  |  |  | C | C | R | C |  |
| Recommend clinical safety readiness and pause / fallback criteria | I | C | A | C | C | R | R | C | C |  | C | C |  | C |  |  |
| Approve project funding and go-live decision after required reviews | A | R | C |  | C | C | C | C | C | C | I | I | I | I | C | C* |
| Review incidents and initiate the agreed safety response | I | R | A | R | R | R | R | C | C |  | I | C | C | I |  | I* |
| Update three-year financial model and investment scenarios | C | C | C |  | C |  | C | R |  | A/R |  | C |  |  |  |  |
| Decide whether to proceed to further evaluation or investment | A | R | C | C | C | C | C | C | C | C | C | C |  |  | C | C* |

\* Engage or notify an authority only where required or appropriate following local review; the project cannot assign statutory responsibilities through this matrix. **A/R** means the same role is accountable and responsible. Go-live is conditional on all applicable independent approvals and readiness gates; a sponsor cannot waive them. A safety concern must be escalated and acted upon immediately under the approved procedure, without waiting for a routine RACI decision.

## Stakeholder engagement plan

This plan translates the register into practical engagement actions for the proposed pilot. 
For this exercise, power and interest are **high (H) or low (L)**. Power reflects the role's possible ability to approve, delay or redirect the project, or materially affect safe delivery; interest reflects likely exposure to its outcomes or workload. Unlike the register's provisional three-level ratings, this working assessment uses the lab's two-level scale; medium register ratings are assessed individually here rather than automatically converted. Both ratings require confirmation. H/H calls for close collaboration; H/L for proportionate decision-focused engagement; L/H for active involvement and feedback; L/L for accessible, proportionate updates. Low power does not imply low importance or justify excluding a patient or staff voice.

**Style starting points:** analytical = evidence and metrics; structural = clear process, responsibilities and deadlines; conceptual = options and wider implications; social = dialogue and collaboration. These are formats to offer, not personal traits. **Commitment:** U = unknown; R = resistant; N = neutral; S = supportive; L = leading. “Leading” means actively contributing within an agreed mandate, not taking over clinical or regulatory authority. Current and target states must be reviewed with stakeholders.

| ID / stakeholder | Power / interest and rationale | Proposed style to test | Current → desired | Engagement strategy and proposed cadence / owner |
|---|---|---|---|---|
| S1 Executive sponsor | H / H — funding and project direction | Analytical | U → L | Agree decision gates, budget and risk appetite; share concise safety, cost and progress reports monthly and at decisions. **Owner:** S2. |
| S2 Project lead | H / H — coordinates delivery and escalation | Structural | U → L | Establish responsibilities, action log, dependencies and escalation routes; coordinate weekly. **Owner:** S1. |
| S3 Clinical lead | H / H — clinical pathway and readiness | Analytical | U → L | Co-design clinical protocol and stopping criteria; review evidence and unresolved safety issues at least biweekly and at gates. **Owner:** S2 with S6. |
| S4 Ward physicians / rapid response | H / H — decisions and response capacity affect safety and adoption | Social | U → S | Involve representatives from each shift in simulations, workflow design and feedback; check in during training and weekly during live use. **Owner:** S3. |
| S5 Nursing lead / nurses | H / H — bedside workflow and escalation affect safe delivery | Social | U → L | Co-design alerts, handovers and workload measures; rehearse across shifts and review feedback weekly during live use. **Owner:** S3 with S14. |
| S6 Clinical safety lead | H / H — safety review and escalation can affect go-live | Analytical | U → L | Maintain hazard and incident review, independent challenge, pause and fallback criteria; review before go-live and routinely during evaluation. **Owner:** S2. |
| S7 IT / clinical informatics | H / H — controls data feeds, integration and fallback | Structural | U → L | Agree technical ownership, interface tests, failure drills and readiness evidence; coordinate weekly and at gates. **Owner:** S2. |
| S8 Data science / evaluation | H / H — validation and evaluation evidence can change decisions | Analytical | U → L | Agree prespecified protocol, local validation, uncertainty and subgroup analyses; review progress biweekly and at decision gates. **Owner:** S3. |
| S9 Privacy / security / legal | H / H — required reviews may constrain or delay launch | Structural | U → S | Engage early on intended use, access, legal obligations and approval evidence; review at design changes and before launch. **Owner:** S2. Independent assessment is welcome. |
| S10 Finance / controlling | H / H — funding analysis informs investment decisions | Analytical | U → S | Agree cost capture and assumptions; reconcile the three-year model and scenarios monthly and at gates. **Owner:** S2. |
| S11 Patients / representatives | L / H — directly affected, though formal project authority is not assumed | Social | U → S | Invite representative feedback on safety, privacy, accessibility and communications before launch and at reviews; offer accessible channels and honor disagreement. **Owner:** S3 with S2. |
| S12 AI vendor, if selected | H / H — product evidence, support and change control can affect delivery | Structural | U → S | Agree evidence requests, intended use, support, version controls and issue escalation; meet during selection and regularly under any contract. **Owner:** S2 with S7. |
| S13 EHR partner, if needed | H / H — interface access and support may constrain delivery | Structural | U → S | Confirm interface scope, testing, recovery responsibilities and service commitments; meet during design and testing. **Owner:** S7. |
| S14 Training / change lead | L / H — directly involved in readiness, without assumed project approval authority | Structural | U → L | Co-design role-specific training and rehearsal, track completion and feedback across shifts; review weekly before go-live. **Owner:** S2 with S3 and S5. |
| S15 Works council / staff representatives, where applicable | H / H — applicable participation rights and workforce acceptance may affect implementation | Social | U → S | Identify rights early, consult on workload and change, and agree follow-up at milestones. **Owner:** S2 with S9. Support is not presumed. |
| S16 Relevant authorities, where applicable | H / L — statutory powers may affect the project; routine interest is not assumed | Structural | U → N | Identify applicable authorities and submit required information or notifications through the designated legal lead at legally relevant points. **Owner:** S9. Neutral denotes no assumed position, not a target to influence an independent decision. |

### Reflection, challenge and early warnings

The greatest *potential* engagement challenge is securing sustained participation across ward physicians and nurses while protecting their time and keeping alerts clinically useful. The work changes multiple shifts and introduces uncertain workload and safety risks; this is a planning hypothesis, not evidence that clinicians are resistant. Explore constraints through representative interviews, workflow observation and rehearsal before selecting interventions. Privacy and safety reviewers may also appropriately challenge readiness; a delay or refusal can be a necessary safeguard rather than an engagement failure.
