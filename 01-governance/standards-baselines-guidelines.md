# Policies vs. Standards vs. Baselines vs. Guidelines

## 1. Quick concept

Organizations may use these terms differently, so their governance process should define them. A useful hierarchy moves from management intent to measurable requirements to implementation and operating steps.

| Type | Meaning | Example | Typical force |
|---|---|---|---|
| Policy | Management intent and mandatory expectations | “Privileged access must use strong authentication.” | Mandatory |
| Standard | Specific requirements implementing policy | “Privileged workforce accounts must use phishing-resistant MFA where supported.” | Mandatory |
| Baseline | Minimum approved configuration for a platform or risk tier | Server image requires approved logging, patching, and encryption settings | Mandatory within scope |
| Procedure / runbook | Repeatable steps to do an activity | Disable access after an approved termination event and record it | Mandatory process |
| Guideline | Recommended practice allowing judgment | Preferred secure design patterns for prototypes | Advisory unless adopted as a requirement |

## 2. Enterprise use

A data-protection policy expresses the expectation. A data-classification standard defines tiers and sharing rules. A cloud baseline translates requirements into configuration. A runbook explains deployment and verification. A guideline provides patterns for cases not fully covered elsewhere.

A control owner may use the policy to explain intent, the standard to define the desired state, a configuration export to show actual state, and a test record to show the state was checked.

## 3. Implementation workflow

1. Inventory documents and map them to policies, risks, systems, and controls.
2. Define the document hierarchy and precedence rule for conflicts.
3. Assign owners and approvers.
4. Make requirements testable: scope, population, frequency, thresholds, exceptions, and evidence.
5. Publish an authoritative location and version.
6. Check deployed configurations/processes using samples, automated checks, and exception tracking.

## 4. Pitfalls

- Calling an optional recommendation a “standard.”
- Setting numeric requirements without considering business context or feasibility.
- Publishing a baseline without checking deployed systems against it.
- Duplicating a requirement across documents but updating only one.

## 5. Interview questions

**Q: Is a baseline different from a standard?** A baseline often describes the minimum approved configuration for a platform or risk tier. A standard defines topic-specific or organization-wide requirements. Terminology varies, so I would check the company's document taxonomy.

**Q: What makes a requirement auditable?** It has a defined scope/population, owner, measurable expectation, frequency or trigger, evidence source, exception route, and review mechanism.

## 6. Checklist

- [ ] Terminology and precedence are defined
- [ ] Requirements map to business risks
- [ ] Requirements can be tested
- [ ] Owners, approvers, and exceptions are clear
- [ ] Actual settings/processes are checked
