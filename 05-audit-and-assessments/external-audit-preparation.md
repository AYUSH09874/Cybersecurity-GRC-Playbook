# Preparing for an External Security Audit

## 1. Quick concept

External audit preparation makes the scope, process owners, records, and responses ready for an independent assessor. The goal is to demonstrate actual operation and disclose limitations and gaps honestly, not to stage a performance.

## 2. Preparation sequence

1. Confirm standard/criteria, legal entity, covered service, system boundary, period, report type, and auditor requests.
2. Reconcile scope to architecture, asset inventory, contracts, vendor dependencies, and prior reports.
3. Map each request to an accountable owner, source system, period, population, and evidence location.
4. Perform readiness checks of high-risk controls; never manufacture retrospective evidence.
5. Schedule walkthroughs and identify subject-matter experts and backups.
6. Confirm confidentiality, secure transfer, redaction, and retention rules.
7. Track requests and answer follow-ups with traceable responses.
8. Review draft findings for factual accuracy; provide documented responses and corrective actions.
9. Track remediation, retest, and lessons learned.

## 3. Example evidence-room layout

Use access-controlled storage and comply with auditor instructions.

```text
/audit-period/
  /00-scope-and-governance/
  /01-risk-and-soa/
  /02-policies-and-awareness/
  /03-identity-and-access/
  /04-change-and-vulnerability/
  /05-incident-and-continuity/
  /06-suppliers-and-privacy/
  /07-internal-audit-and-management-review/
  /08-findings-and-remediation/
```

Do not expose the evidence room publicly or place secrets in an evidence file.

## 4. Interview preparation

Control owners should explain what they do, how often, where records live, how exceptions work, and what happens when a control fails. Do not coach canned answers. A truthful explanation of an exception and its remediation is more defensible than an unsupported claim that everything always works.

## 5. Common pitfalls

- The audit request scope differs from the team's assumptions.
- Evidence has incorrect dates or misses the relevant system population.
- The control owner is unavailable and no backup knows the process.
- Screenshots cannot be interpreted or traced to a source.
- Findings recur because only the symptom was fixed.

## 6. Interview question

**Q: How would you manage 100 evidence requests?** Track unique IDs, criterion, scope/period, owner, due date, status, evidence link, reviewer feedback, and blockers. Prioritize high-risk dependencies, quality-check evidence before submission, communicate real blockers, and do not mark a request complete until it has been reviewed.
