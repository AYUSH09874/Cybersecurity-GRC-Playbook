# Enterprise Risk Register — Starter Template

> **Purpose:** Capture risk decisions and monitor treatment. Tailor the scoring model and approval thresholds to the organization's approved risk methodology.

## Scoring guidance

Use the organization's approved likelihood and impact scales. The example below uses a 1–5 ordinal scale and a simple `Likelihood × Impact` score only to illustrate mechanics. Do not present this multiplication as a statistically calibrated loss estimate or compare scores across teams unless the method is consistently defined.

### Example scales

| Score | Likelihood (example) | Impact (example) |
|---:|---|---|
| 1 | Rare | Negligible, localized impact |
| 2 | Unlikely | Limited disruption or cost |
| 3 | Possible | Meaningful service, privacy, or business impact |
| 4 | Likely | Major disruption, contractual or regulatory exposure |
| 5 | Almost certain | Severe enterprise-wide or existential impact |

## Risk register

| Field | Entry |
|---|---|
| Risk ID | `RISK-###` |
| Date identified / last updated | `YYYY-MM-DD` |
| Risk title | Short, specific title |
| Risk statement | Because **[cause/condition]**, **[event]** may occur, resulting in **[business impact]**. |
| Business process / asset / service |  |
| Risk category | Cybersecurity / privacy / availability / third party / compliance / operational / other |
| Inherent likelihood and impact |  /  |
| Existing controls | Identify controls and link to evidence or control IDs. |
| Control effectiveness / evidence confidence | Effective / partially effective / ineffective / not yet assessed; explain basis. |
| Residual likelihood and impact |  /  |
| Treatment | Mitigate / avoid / transfer or share / accept |
| Treatment plan and milestones | Named actions, deliverables, due dates, dependencies |
| Risk owner | Accountable business owner, not merely the person updating the spreadsheet |
| Action owner(s) | People responsible for specific tasks |
| Target date | `YYYY-MM-DD` |
| Status | Open / assessing / treating / awaiting decision / accepted / closed |
| Acceptance authority and date | Required where risk is accepted, based on policy thresholds |
| Review trigger / next review | Date plus material-change triggers |
| Linked controls, incidents, findings, vendors | IDs/links |
| Closure rationale | Evidence showing risk reduction or approved acceptance; do not close solely because a task was marked done. |

## Worked example (fictional)

| Field | Example |
|---|---|
| Risk ID / title | `RISK-017` — Privileged access to cloud production is not reviewed promptly |
| Risk statement | Because access reviews are performed manually and leaver updates rely on separate tickets, an obsolete privileged account may remain active, enabling unauthorized production changes or data access. |
| Business service | Customer-facing SaaS platform |
| Inherent rating | Likelihood 4 × Impact 5 = 20 (example ordinal score) |
| Existing controls | SSO, MFA, ticketed access requests, centralized audit logs; review frequency and completion evidence require validation. |
| Residual rating | Likelihood 3 × Impact 5 = 15 pending effectiveness testing |
| Treatment | Mitigate |
| Actions | Automate HR-to-IAM deprovisioning; enforce privileged MFA; complete quarterly access recertification; test a leaver sample. |
| Risk owner | VP Engineering |
| Action owner | IAM lead |
| Due date / status | `YYYY-MM-DD` / In progress |
| Decision | Do not claim residual risk has dropped until implementation and operating evidence are tested. |

## Review checklist

- [ ] The risk is written as cause → event → consequence.
- [ ] A business owner is accountable for the risk decision.
- [ ] Existing control claims have evidence, not only verbal assurances.
- [ ] Inherent and residual risk are clearly distinguished.
- [ ] Treatment options and timelines are realistic and funded.
- [ ] Risk acceptance follows the documented approval threshold and expiry/review rules.
- [ ] Linked incidents, audit findings, vendors, and controls are cross-referenced.
- [ ] The register is reviewed when material changes occur, not only on a calendar cadence.
