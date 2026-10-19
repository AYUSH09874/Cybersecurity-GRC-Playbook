# Audit Finding and Remediation Plan — Starter Template

## 1. Finding details

| Field | Value |
|---|---|
| Finding ID | `FND-###` |
| Title | Specific and outcome-focused |
| Assessment / framework |  |
| Date raised / source |  |
| Severity / priority | Per the organization's approved methodology |
| Accountable risk owner |  |
| Remediation owner |  |
| Target date |  |
| Status | Open / action agreed / in progress / pending validation / closed / accepted exception |
| Related risk / control / incident / vendor |  |

## 2. Finding statement

**Criteria:** What policy, contract, control design, or requirement should exist?

**Condition:** What was actually observed? Include sample and period where relevant.

**Cause:** Why did the condition occur? Separate root cause from symptoms.

**Effect / risk:** What could happen, and to which service, data, obligation, or business objective?

**Evidence:** Restricted evidence IDs and concise descriptions.

**Scope and limitations:** Which systems, sample, or period were and were not assessed?

## 3. Corrective action plan

| Action | Owner | Due date | Dependency | Completion evidence | Status |
|---|---|---|---|---|---|
| Immediate containment, if needed |  |  |  |  |  |
| Correct root cause |  |  |  |  |  |
| Address affected population / backlog |  |  |  |  |  |
| Update procedure / training / automation |  |  |  |  |  |
| Define ongoing monitoring |  |  |  |  |  |
| Validate effectiveness | Independent tester / authorized reviewer |  |  | Test results and evidence IDs |  |

## 4. Example (fictional)

- **Title:** Quarterly privileged access recertification did not cover two production platforms.
- **Criteria:** The approved access review standard requires quarterly review of all in-scope production platforms.
- **Condition:** The Q2 review evidence included the primary cloud account but omitted the disaster-recovery account and a managed database platform.
- **Cause:** The platform inventory used by the review owner was maintained manually and was not reconciled to the authoritative asset inventory.
- **Effect / risk:** Privileged access could persist without a periodic business-owner review, increasing the chance of unauthorized changes or data access.
- **Severity:** Set under the organization's approved methodology after evaluating exposure and compensating controls.
- **Corrective actions:** Reconcile inventory; complete a catch-up review; remove or document inappropriate access; automate population generation; add completeness attestation; independently retest the next cycle.
- **Closure criteria:** All in-scope platforms are reconciled; review decisions are traceable; exceptions have resolution evidence; a subsequent cycle demonstrates complete coverage. Merely publishing a new procedure is not sufficient.

## 5. Closure / acceptance gate

- [ ] Root cause is addressed, not just the individual symptom.
- [ ] Actions have completion evidence and a named owner.
- [ ] A qualified person independently validates design and/or operation, as appropriate.
- [ ] Residual risk has been reassessed.
- [ ] Any risk acceptance has an authorized approver, rationale, expiry/review date, and compensating controls.
- [ ] Risk register, control inventory, and reporting dashboard are updated.
- [ ] Closure is approved by the designated authority under the organization's methodology.
