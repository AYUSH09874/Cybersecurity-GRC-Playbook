# NIST SP 800-30 Rev. 1: Risk Assessment in Practice

## 1. Quick concept

NIST Special Publication 800-30 Revision 1, *Guide for Conducting Risk Assessments*, provides guidance for preparing, conducting, and maintaining risk assessments. It helps an organization reason systematically about threat sources/events, vulnerabilities or predisposing conditions, likelihood, impact, and risk. It does not mandate one universal five-by-five scoring formula.

Official source: [NIST SP 800-30 Rev. 1](https://csrc.nist.gov/pubs/sp/800/30/r1/final).

## 2. Working components

| Component | Practical meaning | Example evidence |
|---|---|---|
| Scope and assumptions | What mission, service, assets, and boundaries are assessed? | System diagram, service description |
| Threat source / event | What could cause harm? | Scenario, incident patterns, threat information |
| Vulnerability / predisposing condition | What weakness makes the event more likely or damaging? | Unpatched service, excessive permissions |
| Likelihood | How plausible is the scenario given controls and context? | Threat data, tests, prior incidents, expert judgment |
| Impact | What business harm could occur? | Business impact analysis, contractual exposure, downtime estimates |
| Risk determination | How are likelihood and impact combined under the approved method? | Assessment record |
| Response and monitoring | What action follows and what triggers reassessment? | Treatment plan, risk register |

## 3. Practical workflow

1. **Prepare:** define purpose, scope, stakeholders, risk model, assumptions, and decision criteria.
2. **Identify scenarios:** describe the asset/process, event, weakness/context, and business consequence.
3. **Analyze likelihood and impact:** use evidence and documented assumptions instead of vague labels.
4. **Determine risk:** apply the approved methodology consistently.
5. **Validate with owners:** challenge assumptions with system owners, SecOps, product, Legal/Privacy, and business teams.
6. **Decide response:** mitigate, avoid, transfer/share, or accept within delegated authority.
7. **Maintain:** assign actions, owners, dates, review triggers, and residual-risk reassessment.

### Illustrative scenario

A support platform uses a shared administrator account for a legacy integration. If its credential is compromised, a user could make unauthorized changes to customer records and disrupt support operations. The assessor verifies the account, checks whether actions are attributable to individuals, reviews logs, and validates business impact with the service owner. Treatment includes moving to named accounts, enforcing strong authentication, reducing privileges, and reviewing audit logging. The team tracks implementation and retests before reassessing residual risk.

## 4. Roles and artifacts

GRC facilitates the method; system owners explain architecture and business context; IT/SecOps provide control and threat evidence; Legal/Privacy assess obligations and harm; executives accept risks outside delegated thresholds. Artifacts include scope statement, scenario inventory, assumptions log, assessment, risk register, treatment plan, decision record, and reassessment history.

## 5. Common pitfalls

- Using a score with no defined scale or threshold.
- Calling a vulnerability scan result “the risk” without a scenario or business impact.
- Confusing inherent and residual risk.
- Recording actions without an owner or due date.
- Letting GRC accept risk on behalf of the business owner.

## 6. Interview cheat sheet

**Q: What is the difference between a vulnerability and a risk?** A vulnerability is a weakness or condition. Risk describes an uncertain event and its potential consequence to objectives, considering likelihood and impact. A vulnerability becomes meaningful for prioritization when connected to a plausible scenario and business context.

**Q: What if a team disputes a “high” rating?** Explain the scenario and criteria, show supporting evidence and assumptions, invite the owner to challenge facts, document any revised rating or disagreement, and escalate unresolved questions through the risk forum.

## 7. Checklist

- [ ] Scope and assumptions documented
- [ ] Scenario links event, weakness, asset/process, and consequence
- [ ] Likelihood and impact are evidence-informed
- [ ] Rating follows the approved method
- [ ] Treatment and owner recorded
- [ ] Residual risk and review triggers tracked

## 8. Further reading

- [NIST SP 800-30 Rev. 1](https://csrc.nist.gov/pubs/sp/800/30/r1/final)
- [NIST Risk Management Framework](https://csrc.nist.gov/projects/risk-management/about-rmf)
