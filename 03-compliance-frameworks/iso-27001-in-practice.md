# ISO/IEC 27001:2022 in Practice — An Enterprise Implementation Guide

> **Document metadata**
> - **Category:** Compliance / Information Security Management System (ISMS)
> - **Audience:** Students, freshers, GRC analysts, control owners, audit coordinators
> - **Version reviewed:** ISO/IEC 27001:2022, with Amendment 1:2024 considered
> - **Last reviewed:** 2026-10-19
> - **Owner:** GRC Playbook contributors
> - **Status:** Educational working example

## 1. Executive Summary / Quick Concept

### What ISO/IEC 27001 is

ISO/IEC 27001 is an international standard that specifies requirements for establishing, implementing, maintaining, and continually improving an Information Security Management System (ISMS). The ISMS is the management system used to govern information-security risk—not merely a set of security tools or a folder of policies. It includes organizational context, leadership, planning, support, operations, performance evaluation, and improvement. Controls are selected and operated based on risk and the organization's stated scope.

The 2022 edition is the third edition of the standard. ISO published Amendment 1:2024, which adds climate-change considerations to the common management-system context and interested-party requirements. Organizations should assess whether climate change is a relevant issue in their context and recognize that interested parties may have climate-related requirements; the amendment does not mean every organization must invent a climate-specific information-security control.

Official references: [ISO/IEC 27001:2022](https://www.iso.org/standard/27001.html) and [Amendment 1:2024](https://committee.iso.org/standard/27001).

### Why it exists

Organizations hold information that matters to customers, employees, partners, regulators, and the business itself. ISO 27001 provides a structured, auditable way to understand information-security risks, decide how to treat them, assign responsibility, evaluate whether controls work, and continually improve the management system. It helps an organization demonstrate that information security is managed systematically, but it does **not** guarantee that breaches cannot occur or that every system is secure.

### What it is—and is not

- **It is:** a requirements standard for an ISMS that can be independently certified by a certification body.
- **It is not:** a prescriptive implementation recipe that says every organization must deploy the same product or configuration.
- **It is not:** the same thing as ISO/IEC 27002. ISO/IEC 27002 provides information-security control guidance; ISO/IEC 27001 sets ISMS requirements and references a control set in Annex A for consideration alongside risk treatment.
- **It is not:** a claim that an entire corporate group, every acquired business, every location, or every product is covered. The certificate has a defined scope.
- **It is not:** a SOC 2 report. A certification and an attestation report are different forms of assurance.

Organizations must obtain and consult the official standard for authoritative requirements. This guide summarizes practical implementation without reproducing the copyrighted standard text.

### A realistic mental model

Think of ISO 27001 as a continuous operating loop:

**Understand the business → assess risk → select treatment and controls → operate them → collect evidence → evaluate performance → fix gaps → repeat.**

A GRC analyst helps this loop function. They do not personally configure every technical safeguard. They coordinate owners, maintain the control/evidence trail, facilitate risk decisions, prepare assessments, and make sure claims are backed by evidence.

## 2. Key Domains / Components

### 2.1 Clauses 4–10: the management system

The following are plain-language summaries of the main clause topics. Use the official standard when interpreting a requirement.

| Area | What it means in practice | Typical artifacts and evidence | Frequent owner(s) |
|---|---|---|---|
| Clause 4 — Context of the organization | Understand the organization, interested parties, obligations, and the scope/boundaries of the ISMS. | Context analysis, interested-party register, legal/contract inventory, ISMS scope statement, service and data-flow diagrams | GRC, business owners, Legal/Privacy, Security |
| Clause 5 — Leadership | Leadership demonstrates commitment, establishes policy, and assigns roles and authority. | Approved information-security policy, role/authority matrix, steering committee minutes, resource decisions | Executive sponsor, CISO, GRC |
| Clause 6 — Planning | Address risks and opportunities, set information-security objectives, and plan changes. | Risk methodology, risk register, risk treatment plan, Statement of Applicability (SoA), objectives and measures | GRC, risk owners, Security, leadership |
| Clause 7 — Support | Provide resources, competence, awareness, communication, and controlled documented information. | Training records, competence matrix, communication plan, document register, controlled procedures | HR/L&D, GRC, team leads |
| Clause 8 — Operation | Run risk assessment and risk treatment processes as planned; control planned changes and relevant outsourced activity. | Operational procedures, change tickets, risk assessment records, treatment evidence, supplier records | Control owners, IT/Cloud/DevOps, TPRM, GRC |
| Clause 9 — Performance evaluation | Monitor, measure, analyze, evaluate, audit internally, and conduct management review. | KPI/KRI dashboard, monitoring outputs, internal audit plan/results, management-review inputs and minutes | GRC, Security, control owners, leadership, internal audit |
| Clause 10 — Improvement | Correct nonconformities and improve the ISMS based on results. | Findings log, root-cause analysis, corrective-action plan, retest evidence, continual-improvement log | Finding owner, GRC, relevant management |

**2024 context amendment:** verify and document whether climate change is a relevant context issue and whether interested parties have relevant climate-related requirements. The decision should be based on the organization's context. For a cloud-based SaaS provider, relevant continuity considerations might include regional disruption or supplier resilience where there is a credible business connection, rather than assuming climate change automatically changes every control.

### 2.2 Annex A controls: what they are used for

The 2022 Annex A reference set has **93 controls grouped into four themes**:

| Theme | Control count | Examples of the kinds of topics addressed |
|---|---:|---|
| Organizational | 37 | Policies, roles, threat intelligence, asset management, access control, supplier security, incident management, continuity, compliance |
| People | 8 | Screening where appropriate, employment terms, awareness, responsibilities on role change or termination, confidentiality |
| Physical | 14 | Physical access, secure areas, equipment protection, clear desk/screen, secure disposal |
| Technological | 34 | Endpoint controls, authentication, access rights, configuration, vulnerability management, logging, monitoring, backup, network and application security, secure development |

The numbers above describe the 2022 reference set; check the licensed official text for exact control wording. Annex A is not a universal “all controls must be implemented” checklist. The organization considers the reference controls while treating information-security risks, adds other controls as needed, and records the outcome in the SoA. If an Annex A control is excluded, the rationale should be consistent with the risk assessment, ISMS scope, and treatment decisions. A control that is not listed in Annex A may still be necessary for the organization's risk treatment.

### 2.3 The Statement of Applicability (SoA)

The SoA is one of the most important ISMS artifacts. In practice, it records the controls the organization determined necessary, the status or implementation information required by its process, and the justification for inclusion or exclusion. A well-maintained SoA allows an auditor or management reviewer to trace a decision from risk to treatment to control and evidence.

A useful internal SoA usually includes:

- Control identifier and concise internal description.
- Source / rationale: risk treatment, legal or contractual requirement, business need, or other obligation.
- Applicability decision and justification.
- Implementation status and control owner.
- Linked policy, standard, process, system, risk ID, and evidence location.
- Last reviewed date and planned validation cadence.

Do not copy “implemented” from a project plan without validating the deployed or operating state. If a control is still in progress, represent that honestly and link the gap or remediation record.

### 2.4 ISO 27001 vs. adjacent concepts

| Item | How to distinguish it |
|---|---|
| ISO/IEC 27001 | Requirements for the ISMS; can be used for certification |
| ISO/IEC 27002 | Guidance on information-security controls; not itself a certification standard |
| Risk assessment | Identifies and analyzes scenarios and risk to objectives |
| Risk treatment plan | Defines selected responses, actions, and ownership |
| SoA | Documents selected control applicability and related justifications/status |
| Internal audit | Independent, planned evaluation of whether the ISMS meets criteria and is implemented/effective within scope |
| Certification audit | Third-party assessment by a certification body against the standard and stated scope |

## 3. Real-World Industry Implementation

### 3.1 Fictional company and assumptions

**Company:** Northstar Support Cloud (fictional), a 250-person business-to-business SaaS provider.

**Service:** A multi-tenant customer-support platform hosted in a public cloud. Employees use a cloud identity provider, managed laptops, a source-code platform, CI/CD, a ticketing system, monitoring, and backup services.

**Drivers:** Enterprise customers ask for independent assurance; leadership wants a consistent risk process; the company is introducing a more formal security program.

**Proposed ISMS scope:** the people, processes, and technology used to develop, deploy, operate, and support the production SaaS service, including production cloud infrastructure, identity and privileged access, source control and deployment workflows, customer support operations that can access customer data, relevant backup/monitoring systems, and critical supplier dependencies.

**Scope exclusions:** the company has a separate internal learning microsite owned and operated by an unrelated function. It is excluded only after documenting its separation, confirming it does not support production operations or process in-scope customer data, and checking interfaces and shared controls. Corporate identity or endpoint controls that protect in-scope administrators cannot be casually excluded because those controls are shared with other activities. Scope must represent how the service actually works, not the smallest convenient boundary.

This is an illustrative scenario, not a recommended scope for every SaaS business.

### 3.2 End-to-end implementation workflow

#### Step 1 — Secure sponsorship and define the objective

The executive sponsor agrees why the ISMS is being established, what business services it supports, what resources are available, who makes decisions, and which customers or contracts create commitments. GRC prepares a short charter and governance cadence.

**Outputs:** ISMS charter, executive sponsor, implementation milestones, decision forum, initial stakeholder list.

**Real-world tip:** avoid starting with a control spreadsheet before the organization agrees on the service and boundary. A control list cannot resolve a disputed scope.

#### Step 2 — Understand context, interested parties, and obligations

GRC facilitates workshops with product, engineering, IT, customer success, Legal/Privacy, HR, Procurement, and leadership. The team documents business objectives, key services, data categories, dependencies, customer security clauses, relevant legal requirements, and expectations of interested parties.

**Evidence to request:** service diagram, data-flow diagram, asset/service inventory, data classification, contract register, privacy/data-processing inventory where appropriate, customer security commitments, supplier inventory, business continuity assumptions, organizational chart, and relevant risk committee minutes.

**Outputs:** context analysis, interested-party/obligation register, documented ISMS scope and boundaries.

Do not assume every law applies simply because a customer is overseas. Legal or Privacy should assess applicability and obligations based on actual facts.

#### Step 3 — Define the risk assessment method

The CISO/risk owner approves the organization's method before the team scores risks. Define likelihood and impact scales, the levels requiring leadership approval, treatment options, acceptance authority, reassessment triggers, and how residual risk is evaluated.

The method may be qualitative or quantitative, provided it is repeatable, fit for purpose, and used consistently. ISO 27001 does not require every organization to use the same 5×5 matrix.

**Outputs:** risk assessment procedure, scales/criteria, risk acceptance thresholds, risk register fields, escalation path.

#### Step 4 — Identify and assess risk scenarios

System owners and GRC discuss credible scenarios. Use technical evidence (identity configuration, cloud inventory, vulnerability reports, incident trends, backup restore tests, change records) alongside business context (service criticality, customer impact, recovery objectives, contractual commitments).

Sample risks for Northstar Support Cloud:

| Risk ID | Scenario | Existing control evidence to inspect | Example initial priority | Treatment direction |
|---|---|---|---|---|
| R-001 | A terminated contractor retains privileged access due to a delayed identity workflow, enabling unauthorized production access | HR termination tickets, identity logs, privileged account export, offboarding SLA report | High | Automate deprovisioning and alert on exceptions; test samples |
| R-002 | Backups cannot be restored to the required recovery objective during a cloud-region incident | Backup configuration, failed-job alerts, restore-test records, continuity plan | High | Define recovery objectives and run scheduled restore tests |
| R-003 | A production deployment bypasses required peer review because a service account can merge and deploy changes | Repository branch protection, access list, deployment logs, change tickets | High | Separate duties, limit service account permissions, monitor bypasses |
| R-004 | A critical support SaaS provider materially changes its subprocessor model without timely review | Contract terms, vendor inventory, SOC 2 report, subprocessor list, review notes | Medium | Add trigger-based re-review and contractual notifications |

Ratings are illustrative. They should be based on a defined scale, not copied into an actual register without analysis.

**Outputs:** risk scenarios, risk register, scoring rationale, treatment decisions.

#### Step 5 — Decide treatment and select controls

Risk owners decide which treatment is appropriate. GRC helps map treatment to controls and obligations; technical teams design and implement the control; Legal/Privacy advises on obligations; leadership handles exceptions above delegated authority.

For R-003, the treatment might include protected branches, named-person approvals, restrictions on service-account permissions, alerting on bypass, and periodic review. The control is not considered effective simply because a repository setting was configured once; the team should verify the relevant repositories remain protected and the exception workflow operates.

**Outputs:** risk treatment plan, control mapping, SoA, action tickets, approved exceptions where necessary.

#### Step 6 — Build and operate the ISMS processes

Develop only the policies, procedures, and records needed to meet requirements and manage the risks. Typical topics include information security policy, asset/data handling, access management, supplier security, incident management, vulnerability management, secure development, backup/continuity, change management, awareness, and corrective action.

Every documented process should have an owner, an expected cadence or trigger, a defined population/scope, an evidence source, and an exception route. Keep the process proportionate; more documents do not automatically mean better security.

**Outputs:** approved policies, operating procedures, control owner register, training plan, evidence repository, metrics.

#### Step 7 — Run internal audit and management review

Internal audit should be planned and performed with appropriate objectivity and independence. If a small company has GRC design a control, GRC should not be the only person independently declaring its own work effective; management should set safeguards or use a competent independent reviewer.

Internal audit evaluates the ISMS against defined criteria and scope, gathers evidence, records findings, and follows up. Management review considers matters such as changes in context, objectives, audit results, nonconformities, risk assessment and treatment status, monitoring results, interested-party feedback, and opportunities for improvement.

**Outputs:** internal audit plan, sampling/testing workpapers, findings, management-review agenda/minutes, decisions and actions.

#### Step 8 — Prepare for an independent certification audit

A certification body assesses the defined ISMS scope against ISO 27001. A typical initial certification process has a Stage 1 review of readiness and documentation/context, followed by Stage 2 assessment of implementation and effectiveness; the certification body establishes the specific plan and requirements. GRC coordinates logistics and evidence, while control owners explain and demonstrate operations.

The team should not manufacture retrospective evidence or coach employees to conceal gaps. If a required process did not operate, record the issue, determine impact, correct the underlying condition, and follow the auditor/certification body's finding process.

**Outputs:** scope and audit plan, evidence index, interview schedule, finding responses, corrective-action evidence, certification decision from the certification body.

#### Step 9 — Monitor and improve after certification

Certification is not a one-time project. Maintain the ISMS, reassess risk, operate controls, conduct internal audits and management reviews, resolve findings, and address changes. Certification bodies generally conduct surveillance and recertification activities on a cycle specified by their accreditation/program rules and contract; confirm the actual audit schedule with the certification body.

**Outputs:** recurring control evidence, updated risk register and SoA, audit calendar, performance dashboard, corrective-action log, and updated management decisions.

### 3.3 RACI matrix / cross-functional collaboration

R = Responsible (performs work); A = Accountable (owns the outcome); C = Consulted; I = Informed. This illustrative RACI must be aligned to actual roles and authority. Internal audit independence must be preserved.

| Activity | GRC / ISMS Manager | SecOps / Security Eng. | IT / Cloud / DevOps | Legal / Privacy | HR | Procurement / TPRM | Business owner / Leadership | Internal Audit |
|---|---|---|---|---|---|---|---|---|
| Define ISMS scope and context | R | C | C | C | I | C | A | I |
| Approve risk method and appetite | R | C | C | C | I | I | A | I |
| Identify and analyze technical scenarios | R | R | R | C | C | C | A for business risk | I |
| Choose / approve risk treatment | C | C | R for technical plan | C | C | C | A (risk owner / delegated executive) | I |
| Draft and maintain policies | R | C | C | C | C | C | A | I |
| Implement and operate cloud/access controls | C | C | A/R (as assigned) | I | I | I | I | I |
| Perform supplier due diligence | C | C | C | C | I | A/R | C / A for business decision | I |
| Conduct internal audit | C or support | C | C | C | C | C | I | A/R, with independence safeguards |
| Coordinate external audit evidence | A/R for coordination | R for owned evidence | R for owned evidence | C | R for owned evidence | R for owned evidence | I | C / independent role as applicable |
| Approve policy / accept out-of-threshold risk | R for advice and recording | C | C | C | C | C | A | I |
| Remediate and retest findings | C | R for owned control | R for owned control | C | R for owned process | R for owned process | A for resources / overdue escalation | Independent follow-up as appropriate |

One person may hold several roles in a small company. The organization should explicitly manage conflicts—for example, a control designer should not be the sole independent evaluator of the same control.

### 3.4 Control example: quarterly privileged-access review

**Objective:** confirm that privileged access is limited to authorized users with a current business need.

**Control design:** Each quarter, the application/platform owner reviews a complete export of privileged accounts and roles, confirms business justification, removes unneeded access through the normal ticket/change process, and records approvals and completion. A defined escalation process handles missing reviewers and overdue removals.

**What GRC asks for:**

1. Control description and owner.
2. Population source and extraction date (for example, identity provider and cloud-account inventory).
3. Evidence the population is complete and relevant to in-scope systems.
4. Review record showing reviewers, accounts/roles reviewed, decisions, dates, and exceptions.
5. Tickets or logs for access removals, plus completion timestamps.
6. Escalation evidence for overdue or disputed items.
7. Follow-up test showing the access change occurred and unauthorized access is no longer present.

**How it is tested:** select a period and in-scope population; inspect whether the review took place on schedule, whether the full population was reviewed, whether reviewers had appropriate authority, whether exceptions were resolved, and whether selected removals were completed. If evidence is incomplete, expand testing or record a limitation/finding according to the audit method. A screenshot of a dashboard with “review completed” is not enough if it cannot identify the population and decisions.

**Typical cross-team flow:** IAM exports accounts → platform owner reviews business need → IT opens/remediates access tickets → GRC tracks completion and samples evidence → management sees overdue exceptions → internal audit independently tests the process.

## 4. Day-to-Day Responsibilities & Artifacts

### 4.1 What an entry-level GRC analyst actually does

A junior analyst might spend a typical week doing the following:

- Update the control/evidence tracker and verify that a requested artifact covers the correct audit period, system, population, and owner.
- Follow up with a control owner when an evidence request is overdue or the attachment does not support the control claim.
- Review a policy due for renewal, compare it with actual process changes, coordinate comments, and route approval.
- Help maintain the risk register: check overdue actions, record decisions, verify treatment evidence, and prepare risk committee status.
- Map customer requirements to existing controls, identifying duplicates and genuine gaps rather than creating unnecessary parallel controls.
- Coordinate supplier assessments, track open questions, and route high-risk findings to the business owner.
- Prepare audit schedules, meeting notes, request lists, evidence indexes, and remediation dashboards.
- Record audit findings with criteria, condition, evidence, business impact, owner response, action, due date, and retest result.
- Prepare metrics such as control evidence completion, overdue corrective actions, high residual risks, overdue policy reviews, and supplier assessments past due.

### 4.2 Artifact catalog

| Artifact | Why it exists | What “good” looks like |
|---|---|---|
| ISMS scope statement | Defines the covered boundary | Specific service, people, processes, technology, interfaces, and reasoned exclusions |
| Context / interested-party register | Captures internal/external issues and expectations | Source, relevance, owner, review date, link to obligations/risks |
| Risk methodology | Ensures assessments are repeatable | Defined scales, criteria, acceptance thresholds, and reassessment triggers |
| Risk register | Records scenarios and decisions | Clear statements, owners, rationale, treatment, residual view, due dates |
| Risk treatment plan | Tracks chosen actions | Each action tied to risk/control, owner, milestone, test/evidence and status |
| Statement of Applicability | Explains selected controls and applicability | Inclusion/exclusion rationale and traceability to risks, obligations, status, owner |
| Policy register | Controls the policy lifecycle | Owner, approver, version, effective date, review date, publication link |
| Control register / matrix | Connects obligations and processes | Control objective, scope, operator, frequency, evidence, procedure, system |
| Evidence index / request tracker | Coordinates assessment support | Request ID, criteria, period, population, owner, status, location, reviewer comments |
| Internal audit program and workpapers | Shows planned independent assessment | Scope, criteria, test steps, sample basis, evidence, conclusion, reviewer |
| Management review record | Shows leadership evaluation and decisions | Inputs considered, decisions, owners, deadlines, follow-up |
| Nonconformity / corrective-action log | Resolves issues and prevents recurrence | Root cause, correction, corrective action, effectiveness test, closure approval |
| Metrics dashboard | Supports oversight | Defined calculation, source, owner, trend, thresholds and actions—not vanity counts |

### 4.3 Example evidence requests

Use requests that define scope, period, population, and acceptable proof. Avoid asking for “all security evidence.”

| Control topic | Example request | What to validate |
|---|---|---|
| Access termination | “For sampled in-scope terminations in Q3, provide the HR source date, identity disablement log, privileged account check, and exception ticket if completion exceeded the target.” | Date alignment, completeness of population, actual disablement—not only ticket closure |
| Vulnerability management | “Provide the monthly critical-vulnerability report for in-scope production assets, risk-based remediation SLAs, exception approvals, and retest/closure proof for selected items.” | Asset scope, severity, age, approved exceptions, validated closure |
| Change management | “For selected production changes in the period, provide the change ticket, risk/impact review, approval, test results, deployment log, and rollback details if used.” | Changes sampled from a complete source; evidence aligns with release timestamps |
| Backup and recovery | “Provide the latest scheduled backup status, most recent restore-test results for the in-scope service, recovery objective, failures, and corrective actions.” | A successful backup job is not the same as a successful restore |
| Security awareness | “Provide assigned population, completion export, role-based training coverage, and overdue follow-up for the period.” | Workforce source reconciles to training records and scope |
| Incident management | “Provide the incident register for the period, severity criteria, selected incident timeline, escalation, lessons learned, and corrective-action linkage.” | Selection completeness, timestamps, evidence of required steps, restricted handling |
| Supplier security | “For the critical supplier sample, provide the current assessment, assurance report and period, open exceptions, contract/security terms, and next review trigger.” | Correct service coverage, report type and dates, subservice organizations, gap decisions |

**Sensitive-evidence rule:** use approved repositories with access control and retention rules. Redact credentials, secrets, customer identifiers, personal data, and unrelated confidential information. Never commit real evidence into this public GitHub repository.

### 4.4 Reporting dashboard ideas

A useful executive dashboard may show high/critical residual risks by owner and age; overdue treatment actions; controls with failed or missing operating evidence; internal audit findings by severity, age and recurrence; policy reviews and mandatory training overdue; critical vendor assessments overdue; restore-test and recovery-objective exceptions; and evidence-request status during a defined audit window.

Every metric needs a definition, owner, source, cadence, threshold, and escalation path. A rising number of reported phishing messages, for example, can indicate improved reporting rather than deteriorating security.

## 5. Common Pitfalls & Audit Failure Scenarios

| Pitfall / failure scenario | Why it fails | Better approach |
|---|---|---|
| “We have a policy, so the control is compliant.” | A policy proves documented intent, not operating effectiveness. | Inspect operational records, configurations, and samples for the required period. |
| Scope excludes identity or endpoint controls shared with production administrators. | Exclusions do not reflect real dependencies, leaving a misleading boundary. | Map service dependencies and shared controls; document justified boundaries and interfaces. |
| Risk register contains generic entries like “malware — high.” | The scenario does not support an accountable treatment decision. | Describe event, weakness, affected service, impact, existing controls, and owner. |
| SoA says “implemented” because a ticket was closed. | Work completion is not proof that the control operates or covers the scope. | Validate deployment and sample operation; link source evidence and date. |
| Audit evidence is an undated screenshot with no scope. | The reviewer cannot confirm period, population, completeness, or authenticity. | Provide source report/export, date, filters, scope, owner, and corroborating tickets/logs. |
| Access review has a sign-off but no population or decisions. | There is no proof what was reviewed or what happened to exceptions. | Preserve the population, review decisions, access changes, and completion evidence. |
| Risk acceptance has no expiry or authorized approver. | Exposure may persist indefinitely without informed authority. | Record authority, rationale, scope, duration, compensating controls, and re-review trigger. |
| GRC writes controls but nobody owns operation. | Control operation becomes ceremonial and evidence is assembled only before audits. | Assign an operational owner, backup owner, cadence, source system, and escalation route. |
| Internal audit reviews its own implementation without safeguards. | Independence/objectivity may be compromised. | Use independent reviewers or documented safeguards appropriate to size and structure. |
| Team creates evidence retrospectively to satisfy an auditor. | This undermines integrity and can mislead assurance providers. | Preserve actual records; disclose gaps, correct the process, and follow finding procedures. |
| Company assumes certification means no security incident can happen. | Assurance confirms conformity within scope and audit rules, not zero risk. | Maintain the risk loop and communicate scope, limitations, exceptions, and changes. |
| Climate amendment is ignored or a generic action is invented without context. | The organization has not shown a reasoned assessment of relevance. | Document the context decision and any relevant interested-party requirements. |

### Evidence quality quick test

Before marking a request complete, ask:

1. **Authenticity:** Is it from the approved source and attributable to an owner/system?
2. **Relevance:** Does it prove the specific control assertion?
3. **Period:** Does it cover the requested window?
4. **Population and completeness:** Can we tell what is included and excluded?
5. **Traceability:** Can a reviewer follow it to a ticket, log, approval, or source record?
6. **Outcome:** Does it show actual action and resolution, not merely a status label?
7. **Protection:** Is it safe to share with the intended reviewer and stored appropriately?

## 6. Interview Cheat Sheet

### Q1. What is ISO 27001?

**Strong answer:** ISO/IEC 27001 is a requirements standard for an Information Security Management System. It gives an organization a risk-driven, continually improving management system for information security. Work includes scope/context, risk assessment and treatment, applicable controls, operating processes, measurement, internal audit, management review, and corrective action. It does not prescribe one identical set of technologies for every company.

### Q2. What is the difference between ISO 27001 and ISO 27002?

**Strong answer:** ISO 27001 specifies ISMS requirements and can be used for certification. ISO 27002 is control guidance that helps organizations understand and implement information-security controls. I would use the applicable official documents together, while keeping clear which statements are requirements and which are guidance.

### Q3. What is the Statement of Applicability?

**Strong answer:** The SoA records the controls an organization determined necessary, their applicability decisions and justifications, and required implementation information. It should trace to risk treatment and obligations. It is not just a list copied from Annex A, and an “implemented” status should be supported by evidence.

### Q4. Do all Annex A controls have to be implemented?

**Strong answer:** The organization considers the Annex A reference controls while determining necessary controls through risk treatment and other requirements. It documents applicability and justification in the SoA. The answer is not “implement every item blindly” or “ignore any control you dislike”; it must be justified against risk, obligations, scope, and the standard's requirements.

### Q5. A control owner gives you a policy but no operating evidence. What do you do?

**Strong answer:** I acknowledge the policy as design evidence, then explain the assertion needing proof. I request operational evidence for the relevant period and sample—for example identity logs and completed access-review records. If evidence is missing or shows the process did not operate, I document the gap, assess risk with the owner, agree a treatment plan, and escalate based on severity and governance rules. I do not mark the control effective solely because a policy exists.

### Q6. How would you scope an ISMS for a SaaS company?

**Strong answer:** Start with the services and business objectives to be covered, then map people, data, processes, systems, locations, identity, deployment pipelines, support access, backups, and supplier dependencies. Review customer and legal obligations with the proper owners. Define interfaces and exclusions with reasons, and ensure scope matches how the service is delivered. Shared controls cannot be excluded just because they serve other parts of the company too.

### Q7. What is the difference between a risk assessment and a risk treatment plan?

**Strong answer:** The assessment identifies and analyzes risk scenarios and determines their level under the approved method. The treatment plan records what the organization will do about each risk—actions, control selection, owners, timelines, resources, and residual-risk decisions. One explains the risk; the other manages the response.

### Q8. How do you prepare an organization for an external ISO audit?

**Strong answer:** Confirm scope and audit criteria, maintain an evidence index, schedule control owners, check that evidence covers the period/population and has traceability, review the risk register and SoA for consistency, verify internal audit and management-review outputs, and ensure findings have credible corrective actions. I would not create evidence after the fact or hide a gap; I would surface it and use the formal finding process.

### Q9. An access review found a former employee with active access. What is your response?

**Strong answer:** Follow incident and access procedures to disable access promptly, preserve relevant logs, determine account privilege and activity, and involve SecOps/IT and HR according to process. Assess whether data or systems were accessed, document the timeline, remediate the offboarding failure, evaluate whether this is a control failure or incident, and test other terminations. Update the risk/finding record and verify corrective action rather than treating account disablement as the end of the problem.

### Q10. What happens after an audit finding is fixed?

**Strong answer:** The owner provides implementation evidence; a reviewer checks that the root cause was addressed, not just the symptom; the control is retested for effective operation and relevant scope; residual risk is reassessed; and closure is approved under the finding process. A closed ticket alone is insufficient.

### Q11. What is management review for?

**Strong answer:** It gives leadership a structured view of the ISMS's continuing suitability, adequacy, and effectiveness. It should consider risk and treatment status, audit results, objectives and metrics, nonconformities, changes in context, feedback, and improvement opportunities—and produce decisions, owners, and follow-up actions.

### Q12. Does ISO 27001 certification mean the company cannot be breached?

**Strong answer:** No. Certification provides independent assurance that the defined ISMS was assessed against the standard within the stated scope and audit rules. It does not guarantee zero incidents, coverage of every group entity, or permanent effectiveness without ongoing operation and improvement.

## 7. Reusable Implementation Checklist

### Scope and governance
- [ ] Executive sponsor, ISMS owner, decision rights, and governance cadence are documented.
- [ ] Scope describes services, people, processes, technology, data, dependencies, interfaces, and justified exclusions.
- [ ] Context and interested-party expectations are reviewed, including climate-change relevance and related interested-party requirements under the 2024 amendment.
- [ ] Relevant legal, regulatory, and contractual obligations have been assessed by appropriate owners.

### Risk and controls
- [ ] Approved risk method, scales, acceptance thresholds, and reassessment triggers exist.
- [ ] Risk scenarios are specific and business-linked.
- [ ] Risk treatment decisions and actions have accountable owners and due dates.
- [ ] SoA has current control applicability decisions, justifications, ownership/status, and traceability.
- [ ] Exceptions have authorized approval, rationale, duration, compensating controls, and review trigger.

### Operation and evidence
- [ ] Controls have operators, defined populations/scope, cadence, evidence source, and escalation path.
- [ ] Policies and procedures are approved, controlled, communicated, and reviewed.
- [ ] Required competence and awareness records exist.
- [ ] Critical processes—access, change, vulnerability, incident, supplier, backup/continuity—have operational evidence.
- [ ] Evidence is attributable, relevant, dated, scoped, traceable, and securely stored.

### Evaluation and improvement
- [ ] Monitoring and measurement methods are defined; metrics lead to decisions.
- [ ] Internal audit program has appropriate competence, scope, criteria, and objectivity.
- [ ] Management review records show inputs, decisions, owners, and action follow-up.
- [ ] Findings receive root-cause analysis, corrective action, retesting, and documented closure.
- [ ] ISMS changes and newly emerging risks trigger reassessment.

## 8. Sample Evidence Request / PBC List

PBC usually means “Provided by Client” or “Prepared by Client,” depending on the engagement's terminology. Follow the external auditor's own wording. The table below is a training example, not an official ISO checklist.

| ID | Request | Period / scope | Primary owner | Reviewer check |
|---|---|---|---|---|
| ISO-01 | Approved ISMS scope statement and latest scope-change record | Current | GRC / ISMS Manager | Scope matches service diagrams, data flows, audit boundary |
| ISO-02 | Context and interested-party register, including review of relevant climate-related context | Current | GRC, Legal, business owner | Sources, relevance decisions, owners, review date |
| ISO-03 | Approved information security policy and communication evidence | Current version; last review | GRC / CISO office | Approval, scope, version history, publication and communication |
| ISO-04 | Risk methodology and risk acceptance authority | Current | Enterprise Risk / GRC | Consistent scales, thresholds, approval route |
| ISO-05 | Current risk register and risk treatment plan | Current + changes during audit period | GRC, risk owners | Traceability, rationale, ownership, overdue actions, residual risk |
| ISO-06 | Statement of Applicability with applicability rationale and implementation state | Current | GRC / ISMS Manager | Reconciles to scope, treatment, obligations, and control evidence |
| ISO-07 | Quarterly privileged-access review source export, review decisions, and removal tickets | Latest completed review in period | IAM / platform owner | Full population, approver, exceptions, remediation proof |
| ISO-08 | Production change sample from ticket to approval, test, deployment, and rollback evidence | Auditor-defined sample period | DevOps / Engineering | Traceable timeline, protected deployment workflow, emergency exceptions |
| ISO-09 | Vulnerability management dashboard, critical issue exceptions, and retest proof | Audit period | Security Engineering | Complete in-scope population, SLA, risk exceptions, validated closure |
| ISO-10 | Backup status and latest restore-test results against recovery objectives | Latest cycle + failures | SRE / IT Operations | Actual restore result, data integrity, elapsed time, corrective action |
| ISO-11 | Security training population and completion results | Audit period | HR / L&D | Reconciles to workforce population and defined exclusions |
| ISO-12 | Internal audit plan, reports, finding log, and follow-up tests | Current cycle | Internal Audit | Objectivity, criteria, evidence, complete corrective-action loop |
| ISO-13 | Latest management-review agenda, inputs, minutes, decisions, action log | Latest review | ISMS Manager / leadership | Required topics considered and actions tracked |
| ISO-14 | Critical supplier assessments and relevant assurance reports | Current + triggered reviews | TPRM / Procurement | Correct service, report period/scope, gaps, exceptions |

### Evidence request email example

**Subject:** Evidence request — quarterly privileged-access review (in-scope production systems)

Hi [Control Owner],

For the current ISMS review, please upload the following for the most recently completed quarter:

1. The source export showing all privileged accounts/roles in the in-scope production environment, including the export date and filters.
2. The completed reviewer decisions and approval/date evidence.
3. Tickets or logs showing selected access removals and their completion timestamps.
4. Any exceptions, escalation records, and documented approvals.

Please use [approved evidence repository] and avoid including passwords, tokens, or unrelated customer/personal data. If part of the request is not available, please explain what is missing and point us to the system of record so we can agree the next step.

Thanks,  
[Analyst name / GRC]

## 9. Example Audit Finding and Remediation

**Finding ID:** ISMS-2026-04 (fictional)

**Title:** Evidence of timely privileged-access removal is incomplete for contractor offboarding.

**Criteria:** The organization's approved access management procedure requires timely removal of access after termination and retention of completion evidence. The precise audit criterion must be linked to the organization's own documented requirement and/or applicable standard requirement, not invented by the analyst.

**Condition / evidence:** In a sample of 20 in-scope contractor terminations, two identity accounts were disabled after the organization's stated target. One case lacked a clear privileged-account verification record. Evidence consisted of the HR termination export, identity audit log, and service ticket timestamps.

**Risk / impact:** Former contractors may retain access beyond business need; the organization may be unable to demonstrate timely, complete offboarding. Actual unauthorized use was not established by this sample and should not be claimed without investigation.

**Likely root cause to validate:** The HR ticket workflow triggers identity disablement but does not consistently verify separate application accounts and privileged cloud roles; responsibility for final verification is unclear.

**Corrective-action plan:**
1. Contain: verify and remove any remaining access; review activity logs where indicated.
2. Correct: update the workflow to trigger identity, SaaS, and privileged-role checks; define an accountable verifier and escalation path.
3. Prevent recurrence: automate deprovisioning where feasible and add a daily exception report.
4. Validate: sample terminations after implementation, compare HR timestamps to identity/application logs, and verify no in-scope accounts remain active without approved justification.
5. Close: GRC or the designated independent reviewer records the retest result, evidence links, residual-risk decision if needed, and closure approval.

**Owner:** IAM Lead (technical action), HR Operations (source event), IT Application Owners (local accounts), GRC (tracking), delegated business/security owner (risk decision).

**Due date:** [Example date selected by the organization based on severity and resources].

**Closure rule:** Do not close because a new workflow document was published. Close only after the change is implemented, operation is evidenced, and follow-up testing supports the conclusion.

## 10. Further Reading and Official References

- [ISO/IEC 27001:2022 — Information security management systems requirements](https://www.iso.org/standard/27001.html) — official standard page and status.
- [ISO/IEC 27001:2022 Amendment 1:2024](https://committee.iso.org/standard/27001) — climate-action amendment information.
- [NIST SP 800-30 Rev. 1](https://csrc.nist.gov/pubs/sp/800/30/r1/final) — risk assessment guidance useful for developing a risk method.
- [NIST CSF 2.0](https://www.nist.gov/cyberframework) — cybersecurity outcomes and governance context.
- [AICPA SOC resources](https://www.aicpa-cima.com/topic/audit-assurance/audit-and-assurance-greater-than-soc-2) — useful for understanding how SOC reporting differs from certification.
- [ISO 19011:2026](https://www.iso.org/standard/19011) — current published ISO guidance for management-system auditing as of this guide's review date; use the version applicable to your audit/program.

> **Disclaimer:** This is a fictional education example, not an implementation plan or certification opinion. Requirements and official standards can change. Before relying on it, confirm current official publications, relevant legal/contractual obligations, the certification body's instructions, and your organization's approved policies and risk decisions.
