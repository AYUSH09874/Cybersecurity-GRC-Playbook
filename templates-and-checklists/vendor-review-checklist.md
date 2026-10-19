# Third-Party Security Review — Starter Checklist

> Tailor the depth of review to the supplier's service criticality, data sensitivity, access, hosting model, and business dependency. A completed questionnaire is an input to risk analysis, not an automatic approval.

## 1. Intake and inherent risk

- [ ] Business sponsor, service description, legal entity, and intended use identified.
- [ ] Data types, data subjects, sensitivity, volume, and processing locations documented.
- [ ] Access model understood: public API, SSO, admin access, network integration, support access, or no access.
- [ ] Business criticality, recovery expectations, outage impact, and alternatives assessed.
- [ ] Subprocessors, hosting providers, and material dependencies identified.
- [ ] Data retention, deletion, portability, and exit needs understood.
- [ ] Inherent-risk tier assigned under the approved methodology.

## 2. Assurance materials

- [ ] Current SOC 2 Type II report or other relevant independent assurance reviewed where available.
- [ ] Report period and service/system scope match the service being purchased.
- [ ] Auditor opinion and any qualifications/exceptions reviewed.
- [ ] Complementary user entity controls (CUECs) identified and assigned internally.
- [ ] Subservice organizations and inclusive/carve-out method understood.
- [ ] Bridge letter or management statement considered if there is a gap since report end; it does not replace independent assurance.
- [ ] ISO 27001 certificate validity, certification scope, and accredited certification body checked if supplied.
- [ ] SIG, CAIQ, or other questionnaire responses reviewed for completeness, consistency, and evidence.
- [ ] Penetration-test summaries, remediation status, vulnerability management, and incident history reviewed according to risk and availability.

## 3. Control domains to assess

- [ ] Governance, security policies, assigned roles, and independent assurance.
- [ ] Identity, authentication, MFA, privileged access, and access recertification.
- [ ] Encryption, key management, data segregation, and secure deletion.
- [ ] Secure development, change management, vulnerability handling, and patch SLAs.
- [ ] Logging, detection, incident response, and customer notification commitments.
- [ ] Business continuity, disaster recovery, backups, and tested recovery objectives.
- [ ] Privacy obligations, international transfers, data-subject support, and processing terms where relevant.
- [ ] Workforce screening, training, and access termination.
- [ ] Subprocessor governance, flow-down requirements, and change notifications.
- [ ] AI-specific controls, data use, model training/retention, prompt/data leakage, and tenant separation where AI services are used.

## 4. Contract and approval

- [ ] Security/privacy addendum, confidentiality, breach notification, audit/assurance rights, and remediation commitments reviewed by authorized teams.
- [ ] Availability, support, recovery, and service-level obligations align to business needs.
- [ ] Data location, return/deletion, retention, and termination assistance are defined.
- [ ] Open findings have owners, dates, compensating controls, and acceptance authority.
- [ ] Business owner, Security, Privacy/Legal, Procurement, and risk approver sign off as required.
- [ ] Residual risk decision is recorded and justified; high risk is escalated under policy.

## 5. Ongoing monitoring and offboarding

- [ ] Reassessment date and event-based triggers scheduled.
- [ ] Assurance-report renewal and critical security notifications tracked.
- [ ] Changes in ownership, service scope, incidents, subprocessors, or hosting locations trigger review.
- [ ] Open remediation commitments are tracked to evidence-backed closure.
- [ ] At termination, access is revoked, data is returned/deleted as agreed, and records are retained per policy.

## Decision summary

| Field | Entry |
|---|---|
| Supplier / service |  |
| Inherent-risk tier |  |
| Review date / reviewer |  |
| Key strengths |  |
| Gaps / exceptions |  |
| Required remediation and due dates |  |
| Residual risk and rationale |  |
| Decision | Approve / approve with conditions / defer / reject |
| Approver / next review |  |
