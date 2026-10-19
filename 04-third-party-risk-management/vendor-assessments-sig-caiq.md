# Vendor Assessments: SIG and CAIQ

## 1. Quick concept

Standardized questionnaires gather consistent information about supplier security practices. The **Standardized Information Gathering (SIG)** questionnaire is associated with Shared Assessments; the **Consensus Assessments Initiative Questionnaire (CAIQ)** is associated with the Cloud Security Alliance's Cloud Controls Matrix (CCM). Use the latest applicable version from official sources and validate what the version is intended to do.

Sources: [Shared Assessments SIG](https://sharedassessments.org/sig/) and [CSA Cloud Controls Matrix and CAIQ v4.1](https://cloudsecurityalliance.org/artifacts/cloud-controls-matrix-v4-1). CSA published CCM/CAIQ v4.1 in January 2026; confirm whether the variant fits your service and desired use.

## 2. SIG vs. CAIQ

| Tool | Typical fit | Practical note |
|---|---|---|
| SIG | General third-party risk assessment across common risk domains | Tailor the questionnaire to vendor tier and service; current product materials may require access/licensing |
| CAIQ | Cloud-service security transparency mapped to CSA CCM | Confirm version, intended use, and compatibility with the desired CSA STAR pathway |

Questionnaires provide structured assertions, not independent verification. Review them against the vendor service scope and corroborate important answers with suitable evidence.

## 3. Workflow

1. Determine inherent risk and identify the vendor service being assessed.
2. Choose an appropriate questionnaire and version.
3. Give the vendor clear scoping context and a response deadline.
4. Review “yes” claims, unexplained “not applicable,” blanks, contradictions, and high-risk exceptions.
5. Request evidence for material controls (policy, report extract, test summary, process description).
6. Reconcile answers with assurance reports, contract terms, architecture, and service dependencies.
7. Record findings, assign owners, agree remediation/compensating controls, and set dates.
8. Make a documented business decision and define monitoring triggers.

## 4. Example

A vendor answers “Yes” to quarterly access reviews. Ask for the control description, scope, latest completed review, remediation evidence, and whether privileged access is included. If the vendor cannot share a specific artifact for confidentiality reasons, discuss an appropriate alternative such as an auditor report or controlled review; do not assume the control exists.

## 5. Common pitfalls

- Treating every question as equally important regardless of risk.
- Using an outdated questionnaire without checking edition.
- Asking for evidence irrelevant to the vendor's service or tier.
- Confusing lack of evidence with proof a control does not exist; record the limitation accurately.
- Accepting “yes” while ignoring contradictory exceptions or contract gaps.

## 6. Interview questions

**Q: A vendor leaves critical questions blank. What do you do?** Check applicability, follow up with targeted clarification, request alternative evidence, assess potential impact, and hold or condition approval if needed. Document the gap and decision authority.

**Q: Is a questionnaire enough for a critical cloud vendor?** Usually not on its own. Use a risk-based combination of questionnaire, independent assurance report, exception review, contract/privacy review, resilience evidence, and ongoing monitoring.
