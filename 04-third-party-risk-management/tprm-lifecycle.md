# Third-Party Risk Management (TPRM) Lifecycle

## 1. Quick concept

TPRM is the process for understanding and managing risks introduced by suppliers, cloud services, outsourced operations, and other external parties. A questionnaire is one input—not the whole assessment. Risk depends on the service, data handled, access, business criticality, substitutability, and potential impact.

## 2. Typical lifecycle

1. **Intake and classification:** business owner describes service, data, access, use case, criticality, and start date.
2. **Inherent-risk tiering:** assess exposure before relying on vendor controls.
3. **Due diligence:** use a risk-appropriate combination of questionnaire, SOC 2/ISO reports, penetration-test summary, architecture, continuity, privacy, and contract review.
4. **Gap analysis:** record exceptions and distinguish missing evidence from a confirmed control failure.
5. **Decision:** approve, approve with conditions, defer, or reject according to delegated authority.
6. **Contracting/onboarding:** include appropriate security/privacy terms, breach notification, audit rights, data return/deletion, subcontractor provisions, and exit support.
7. **Continuous monitoring:** track incidents, report expiry, subprocessor/service changes, remediation, and reassessment triggers.
8. **Offboarding:** revoke access, return/delete data, verify retained records, and close contracts/accounts.

## 3. Risk-based evidence

Critical providers may warrant review of independent assurance reports, exceptions, penetration-test summaries, business continuity, data location/transfer, subcontractors, access model, incident response, recovery testing, and remediation status. A low-risk supplier with no sensitive data or system access should not necessarily receive the same burden as a production identity provider.

## 4. Roles

The business sponsor owns the service decision; Procurement owns sourcing/contract workflow; TPRM/GRC coordinates the assessment; Security evaluates technical controls; Privacy/Legal reviews personal-data and contract issues; IT evaluates integrations/access; leadership accepts material residual risk within its authority.

## 5. Artifacts

Supplier inventory, inherent-risk questionnaire, due-diligence request list, report review checklist, issue/exception register, contract clause matrix, approval decision, monitoring history, renewal trigger, and offboarding confirmation.

## 6. Common pitfalls

- Treating a vendor's yes/no answer as proof.
- Approving a certificate without checking scope, date, service, exceptions, and subservice providers.
- Collecting a questionnaire but never obtaining remediation evidence for material gaps.
- Not reassessing after material service, ownership, data, or subprocessor changes.
- Leaving vendor accounts active after contract termination.

## 7. Interview questions

**Q: A critical vendor has a SOC 2 report with exceptions. Is it rejected?** Not automatically. Check service and period, the nature and relevance of exceptions, compensating controls, management response, user-side responsibilities, contract requirements, and criticality. Route residual risk to an authorized owner and document conditions/remediation.

**Q: Who owns vendor risk?** The business owner owns the decision to use the service and associated residual risk within authority. TPRM coordinates due diligence; Security and Privacy provide specialist review; Procurement supports contractual safeguards.
