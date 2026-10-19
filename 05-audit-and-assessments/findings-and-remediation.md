# Audit Findings, Root Cause, and Remediation

## 1. Quick concept

A finding records an evidence-based deviation from a defined criterion or another issue that the audit method requires reporting. A defensible finding connects the criterion, observed condition, evidence, and impact/risk. Root cause and corrective action should be validated rather than guessed.

## 2. Finding structure

- **ID/title:** stable identifier and concise summary.
- **Criterion:** policy, control requirement, contract, framework requirement, or audit criterion.
- **Condition:** what was observed and where/when.
- **Evidence:** source, population/sample, period, and references.
- **Risk/impact:** credible consequence, without unsupported claims.
- **Severity:** apply the approved method.
- **Root cause:** why the gap occurred, supported by analysis.
- **Correction:** immediate fix for the observed case.
- **Corrective action:** change intended to prevent recurrence.
- **Owner/due date:** accountable role, milestones, resources.
- **Retest/closure:** evidence of implementation and effectiveness, plus authorized closure.

## 3. Example

**Weak:** “Access controls are poor. Buy an identity tool.”

**Stronger:** “In a sample of 20 terminations from the in-scope application, two accounts remained active beyond the documented removal target. Evidence included the HR termination export and identity audit logs. The process does not consistently verify application-local accounts. An active former-worker account could allow inappropriate access. The IAM Lead and application owners will update offboarding checks, automate exceptions where feasible, and provide new-period sample evidence for retest.”

Do not claim an attacker used the accounts unless evidence establishes that fact.

## 4. Remediation lifecycle

1. Validate facts and criteria.
2. Contain immediate exposure where needed.
3. Identify root cause and contributing factors.
4. Define correction and preventive action.
5. Assign owner, resources, milestones, and target date.
6. Record interim risk and authorized exception if needed.
7. Validate implementation and operating effectiveness.
8. Close with evidence and approval, or escalate if the fix fails.
9. Analyze recurring themes across findings.

## 5. Common pitfalls

- Root cause is simply “human error.”
- Corrective action only reminds staff when workflow design contributed.
- Due dates are extended repeatedly without a risk decision.
- Finding closes when a document changes, with no retest.
- Severity changes informally to improve dashboard metrics.

## 6. Interview question

**Q: Difference between correction and corrective action?** Correction fixes the specific observed issue. Corrective action addresses the cause to reduce recurrence. Both may be necessary; a reviewer should validate effectiveness before closure.
