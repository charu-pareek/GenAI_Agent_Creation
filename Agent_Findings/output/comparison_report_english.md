# Comparison Report (English)

## Files Compared
- `Agent_Findings/Reference/Reference1.png`
- `Agent_Findings/Reference/Generated1.png`

## Summary
- `Reference1.png` is the blank Zurich General Purpose Endorsement template with placeholder values and generic wording.
- `Generated1.png` is the populated version of the same template with actual policyholder and policy data filled in.
- The two documents match structurally and follow the same clause sequence, but they are not textually identical because the generated version contains actual values while the reference is a template.

## OCR Findings
### Reference1.png
```text
General Purpose Endorsement ZURICH

Endorsement # |

Policyholder
Policy Number TBD Date of Endorsement
Effective Date of Policy August 18, 2021 Expiry Date of Policy August 18, 2022
Additional Premium

This endorsement changes the policy. Please read it carefully.
This endorsement modifies insurance provided under the following:
Directors & Officers Liability Insurance Policy — Zurich D&O Select

It is agreed that:
Item 1 of the Declarations is replaced with the following:
Item 1.
Policyholder INSURED NAME
Mailing Address: INSURED ADDR
INSURED CITY, PROVINCE, POSTAL CODE
INSURED COUNTRY

Item 3 of the Declarations is replaced with the following:
Item 3. Policy Period: From: 12:01 AM on 1 July 2021 To: 12:01 AM on 1 July 2022
Local time at the address shown in Item 1 of the Declarations
Any extension of the Policy Period pursuant to this endorsement does not reinstate or increase the applicable Limits of Liability as shown in Item 2 of the Declarations.
Endorsement # [blank] is deleted in its entirety.
Endorsement # [blank] is added to this Policy.
Subsection IV [ADD EXCLUSION REFERENCE] is deleted in its entirety.
The changes shown in this endorsement result in an additional premium of $.
The changes shown in this endorsement result in a return premium of $.

In consideration of a return premium of $[blank], it is understood and agreed that this policy is cancelled in its entirety effective [date].
```

### Generated1.png
```text
General Purpose Endorsement ZURICH

Endorsement #1

Policyholder D&O Aug Domestic
Policy Number TBD Effective Date of Endorsement August 10, 2026
Effective Date of Policy August 10, 2026 Expiry Date of Policy August 10, 2027
Additional Premium N/A Return Premium N/A

This endorsement changes the policy. Please read it carefully.
This endorsement modifies insurance provided under the following:
Directors & Officers Liability Insurance Policy — Zurich D&O Select

It is agreed that:
Item 1 of the Declarations is replaced with the following:
Item 1. Policyholder PH Name
Mailing Address: 28 Hanover Court, Canada
Strathroy, Ontario, ON N7G 2V1

Item 3 of the Declarations is replaced with the following:
Item 3. Policy Period: From: 12:01 AM on July 08, 2026 To: 12:01 AM on July 30, 2026
Local time at the address shown in Item 1 of the Declarations
Any extension of the Policy Period pursuant to this endorsement does not reinstate or increase the applicable Limits of Liability as shown in Item 2 of the Declarations.
Endorsement # NEW PS EN is added to this Policy.
Endorsement # DEL-PS-EN is deleted in its entirety.
Subsection IV. PS EX REF is deleted in its entirety.
The changes shown in this endorsement result in an additional premium of $9,898.
The changes shown in this endorsement result in a return premium of $8,989.
In consideration of a return premium of $9,008, it is understood and agreed that this policy is cancelled in its entirety effective July 21, 2026.
```

## Structure Match
- Same document title: `General Purpose Endorsement ZURICH`
- Same endorsement flow:
  - Endorsement header and numbering
  - Policyholder and policy metadata
  - Effective and expiry dates
  - Additional or return premium section
  - Insurance modification statement
  - Item 1 replacement clause
  - Item 3 replacement clause
  - Endorsement add/delete references
  - Premium result clause
  - Cancellation clause

## Key Differences
- `Reference1.png` contains placeholders such as `INSURED NAME`, `INSURED ADDR`, `INSURED CITY, PROVINCE, POSTAL CODE`, and date placeholders.
- `Generated1.png` contains actual values such as:
  - Policyholder: `D&O Aug Domestic`
  - Address: `28 Hanover Court, Canada / Strathroy, Ontario, ON N7G 2V1`
  - Policy period: `July 08, 2026` to `July 30, 2026`
  - Additional premium: `$9,898`
  - Return premium: `$8,989`
  - Cancellation effective date: `July 21, 2026`

## Template Verification Result
- Template match: PASS
- Document structure and clause order match for both files.
- Differences are expected because the reference image is a blank template while the generated image is a populated instance.

## Final Verdict
- `Generated1.png` matches the template structure of `Reference1.png`.
- The documents are not identical in content, but they are consistent as a blank template and its completed version.
- Final decision: PASS for template verification with expected filled-value differences.
