# NIST Cybersecurity Framework (CSF) 2.0

## 1. Quick concept

NIST CSF 2.0 is a taxonomy of high-level cybersecurity outcomes that organizations use to understand, prioritize, and communicate cyber risk. It is not a prescriptive checklist and does not itself require a particular technology. Organizations define a current state, target state, and prioritized actions aligned with their context.

Official source: [NIST CSF 2.0](https://www.nist.gov/cyberframework), published February 26, 2024. CSF 2.0 added the **Govern** function, making six functions in total.

## 2. The six functions

| Function | Practical question | Example evidence / output |
|---|---|---|
| Govern (GV) | How are cybersecurity strategy, risk expectations, roles, policy, and oversight established? | Risk appetite, policy approvals, supplier-risk approach, governance minutes |
| Identify (ID) | What assets, data, suppliers, and risks must be understood? | Asset inventory, business impact, risk register |
| Protect (PR) | What safeguards reduce likelihood or impact? | IAM, secure configuration, training, data protection |
| Detect (DE) | How does the organization find anomalies and events? | Logging coverage, alert metrics, detection tests |
| Respond (RS) | How are incidents analyzed, communicated, contained, and managed? | Incident plan, tickets, exercise report |
| Recover (RC) | How are capabilities restored and improvements incorporated? | Restore tests, recovery plans, lessons learned |

Functions are a conceptual organization, not a mandatory execution order.

## 3. Implementation workflow

1. Agree on business objectives and the organizational/system boundary.
2. Build a **Current Profile** of relevant outcomes and evidence.
3. Build a **Target Profile** based on risk, obligations, resources, and strategy.
4. Perform a gap analysis and rank improvements by risk and feasibility.
5. Assign owners/budgets and link improvements to existing risk/control registers.
6. Track implementation and update the profile as evidence changes.

## 4. Example

A SaaS company finds that governance for critical suppliers is informal and incident exercises are overdue. Under Govern, it defines supplier-risk ownership and reporting. Under Identify, it creates a critical-supplier inventory. Under Respond, it formalizes severity and escalation expectations. Under Recover, it tests restoration and service recovery. A profile organizes desired outcomes; a framework label alone does not prove a control operates.

## 5. Pitfalls

- Treating CSF as a certification program or legal mandate.
- Claiming a function is complete because a policy mentions it.
- Using the framework without boundaries or business priorities.
- Mapping outcomes to tools without owners or evidence.

## 6. Interview questions

**Q: What changed in CSF 2.0?** It added Govern and emphasized governance and cybersecurity supply-chain risk; it also broadened application to organizations of different sizes and sectors.

**Q: How would you use CSF in a gap assessment?** Define scope/goals, document current outcomes supported by evidence, select a target state based on risk and obligations, identify gaps, assign treatment owners, prioritize, and track progress. Do not describe the profile as a certification.

## 7. Further reading

- [NIST CSF 2.0 publication](https://www.nist.gov/publications/nist-cybersecurity-framework-csf-20)
- [NIST CSF FAQ](https://www.nist.gov/cyberframework/faqs)
