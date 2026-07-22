# Document Verification Report

## 1. Overall Result
PARTIAL MATCH

## 2. File type detection
- Reference input: PNG screenshot
- Generated input: PNG screenshot
- OCR used: Yes, because both inputs are image-based documents

## 3. Extracted Markdown summary

### Reference screenshot (OCR)
```md
# Avenant à usage général ZURICH

## En-tête
- Avenant n° [UNREADABLE]
- Titulaire de police: [UNREADABLE]
- Date de prise d'effet de l'avenant: [UNREADABLE]
- Date d'entrée en vigueur: [UNREADABLE]
- Date d'expiration de l'avenant: [UNREADABLE]
- Prime supplémentaire: [UNREADABLE]
- Ristourne: [UNREADABLE]

## Introduction
- Le présent avenant modifie le contrat. Veuillez le lire attentivement.
- Le présent avenant modifie la protection accordée en vertu de la police d'assurance de la responsabilité civile en matière de pratiques d'emploi.

## Clauses principales
1. Article 1 des Conditions particulières remplacé par le texte suivant.
2. Article 1 — Titulaire de police: [NOM DU TITULAIRE DE POLICE]
3. Adresse postale: [ADRESSE ASSURÉ]
4. Ville / province / code postal / pays: [UNREADABLE]
5. Article 3 des Conditions particulières remplacé par le texte suivant.
6. Article 3 — Période d'assurance: [UNREADABLE]
7. Toute prolongation de la période d'assurance ne rétablit pas ni n'augmente les limites de garantie applicables.
8. L'Avenant [N°] est ajouté au présent contrat.
9. L'Avenant [N°] est supprimé dans son intégralité.
10. Le chapitre IV est supprimé dans son intégralité.
11. Les changements donnent lieu à une prime supplémentaire de $[UNREADABLE].
12. Les changements donnent lieu à une ristourne de prime de $[UNREADABLE].
13. En contrepartie d'une ristourne de prime de $[UNREADABLE], le contrat est résilié à compter du [DATE DE RÉSILIATION].
```

### Generated screenshot (OCR)
```md
# Avenant à usage général ZURICH

## En-tête
- Avenant n° [UNREADABLE]
- Titulaire de police: [POPULATED VALUES, PARTIALLY READABLE]
- Date de prise d'effet: 19 août 2026
- Date d'expiration: 10 août 2027
- Prime supplémentaire: 34352
- Ristourne de prime: 80

## Introduction
- Le présent avenant modifie le contrat. Veuillez le lire attentivement.
- Le présent avenant modifie la protection accordée en vertu de la police d'assurance de la responsabilité civile en matière de pratiques d'emploi.

## Clauses principales
1. Article 1 des Conditions particulières remplacé par le texte suivant.
2. Article 1 — Titulaire de police: [PARTIALLY READABLE]
3. Adresse postale: 28 Hanover Court, Canada
4. Ville / province / code postal / pays: Strathroy, Ontario, ON N6G 2V1
5. Article 3 des Conditions particulières remplacé par le texte suivant.
6. Article 3 — Période d'assurance: du 23 juillet 2026 au 30 juillet 2026
7. Toute prolongation de la période d'assurance ne rétablit pas ni n'augmente les limites de garantie applicables.
8. L'Avenant [N°] est ajouté au présent contrat.
9. L'Avenant [N°] est supprimé dans son intégralité.
10. Le chapitre IV est supprimé dans son intégralité.
11. Les changements donnent lieu à une prime supplémentaire de $[UNREADABLE].
12. Les changements donnent lieu à une ristourne de prime de $[UNREADABLE].
13. En contrepartie d'une ristourne de prime de $[UNREADABLE], le contrat est résilié à compter du [UNREADABLE].
```

## 4. Order comparison result
- The generated document preserves the same overall reading order and clause sequence as the reference.
- The major sections appear in the same order: title → header metadata → introduction → article 1 → article 3 → extension clause → add/remove clause references → chapter IV → premium/return and termination clause.
- No clear out-of-order section was detected from the OCR output.

## 5. Missing sections
- No major section appears to be missing from the generated screenshot.
- Some values are partially unreadable, but the structural sections are still present.

## 6. Extra sections
- No meaningful extra section was detected.
- A few OCR artifacts appear, but they do not represent new document sections.

## 7. Out-of-order sections
- None detected.

## 8. Mismatched values
- The reference uses placeholder or generic values such as [NOM DU TITULAIRE DE POLICE] and [ADRESSE ASSURÉ].
- The generated screenshot contains populated values, including a different policyholder/address and different dates.
- The premium and refund amounts also differ.
- Some fields remain partially unreadable due to OCR quality.

## 9. Final verdict
The generated document follows the same order and structural flow as the reference, but it is not an exact semantic match because several values and fields differ and some content is partially unreadable. The order is correct; the content is not fully equivalent.

## 10. Overall output summary
- Structural order: Match
- Section sequence: Match
- Article sequence: Match
- Table/field order: Match
- Semantic meaning: Partial match
- Overall document quality: Partially aligned but not fully equivalent

## 11. Confidence score
0.84

## 12. Detailed diff report
| Section | Issue | Severity |
|---|---|---|
| Header metadata | Generated page contains populated values and different date information | Medium |
| Article 1 | Reference uses placeholders; generated page shows specific policyholder and address details | Medium |
| Article 3 | Coverage dates differ between the two images | Medium |
| Premium/termination clause | Premium and refund amounts differ | Medium |
| OCR quality | Some text is partially unreadable and may affect exact matching | Medium |

## 13. Mismatch coverage checklist
- Missing sections: None detected
- Extra sections: None detected
- Duplicated sections: None detected
- Out-of-order sections: None detected
- Mismatched values: Yes
- Moved paragraphs or fields: Not clearly detected
- Semantic mismatch: Yes
- Content structure mismatch: No major mismatch
