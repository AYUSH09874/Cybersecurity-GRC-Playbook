# GDPR and Data Privacy Basics for GRC Analysts

## 1. Quick concept

The General Data Protection Regulation (GDPR) is an EU data-protection regulation governing personal-data processing within its material and territorial scope. It can apply to organizations established outside the EU in defined circumstances, such as offering goods/services to people in the EU or monitoring their behavior. Applicability is fact-dependent; Legal/Privacy should assess the actual organization, processing, and jurisdiction.

Official starting points: [European Commission — GDPR application](https://commission.europa.eu/law/law-topic/data-protection/information-business-and-organisations/application-gdpr_en) and [GDPR principles](https://commission.europa.eu/law/law-topic/data-protection/information-business-and-organisations/principles-gdpr_en).

## 2. Seven core principles

The European Commission describes seven principles: lawfulness, fairness and transparency; purpose limitation; data minimization; accuracy; storage limitation; integrity and confidentiality; and accountability. Accountability matters for GRC because organizations should be able to demonstrate compliance, not simply state that they are compliant.

Other practical concepts include controller/processor roles, lawful basis, data subject rights, records of processing, processor contracts, security of processing, breach response, international transfers, retention/deletion, and data protection impact assessments where required. This guide is not legal advice and does not cover every obligation.

## 3. Practical workflow

1. Inventory personal-data processing: data subjects, categories, purpose, systems, recipients, locations, retention, and suppliers.
2. Ask Privacy/Legal to confirm scope, roles, lawful basis, notices, and obligations.
3. Map technical and organizational controls: access, encryption, minimization, logging, deletion, backups, incident response, and supplier management.
4. Define request and incident workflows with deadlines and accountable owners.
5. Review processor contracts, data transfers, retention schedules, and vendor changes.
6. Maintain evidence: approvals, processing records, requests, training, tests, and remediation.
7. Reassess when purpose, data types, suppliers, processing locations, or risk changes.

## 4. Example: customer support data

A SaaS support platform stores names, work email addresses, support messages, and sometimes attachments containing sensitive information. GRC partners with Privacy, Product, Engineering, and Customer Success to map flows, restrict support access, define retention/deletion, confirm roles and contracts, and test request handling. A “GDPR compliant” checkbox is not enough; the organization needs a defensible account of actual processing and applicable obligations.

## 5. Common pitfalls

- Assuming an organization is exempt because it is not based in the EU.
- Treating pseudonymized or encrypted data as automatically anonymous.
- Collecting more data than the purpose needs.
- Retaining data indefinitely because deletion is inconvenient.
- Having a breach playbook that does not involve Privacy/Legal.
- Treating a security framework as a substitute for legal applicability analysis.

## 6. Interview questions

**Q: Is an IP address always personal data?** It can be personal data depending on whether it relates to an identified or identifiable person and the context. Assess the actual processing; do not assume every identifier is always personal or always anonymous.

**Q: A customer asks to delete their data. What does GRC do?** Follow the approved rights workflow, route the request to Privacy/Legal and system owners, locate relevant systems/processors, check applicable exceptions and retention duties, document actions and deadlines, and validate completion. GRC coordinates evidence but does not make a legal decision alone.

## 7. Further reading

- [European Commission — GDPR principles](https://commission.europa.eu/law/law-topic/data-protection/information-business-and-organisations/principles-gdpr_en)
- [European Commission — GDPR application](https://commission.europa.eu/law/law-topic/data-protection/information-business-and-organisations/application-gdpr_en)
- [Official GDPR text on EUR-Lex](https://eur-lex.europa.eu/eli/reg/2016/679/oj)
