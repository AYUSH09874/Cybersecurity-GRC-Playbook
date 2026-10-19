# FAIR Risk Analysis: Quantifying Cyber Risk

## 1. Quick concept

FAIR stands for Factor Analysis of Information Risk. It is a model for analyzing and quantifying information risk, often with financial loss estimates. Rather than assigning only a red/amber/green score, an analyst examines the factors that drive loss and represents uncertainty. Quality depends on clear scope, defensible data, and documented assumptions.

References: [FAIR Institute — Learn FAIR](https://www.fairinstitute.org/learn-fair) and [FAIR Model Standard v3.0 (January 2025)](https://www.fairinstitute.org/hubfs/Standards%20Artifacts/Factor%20Analysis%20of%20Information%20Risk%20%28FAIR%29%20Standard%20v3.0%20%28January%202025%29.pdf).

## 2. When FAIR is useful

- Comparing proposed control investments with estimated loss exposure.
- Communicating cyber risk to finance and executives.
- Expressing uncertainty rather than hiding it in one score.
- Comparing scenarios consistently across business units.

FAIR is not necessary for every risk. Qualitative scoring may be appropriate for triage or when reliable data is limited.

## 3. Practical workflow

1. **Define the decision:** e.g., “What is the loss exposure from compromise of the customer portal, and how could MFA reduce it?”
2. **Define scenario boundaries:** asset/process, threat community, event, and business consequence.
3. **Identify loss dimensions:** incident response, downtime, fraud, replacement/recovery, contractual liabilities, and other supportable costs.
4. **Estimate frequency factors:** use incident history, exposure, control performance, threat data, and expert estimates.
5. **Estimate magnitude factors:** consult finance, operations, Legal, and business owners.
6. **Model uncertainty:** state ranges/distributions, confidence, and sensitivity to assumptions.
7. **Compare options:** estimate how each treatment changes frequency or magnitude and compare costs.
8. **Validate and update:** revisit after incidents, architecture changes, or new loss data.

## 4. Illustrative example (not a FAIR calculation)

A SaaS business estimates response, customer notification, service interruption, and contractual costs from an account-takeover scenario. Finance provides cost ranges; incident response provides effort estimates and exposure information; Legal identifies relevant contracts; GRC documents assumptions and confidence. The team models a range instead of presenting a single precise number as fact. MFA and abuse detection are compared based on their expected effect on event frequency or loss magnitude.

Do not represent fabricated numbers as organizational loss data. A real quantitative analysis needs an approved model, documented inputs, sensitivity analysis, and validation by appropriate owners.

## 5. Roles and artifacts

GRC/risk analyst defines the scenario and model assumptions; Security/SecOps supplies exposure and control data; Finance validates costs; Legal/Privacy considers contractual impacts; the business owner explains operational impacts; leadership makes the investment and residual-risk decision. Artifacts include scenario definition, assumptions register, data sources, model version, estimates, uncertainty/sensitivity results, option comparison, and decision record.

## 6. Common pitfalls

- Calling a basic color-coded matrix “FAIR.”
- Presenting a single point estimate without uncertainty or data provenance.
- Comparing different scenario boundaries as though they were equivalent.
- Assuming a quantitative result removes judgment or governance.

## 7. Interview cheat sheet

**Q: How does FAIR differ from qualitative scoring?** Qualitative scoring uses categories or bands. FAIR analyzes the factors driving loss and aims to quantify risk, often financially. Choice depends on the decision, available data, maturity, and the cost of analysis.

**Q: The CFO asks whether a control is worth the cost.** Define the scenario and decision; gather technical and finance inputs; estimate exposure and uncertainty; assess how the control changes frequency or magnitude; compare costs and alternatives; and communicate assumptions and limitations before recommending an option.

## 8. Checklist

- [ ] Decision question and scenario boundaries defined
- [ ] Data sources and assumptions traceable
- [ ] Uncertainty and confidence documented
- [ ] Impact validated by relevant owners
- [ ] Model limitations explained
- [ ] Recommendation is tied to a real decision
