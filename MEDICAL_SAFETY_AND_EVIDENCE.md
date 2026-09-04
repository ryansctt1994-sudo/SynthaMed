# Medical Safety and Evidence Boundary

Status date: 2026-09-04
Classification: research / architecture only

SynthaMed, Chaos Command, and CATHEDRAL-OS are not clinically validated products and must not be represented as medical devices, diagnostic systems, prescriptive systems, or autonomous clinical decision makers without the relevant regulatory, clinical, privacy, security, human-factors, and operational evidence.

## Nonclaims

Current repository material does not establish:

- diagnostic accuracy or clinical utility;
- treatment efficacy;
- patient-outcome improvement;
- safe autonomous triage, diagnosis, prescribing, ordering, or care-plan execution;
- regulatory clearance/approval or conformity assessment;
- HIPAA, GDPR, state-law, or other compliance by architecture alone;
- cybersecurity assurance;
- bias/fairness across patient populations;
- prospective safety in a clinical environment;
- interoperability correctness with EHR/FHIR/HL7 systems;
- clinician usability or alarm-fatigue safety;
- liability allocation or legal sufficiency.

## Required evidence before clinical promotion

A clinical claim should have, as applicable: intended-use definition; target users and population; hazard analysis; human-factors/usability testing; data governance and consent model; privacy/security assessment; locked model/version identity; dataset provenance; performance metrics with confidence intervals and subgroup analysis; external validation; prospective or appropriately designed retrospective clinical evaluation; change-control plan; clinician oversight boundaries; incident monitoring; regulatory analysis; and independent review.

## Authority invariant

```text
model_output != diagnosis
recommendation != order
workflow_control != clinical_authority
simulation != clinical_validation
retrospective_accuracy != prospective_safety
regulatory_architecture != regulatory_clearance
```

If an AI component is added, uncertainty must be surfaced, provenance retained, and the system must fail closed where required information or authorization is absent. Human clinical authority cannot be inferred from software control of a workflow.

## Research use

Synthetic scenarios and pressure tests are useful for governance design. They are simulations of failure modes, not evidence of patient safety or clinical effectiveness.
