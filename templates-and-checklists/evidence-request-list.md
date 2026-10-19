# GRC Evidence Request List — Starter Template

> Use this tracker for internal control testing, certification readiness, customer assurance, or external audit requests. Align request wording and sample sizes with the agreed scope and assessor instructions.

## Evidence request tracker

| Field | Description / example |
|---|---|
| Request ID | `PBC-###` or `EVID-###` |
| Framework / control | Framework, clause/control ID, or requirement |
| Control objective | What risk the control is intended to reduce |
| Evidence requested | Specific report, record, configuration, minutes, or sample |
| Population / period | Defined population and date range; e.g., all production privileged users as of 30 September |
| Owner / contributor | Named accountable owner and evidence producer |
| Due date / status | Requested date; Not started / In progress / Submitted / Clarification / Accepted / Rejected |
| Secure repository link | Approved evidence location with least-privilege access; no secrets in the tracker |
| Reviewer / review date | Who checked and when |
| Result / gap | Accepted, incomplete, inconsistent, or not applicable—with rationale |
| Follow-up / issue ID | Actions, owner, due date, finding or risk ID |
| Retention / sensitivity | Classification and authorized retention period |

## Example request rows (fictional)

| ID | Requirement | Evidence requested | Scope / period | Owner | Acceptance criteria |
|---|---|---|---|---|---|
| PBC-001 | Joiner/mover/leaver access | Sampled approved access and termination tickets; corresponding IAM timestamps and account status | Sample period defined with auditor; include leavers and privileged users where in scope | IAM / HR Ops | Approval, appropriate provisioning/deprovisioning, timestamps, and traceable user identity are visible. |
| PBC-002 | Privileged access review | Dated review export, reviewer identity, decisions, and remediation tickets | In-scope systems and review period | System owners | Population is clear; reviewer has authority; exceptions are tracked to closure. |
| PBC-003 | Vulnerability management | Scan summary, severity, remediation due dates, exception approvals, and retest evidence | In-scope production assets and agreed period | SecOps / Platform | Asset coverage and aging are visible; overdue items have documented action or approved exception. |
| PBC-004 | Change management | Production change population, selected tickets, approvals, testing, and deployment evidence | Agreed audit period | Engineering / DevOps | Selected changes trace to authorization, test result, and deployment record. |
| PBC-005 | Incident response | Incident register, response procedures, tabletop results, and corrective actions | Relevant period | SecOps / Incident lead | Dates, ownership, disposition, and follow-up actions are consistent. |
| PBC-006 | Supplier assurance | Current assurance report or equivalent, scope, exceptions, complementary user entity controls, and bridge statement if applicable | Critical suppliers in assessment scope | TPRM / Procurement | Period and service scope cover reliance; gaps and subservice considerations are assessed. |

## Evidence quality gate

Before accepting evidence, confirm:

- **Relevance:** It proves the stated control objective and maps to the correct systems or process.
- **Period:** It covers the requested timeframe; a current screenshot may not prove past operation.
- **Completeness:** Population, filters, date range, and exclusions are visible or independently documented.
- **Authenticity:** Source, generation date, owner, and system are identifiable.
- **Integrity:** The artifact has not been altered in a way that changes its meaning.
- **Traceability:** A reviewer can follow the record to the underlying ticket, system, or approval.
- **Confidentiality:** Evidence is shared through an approved repository, appropriately redacted, and not committed to a public repository.

## Request email

**Subject:** Evidence request — `[control / assessment]` — due `[date]`

Hi `[owner]`,

For `[assessment and scope]`, please provide `[specific evidence]` covering `[population and period]` by `[due date]`. The evidence should show `[approval / completeness / timing / outcome required]`. Please upload it to `[approved restricted repository link]` rather than attaching sensitive exports to email. If the evidence is unavailable or the control changed during the period, note the reason and link any related issue or exception.

Thank you,
`[name / GRC team]`
