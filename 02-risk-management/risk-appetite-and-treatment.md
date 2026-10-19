# Risk Appetite, Tolerance, and Treatment Decisions

## 1. Quick concept

Risk appetite is the broad amount/type of risk an organization is willing to pursue or retain while meeting objectives. Risk tolerance expresses acceptable variation around a particular objective or category. Thresholds turn these concepts into operational triggers. Organizations define terms within their own policy; wording and thresholds are not universal.

## 2. Treatment options

| Option | Meaning | Example |
|---|---|---|
| Mitigate / reduce | Change likelihood and/or impact | Enforce MFA, restrict access, test backups |
| Avoid | Stop the activity creating the risk | Delay a feature until safeguards are ready |
| Transfer / share | Allocate some consequences elsewhere | Insurance or contract terms; risk is not eliminated |
| Accept / retain | Authorized decision to live with residual risk | Time-limited acceptance with compensating monitoring |

## 3. Workflow

1. Identify the decision owner and appetite/tolerance statement.
2. Validate the scenario and residual exposure.
3. Compare feasible treatments, cost, timeline, dependencies, and downside.
4. Assign owner, milestones, success criteria, and evidence.
5. Record acceptance with approver, authority, rationale, scope, duration, compensating controls, and review trigger.
6. Escalate exposure above tolerance, authority, legal obligation, or customer commitment.
7. Reassess after implementation and testing.

## 4. Example

Engineering cannot upgrade a legacy integration before a customer migration. GRC documents the risk; Engineering explains the constraint; Security proposes monitoring and network restrictions; Legal checks contract implications; the business risk owner decides whether the exposure may be accepted for 45 days. The exception expires unless renewed by an authorized approver. GRC tracks replacement and verifies the new control before closure.

## 5. Pitfalls

- “We accept low risk” with no thresholds.
- Allowing any manager to accept any risk.
- Treating insurance as elimination of cyber risk.
- Accepting risk without expiry or reassessment triggers.
- Treating a legal/contractual requirement as optional because a score is low.

## 6. Interview question

**Q: A VP asks you to mark a high risk accepted immediately. What do you do?** Confirm the authority and threshold, explain the scenario/options, verify whether legal or customer obligations constrain acceptance, document rationale and compensating controls, capture duration and review trigger, and escalate if it exceeds policy. GRC must not fabricate approval or bypass governance.
