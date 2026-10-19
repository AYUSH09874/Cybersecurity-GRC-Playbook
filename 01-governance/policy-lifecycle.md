# Security Policy Lifecycle in Practice

## 1. Executive summary

A security policy states management's intent and mandatory expectations for protecting information. It translates risk and business decisions into direction employees and teams can follow. A policy is not a technical configuration and does not prove that a control operates.

In production, policy management is a controlled lifecycle: identify the need, assign an owner, draft, review, approve, publish, communicate, enforce, handle exceptions, and periodically review. Triggers include incidents, new systems, contract or legal changes, audit findings, and scheduled review dates.

## 2. Key components

| Component | Practical question | Artifact |
|---|---|---|
| Purpose and scope | Which people, systems, data, and entities are covered? | Policy |
| Ownership | Who maintains the document? | Policy inventory |
| Approval | Who has authority to approve? | Workflow / minutes |
| Supporting standard/procedure | What measurable rules and steps implement it? | Standard / runbook |
| Communication | How will staff know what changed? | LMS record / announcement |
| Exceptions | How is a justified deviation approved and time-limited? | Exception ticket |
| Review | How are stale rules identified? | Version history / review log |

## 3. Enterprise workflow

1. **Trigger:** a contract requires MFA, audit finds unclear access requirements, or a system migration changes controls.
2. **Scope and owner:** identify affected teams and appoint a person with authority to maintain the policy.
3. **Draft:** state intent, scope, requirements, responsibilities, exceptions, enforcement, and related documents.
4. **Review:** IT/SecOps checks feasibility; Legal/Privacy reviews commitments; HR considers workforce implications; business teams assess operational impact.
5. **Approve:** use the company's formal workflow; do not infer approval from a meeting invite or informal reaction unless governance explicitly permits it.
6. **Publish and communicate:** maintain one authoritative version and notify affected staff.
7. **Operate and monitor:** technical/process owners implement the policy; GRC tracks evidence and exceptions.
8. **Review or retire:** review on schedule and on material change; archive superseded versions.

### Example: Access Control Policy

A SaaS company requires MFA for workforce access to production and privileged administration. The CISO delegate owns the policy. Identity Engineering implements conditional access; IT manages workforce identities; HR triggers joiner/mover/leaver events; GRC samples access reviews and records exceptions. Evidence includes the approved policy, identity-provider configuration, review records, and a sample of termination tickets compared with account disablement timestamps.

## 4. RACI example

| Activity | GRC | Security / IT | Legal / Privacy | HR | Business owner / executive |
|---|---|---|---|---|---|
| Identify policy need | R | C | C | C | A |
| Draft policy | R | C | C | C | A |
| Validate technical feasibility | C | A/R | I | I | I |
| Approve policy | C | C | C | C | A |
| Publish and train | C | R | I | A/R for workforce training | I |
| Track exceptions and review | R | R | C | C | A for risk acceptance within delegated authority |

## 5. Day-to-day responsibilities and artifacts

Maintain a policy inventory with owner, approver, version, scope, review date, and links to standards. Send review reminders, record reasoned “no change” decisions, track training/communication, and verify exceptions contain rationale, risk owner, approval, compensating controls, expiry, and closure plan.

## 6. Common pitfalls

- Treating “policy exists” as proof staff follow it.
- Writing rules that no team can technically meet.
- Allowing exceptions to remain open indefinitely.
- Keeping multiple conflicting “final” copies.
- Reviewing only on an annual calendar while ignoring material change.

## 7. Interview cheat sheet

**Q: Difference between a policy and procedure?** A policy states mandatory expectations and management intent; a procedure describes the steps to meet them. A standard defines more specific requirements; a guideline recommends practices.

**Q: The policy is approved but the technical team says it is not implemented. What do you do?** Do not mark the control effective based on the document alone. Confirm scope and requirements, agree an implementation plan and due date with the owner, record the gap and risk, consider compensating controls, and escalate overdue remediation. Any interim exception needs an authorized risk approver and expiry.

## 8. Checklist

- [ ] Owner and approver named
- [ ] Scope, requirements, responsibilities, and exception path defined
- [ ] Technical and legal feasibility reviewed
- [ ] Authoritative version published; superseded copies controlled
- [ ] Communication evidence retained
- [ ] Review date and triggers set
- [ ] Exceptions have approval, rationale, controls, and expiry

## 9. References

- [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)
- [ISO/IEC 27001:2022](https://www.iso.org/standard/27001.html)
