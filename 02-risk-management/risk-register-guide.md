# Building and Maintaining a Risk Register

## 1. Quick concept

A risk register is a living decision-support record. It links a defined scenario to business impact, rating rationale, accountable owner, treatment, deadlines, and residual exposure. It is not just a list of audit findings, vulnerabilities, or remediation tasks.

## 2. Minimum useful fields

| Field | What to record |
|---|---|
| Risk ID / title | Stable ID and concise title |
| Scenario | Event + weakness/context + business consequence |
| Scope / asset / process | Product, data, service, vendor, or process affected |
| Existing controls | Controls operating now, with evidence references |
| Inherent risk | Before the specified controls, as defined by the method |
| Current / residual risk | After controls; describe what has been validated |
| Rating rationale | Why likelihood and impact received their values |
| Treatment | Mitigate, avoid, transfer/share, or accept |
| Action, owner, due date | Concrete tasks and accountable roles |
| Approval / acceptance | Approver and applicable authority |
| Review trigger | Date, incident, architecture/vendor change, or new obligation |

## 3. Good operating practices

- Define rating scales and approval thresholds.
- Maintain a risk record and link it to separate remediation tickets.
- Distinguish the risk owner from the task assignee when appropriate.
- Do not lower the rating just because a treatment is planned; reassess after implementation and testing.
- Record acceptance duration, rationale, compensating controls, and re-review trigger.
- Report overdue high risks, accepted risks nearing expiry, repeated control failures, and concentrations of exposure—not only total risk count.

## 4. Example risk statement

**Weak:** “MFA risk — high.”

**Better:** “Because a legacy administrator integration permits password-only authentication, an attacker who obtains the credential could access production configuration and disrupt customer service. Network restrictions reduce exposure but do not remove the credential risk. The IAM Lead will migrate the integration by [date]; until then, the platform owner has approved time-limited monitoring under the exception process.”

## 5. Interview questions

**Q: When can you close a risk?** After agreed treatment is implemented, relevant evidence is reviewed/tested, residual risk is reassessed, and the designated authority approves closure under the process. Closing a ticket alone is insufficient.

**Q: A business owner accepts a high risk. What do you check?** Confirm delegated authority, informed rationale, duration, compensating controls, and review triggers; check legal/customer constraints; escalate if acceptance exceeds authority.
