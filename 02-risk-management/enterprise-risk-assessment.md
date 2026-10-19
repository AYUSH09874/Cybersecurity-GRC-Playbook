# Enterprise Cyber Risk Assessment — Worked Method

## 1. Executive summary

An enterprise cyber risk assessment helps leadership prioritize uncertainty that could affect organizational objectives. It is not simply a list of vulnerabilities or a technical scan: it considers services, assets, threat events, current controls, consequences, and treatment decisions.

## 2. Scope and preparation

Document the business objective, assessment boundary, in-scope services, locations, data, third parties, participants, methodology, scoring criteria, and approval route. Obtain architecture/data-flow views when systems or sensitive data are involved.

**Fictional example:** a 250-person SaaS company runs a customer-support platform in a public cloud. The assessment covers production hosting, identity, source-code/deployment workflows, customer data operations, support tooling, backups, and critical suppliers. A separate internal learning microsite is excluded only after documenting separation, confirming it does not support production or process in-scope customer data, and reviewing shared-control interfaces. Scope must not be narrowed just to hide a weakness.

## 3. Scenario design

Write the risk as: **Because of [event/weakness], [asset or process] may experience [consequence], resulting in [business impact].** Avoid vague entries such as “access risk — high.”

Example: “Because a terminated contractor's privileged account may not be disabled promptly, the account could be used to access production customer records, causing unauthorized disclosure and customer impact.”

## 4. Assessment workflow

1. Set scope and risk criteria.
2. Inventory important services, data, users, dependencies, and vendors.
3. Interview process owners and inspect technical/operational evidence.
4. Build plausible scenarios and document existing controls.
5. Estimate likelihood and impact under the approved scoring method.
6. Validate ratings with technical and business owners.
7. Choose treatment, assign owners and milestones, and record risk acceptance where applicable.
8. Report aggregate exposure, overdue actions, and themes to leadership.
9. Reassess on schedule and after incidents, major changes, new vendors, or obligation changes.

## 5. Example risk register entries

Ratings are illustrative; a real organization must define its own scales.

| ID | Scenario | Existing controls | Initial priority | Treatment | Owner | Due | Status |
|---|---|---|---|---|---|---|---|
| R-001 | Terminated privileged account retains access | HR ticket, monthly access review | High | Automate offboarding, alert on exceptions, test completion times | IAM Lead | 60 days | In progress; reassess after test |
| R-002 | Backup restore misses recovery objective | Daily backups; no recent restore test | High | Quarterly restore test, record RTO/RPO and corrective action | SRE Manager | 45 days | Pending validation |
| R-003 | Supplier changes subprocessor without review | Contract notification clause; annual questionnaire | Medium | Add change trigger and inventory check | TPRM Lead | 90 days | In progress |

## 6. Roles and governance

GRC manages the method and evidence trail. Technical owners explain the system and existing controls. Legal/Privacy assess obligations and impact. Procurement/TPRM manage supplier reviews. Finance supports business-impact estimates. Leadership sets appetite and accepts risk within delegated authority.

## 7. Day-to-day artifacts

Scope statement, stakeholder list, service/data inventory, scenario log, existing-control inventory, scoring rationale, risk register, treatment plan, risk-acceptance record, workshop notes, reporting dashboard, and reassessment trigger log.

## 8. Pitfalls

- Scoring a scanner finding without considering exploitability and business impact.
- Using inconsistent scales across business units.
- Closing a risk when only a task ticket closed and the control was not retested.
- Accepting risk without an authorized approver, duration, rationale, and compensating controls.
- Treating a one-time assessment as current indefinitely.

## 9. Interview questions

**Q: What makes a good risk statement?** It describes a plausible event, why it could happen, the affected asset/process, and the consequence to business objectives. It is specific enough to assign an owner and decide treatment.

**Q: Who owns a cyber risk?** Usually the accountable business or service owner owns the risk. Security and GRC advise, facilitate, and validate control information. The organization should define which roles may accept each risk level.

## 10. Further reading

- [NIST SP 800-30 Rev. 1](https://csrc.nist.gov/pubs/sp/800/30/r1/final)
- [NIST CSF 2.0](https://www.nist.gov/cyberframework)
- [FAIR Institute](https://www.fairinstitute.org/learn-fair)
