# Qualitative vs. Quantitative Risk Scoring

## 1. Quick concept

Qualitative assessment uses categories such as Low/Medium/High based on defined criteria. Quantitative assessment estimates numerical outcomes, often a range or distribution of loss. A score such as 12/25 is still usually ordinal or semi-quantitative if it represents ranked bands rather than measured quantities.

## 2. Comparison

| Dimension | Qualitative / ordinal | Quantitative |
|---|---|---|
| Output | Category or score band | Estimate or distribution |
| Inputs | Criteria, evidence, judgment | Data, assumptions, model, ranges/distributions |
| Strength | Accessible, efficient for triage | Supports economic comparison and uncertainty analysis |
| Limitation | Categories hide variation; ratings may be subjective | Data-intensive; false precision and model risk possible |
| Best use | Initial prioritization, recurring workflows | Investment decisions where reliable inputs support analysis |

## 3. Workflow

1. Define the decision the assessment must support.
2. Agree on rating definitions and thresholds.
3. Collect evidence and state uncertainty.
4. Apply the selected method consistently.
5. Explain method limitations in reporting.
6. Escalate risks above appetite or delegated authority.
7. Revisit the method if it fails to distinguish risks usefully.

## 4. Example

A team rates backup restoration risk “High” because there is no recent restore evidence and recovery objectives are strict. That is useful for triage. If leadership must choose between two architectures, it may need estimates of outage cost per hour, event frequency, restoration time, implementation cost, and uncertainty. Do not convert “High” to a dollar amount without a defensible model.

## 5. Interview questions

**Q: Is a 5×5 matrix quantitative?** Usually it is an ordinal qualitative scoring approach, even though it uses numbers; the numbers rank categories and should not automatically be treated as precise arithmetic values.

**Q: When would you use FAIR?** When a decision benefits from estimating loss magnitude/frequency, adequate inputs can be developed, and the value of analysis outweighs the cost. Communicate uncertainty and limits.
