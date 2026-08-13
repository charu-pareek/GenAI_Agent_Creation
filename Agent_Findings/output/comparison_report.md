# Comparison Report

## Summary
- `reference.png` is a blank Zurich amendment template with placeholders and generic fields.
- `generated.png` is the completed version of that template with actual contract values filled in.
- The two images are structurally equivalent, but not textually identical.

## Structure Match
- Same document title: `Avenant à usage général ZURICH`
- Same section flow:
  - Policyholder and contract header
  - Dates of effect and expiration
  - Additional premium / premium rebate
  - Covered insurance and agreed protections
  - Article 1 replacement text
  - Article 3 replacement text
  - Amendment checkbox items
  - Chapter IV exclusion/deletion
  - Premium/return clauses
  - Termination clause

## Key Differences
- `reference.png`
  - Contains placeholders like `NOM DU TITULAIRE DE POLICE`, `ADRESSE ASSURÉ`, `VILLE, PROV. CODE POSTAL`, `DATE DE RESILIATION`
  - Empty or generic values for dates and amounts
  - Template wording without real contract data

- `generated.png`
  - Filled values:
    - `Titulaire de police: D&o Aug Domestic`
    - `N° de contrat: a déterminer`
    - `Date de prise d’effet de l’avenant: 10 août 2026`
    - `Date d’expiration du contrat: 10 août 2027`
    - `Prime supplémentaire: 34 352 $`
    - `Ristourne de prime: s.o.`
  - Article 1 populated with `PH`, `28 Hanover Court, Canada`, `Strathroy Ontario, ON N7G 2V1`
  - Article 3 populated with coverage period `23 juillet 2026` to `30 juillet 2026`
  - Completed amendment selections and financial figures:
    - `prime supplémentaire de 9 812 $`
    - `ristourne de prime de 898 $`
    - termination clause with `ristourne de prime de 892 $`

## Verdict
- If the goal is format/structure verification: `generated.png` matches the template in `reference.png`.
- If the goal is exact content equality: `generated.png` differs because it is the filled-in instance of the template.

## Notes
- OCR extraction shows some recognition noise, but the core template vs. filled-instance difference is clear.
- No extra or missing major sections are present between the two images.
