# Cybersecurity GRC Playbook — From Fundamentals to Enterprise Practice

A practical, open-source learning repository for students, freshers, and entry-level analysts entering **Cybersecurity Governance, Risk, and Compliance (GRC)**. It bridges concepts and frameworks with enterprise implementation: who does the work, what evidence is produced, what decisions need approval, and how control gaps are remediated.

> **Core principle:** a policy does not prove a control operates. Effective control assurance connects a risk, an owner, a repeatable process, operating evidence, exception handling, and review.

## Who this is for

- Students and career switchers learning GRC fundamentals.
- Junior GRC, risk, compliance, vendor-risk, and IT audit analysts.
- Technical analysts moving into control assurance or security governance.

## Learning outcomes

1. Turn business priorities into policies, standards, roles, and governance.
2. Identify, assess, treat, document, and monitor cyber risk.
3. Understand ISO/IEC 27001:2022, SOC 2, NIST CSF 2.0, PCI DSS, and GDPR basics.
4. Conduct risk-based third-party due diligence and assess vendor assurance evidence.
5. Prepare evidence for internal/external audits and track findings through retest.
6. Build practical artifacts: risk registers, control mappings, evidence trackers, workpapers, and remediation plans.

## Suggested learning path

| Stage | Study | Practical output | Completion signal |
|---|---|---|---|
| 0. Orientation | GRC concepts, basic IT/cloud, IAM, data handling | One-page map of a fictional SaaS service | Can distinguish governance, risk, compliance, and SecOps |
| 1. Governance | Policy lifecycle; policies vs standards vs baselines vs guidelines; awareness | Access-control policy plus approval record | Owner, scope, approver, review, exception path and evidence are clear |
| 2. Risk | NIST SP 800-30; FAIR; risk register; scoring; appetite/treatment | Five-row risk register | Each risk has a scenario, rationale, owner, treatment, due date and residual view |
| 3. Frameworks | ISO 27001; SOC 2; NIST CSF 2.0; PCI DSS; GDPR | Control map and evidence plan | Can explain framework boundaries and avoid treating them as interchangeable |
| 4. Third parties | TPRM; SIG/CAIQ; SOC 2 reports and bridge letters; monitoring | Vendor assessment and decision memo | Gaps and residual risk are evaluated, not hidden by questionnaire scores |
| 5. Audit | Internal audit; external audit prep; PBC; findings | One workpaper and remediation plan | Evidence is relevant, dated, scoped, traceable and sufficient for a conclusion |
| 6. Capstone | Combine the stages | Mini ISMS / audit-readiness pack | Artifacts are consistent and all decisions have accountable owners |

## Practical prerequisites

You do **not** need to be a penetration tester to begin. The following basics help: identity and access management (users, roles, MFA, joiner-mover-leaver); IT operations (cloud, endpoints, backup, change, incident response); software delivery (source control, code review, CI/CD); data classification and retention; concise business writing; and spreadsheets for tracking risks and evidence.

Use synthetic data in exercises. Never commit real customer records, credentials, vulnerability details, audit reports, confidential vendor responses, or production evidence into a public repository.

## Repository map

```text
.
├── README.md
├── ROADMAP.md
├── CONTRIBUTING.md
├── SECURITY.md
├── LICENSE
├── .gitignore
├── 01-governance/
│   ├── policy-lifecycle.md
│   ├── standards-baselines-guidelines.md
│   └── security-awareness.md
├── 02-risk-management/
│   ├── nist-sp-800-30.md
│   ├── fair-risk-analysis.md
│   ├── enterprise-risk-assessment.md
│   ├── risk-register-guide.md
│   ├── qualitative-vs-quantitative.md
│   └── risk-appetite-and-treatment.md
├── 03-compliance-frameworks/
│   ├── iso-27001-in-practice.md
│   ├── soc-2-trust-services-criteria.md
│   ├── nist-csf-2.0.md
│   ├── pci-dss-v4-0-1.md
│   └── gdpr-data-privacy-basics.md
├── 04-third-party-risk-management/
│   ├── tprm-lifecycle.md
│   ├── vendor-assessments-sig-caiq.md
│   ├── soc-2-bridge-letters.md
│   └── continuous-monitoring.md
├── 05-audit-and-assessments/
│   ├── internal-audit.md
│   ├── external-audit-preparation.md
│   ├── pbc-evidence-management.md
│   └── findings-and-remediation.md
└── templates-and-checklists/
    ├── README.md
    ├── standard-document-template.md
    ├── risk-register-template.md
    ├── evidence-request-list.md
    ├── control-test-workpaper.md
    ├── audit-finding-remediation.md
    ├── policy-template.md
    └── vendor-review-checklist.md
```

## How to use the repository

1. Read a topic's quick concept and write it in your own words.
2. Follow the implementation workflow and identify the accountable team for each step.
3. Complete the linked template using a fictional organization and realistic assumptions.
4. Ask whether another analyst could repeat the work from your notes and evidence references.
5. Practice explaining the result to both a technical control owner and a non-technical business owner.

## Important distinctions

- **ISO/IEC 27001** sets ISMS requirements; **ISO/IEC 27002** provides control guidance. **NIST CSF 2.0** organizes cybersecurity outcomes. **SOC 2** is an independent examination/reporting model based on selected Trust Services Criteria. **PCI DSS** applies to relevant payment-card environments. **GDPR** is a legal data-protection regulation whose application depends on processing and territorial scope.
- Certification, attestation, and self-assessment are different. Do not call a SOC 2 report a certification or claim ISO certification proves every system is secure.
- Evidence must match the assertion. A policy proves documented intent; it does not prove a quarterly access review took place.
- Risk acceptance is a business decision within delegated authority. GRC facilitates analysis and records the decision; it should not silently accept risk for the owner.

## Primary starting points

- [ISO/IEC 27001:2022 — official ISO page](https://www.iso.org/standard/27001.html)
- [ISO/IEC 27001:2022 Amendment 1:2024](https://committee.iso.org/standard/27001)
- [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)
- [NIST SP 800-30 Rev. 1](https://csrc.nist.gov/pubs/sp/800/30/r1/final)
- [AICPA SOC resources and Trust Services Criteria](https://www.aicpa-cima.com/topic/audit-assurance/audit-and-assurance-greater-than-soc-2)
- [PCI Security Standards Council — PCI DSS](https://www.pcisecuritystandards.org/standards/pci-dss/)
- [European Commission — GDPR principles](https://commission.europa.eu/law/law-topic/data-protection/information-business-and-organisations/principles-gdpr_en)
- [FAIR Institute — Learn FAIR](https://www.fairinstitute.org/learn-fair)
- [Shared Assessments — SIG](https://sharedassessments.org/sig/)
- [Cloud Security Alliance — CCM and CAIQ v4.1](https://cloudsecurityalliance.org/artifacts/cloud-controls-matrix-v4-1)

## License and safe contributions

Original repository documentation is licensed under [CC BY 4.0](LICENSE), except where stated otherwise. This does not license third-party standards or linked materials. Read [SECURITY.md](SECURITY.md) before filing security-related issues, and review your diff before committing. The `.gitignore` file helps prevent accidental evidence/secrets commits but cannot guarantee safety.

## Disclaimer

This repository is educational and is not legal advice, a certification opinion, or an audit opinion. Verify current editions, laws, contracts, regulator guidance, and auditor instructions before using it in a real engagement. Official standards may be copyrighted or require purchase; this repository summarizes application rather than reproducing their full text.
