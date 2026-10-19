# PBC Evidence Gathering and Management

## 1. Quick concept

PBC often means “Provided by Client” or “Prepared by Client,” depending on the audit engagement. Follow the engagement's own terminology. Evidence should support a defined assertion, come from an attributable source, match the scope and period, and be protected appropriately.

## 2. Evidence tracker fields

| Field | Purpose |
|---|---|
| Request ID | Unique identifier for follow-up |
| Criteria/control | Why evidence is needed |
| Requested artifact and period | Clear request plus date range |
| Population/scope | Systems, accounts, records, or transactions covered |
| Owner and backup | Primary supplier and alternate contact |
| Due date/status | Delivery tracking |
| Evidence location/version | Traceability to approved storage |
| Reviewer notes | Missing context or follow-up needed |
| Submission date/follow-up | Audit trail of delivery and questions |

## 3. Evidence quality checklist

- Is evidence from an approved system of record?
- Does it cover the period and defined population?
- Are filters, time zones, and exclusions clear when relevant?
- Does it show action/result rather than just a status label?
- Does it reconcile with supporting tickets, logs, or change records?
- Can a reviewer understand it without guessing?
- Is it redacted and transferred through an approved channel?

## 4. Example

A control owner uploads a screenshot reading “Quarterly access review: Completed.” GRC requests the underlying account population, reviewer decisions, reviewer identity/date, exception list, and tickets showing that unneeded access was removed. The screenshot can orient a reviewer, but it is not enough by itself to show what was reviewed and whether exceptions were actioned.

## 5. Confidential evidence

Use access-controlled repositories, least privilege, retention rules, and secure auditor transfer. Never upload live secrets, production credentials, unredacted personal data, or customer-confidential evidence to a public Git repository. If redaction removes necessary context, agree an authorized alternative with the auditor and owner.

## 6. Interview question

**Q: What if evidence is missing?** Do not fabricate or backdate it. Check whether another reliable source exists, document the gap, notify the control owner, assess impact, follow the audit/finding process, and track corrective action.
