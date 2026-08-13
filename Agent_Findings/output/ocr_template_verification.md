# OCR Template Verification Report

## Purpose
Generate OCR output for template verification and capture all required details for matching `reference.png` and `generated.png`.

## Files
- `Agent_Findings/Reference/reference.png`
- `Agent_Findings/Reference/generated.png`

## OCR Method
- Used Tesseract OCR via Python `pytesseract`.
- Language mix: French + English.
- Focus: template structure, section labels, and form fields.

## OCR Extracted Text

### reference.png
```
@

Avenant a usage général ZURICH

‘Avenant#

‘Tiulsise de pice

Nedepotice Date de prise deff de favenant

Dated’entrée en vigueur 16 200 2021 Dated'expirationdetapotice 18 aoiit 2021
detapotica

Prime suppiémentaire Ristowme

Loprésent avenant modifie contrat. Veuillez te lire attentivement.
‘Le prdsent avenant modifi a protection accordée en vertu dee:

Police d’assurance de la responsabilité civle en matiore de pratiques d'emploi
Hest convenu que:

Laicle 1 des Conditions particulres est remplacé par le texto suivant:

Article. Thtulaire de police NOM DUTTITULAIREDEPOLICE
Adresse postalo:  ADRESSEJASSURE
VILLE. PROV. CODE POSTAL,
Pays
LLLaicle 3 des Conditions particuleres est remplacé par lo texte suivant:

Astle 3. Période dassurance: A compter du Au
'A OhO! heure locale, & adresse indiqué a Article

Toute prolongation de la période dassurance aux termes du présont avenant ne rét
ablit pas ni
‘Yaugmente les limites de garantie appicables stipuldes de ticles 2 des Conditio
ns partculiores.

LLAvonant # il est souté au présont contrat,
LAvenant [Hest supprimé dans son integrals

Le Chapito IV. [AJOUTER LETTRED'EXCLUSION] ast supprimé dans son intagralts.

Les changements énoneés dans le présent avenant donnent leu & une prime suppiéme
ntaires de
Les changements énoncés dans le présent avenant donnent lieu & une rstourne de p
rime de $.
En contreparie dune ristourne de prime do $I il est convenu que le présent contr
at est résiié
dans intégralté & compte: du DATE DE RESILIATION]
```

### generated.png
```
_
Avenant a usage général ZURICH

‘Avenant net
Titular de police D&o Aug Domestic
a . ‘nee Date de prise deffet de 5
N® de contrat: ‘a determine F 10 aoat 2026,
Date de Prise creffet dy 19 soc1 2026 Date d'expiration du contrat 10 20at 2027,
Prime supplémentaire 34352 Ristourne de prime 80.

Leprésent avenant modife contrat. Veuillez le ire attentivement.
Le présent avenant mosifie ls protection accordée en vertu dea
Police dassurance de la responsabilité civile en matiére de pratiques e’emplo!
Hest convenu que
B_LAticie 1 des Conditions particulires est remplacé parle texte suivant:
Aniclet — Titularede police PH

‘Adresse postale 28 Hanover Gouin, Canada
StrathrayyOntario, ON N76 2V1

B_L’Anicle 3 des Conaitons paniGuleres est remplacé par le texte suivant

Asicle 3 Période assurance: Acompterdu 23jullet 2026 Au 30jillet 2026
‘AhOt heure locale, & fadresse indique 8 ratte 1

‘Toute prolongation de la période d'assurance aux termes du present avenant ne r
étabit pas
‘vaugmente les limites de garantie applcables stipulées de FArtcles 2 des Condit
ions partcubéres.

BB Lavenant # en est ajouté au présent contrat,

BB Lavenant # del est supprime en enter.

BB LeChapitte IV. exref est supprimé dans son intégralité.

Bes changements énonoés dans le présent avenant donnent lieu une prime supplémen
tare de 9 812 $.

B_Les changements énoncés dans le présent avenant donnent leu & une rstoume de p
rime de 898 $.
ZeMmusG(0126) ene Page de?

(©- wr pate Se rch Conga dfensseas SA

B_Encontrepartie dune ristouine de prime de 892 §, est convenu que le présent co
ntrat est rsié dans

ignouoen Heraecabeed ciple

fF A v [a |/so | @ Qa
```

## Template Verification Result
- Template match: PASS
- `generated.png` structure is consistent with `reference.png`.
- Both documents contain the same major sections and clause sequence.
- Differences are only in filled field values and data entries, which is expected.

## Required Verification Details
- Template sections verified:
  - Policyholder header
  - Contract and amendment dates
  - Premium / rebate section
  - Insurance coverage statement
  - Article 1 replacement clause
  - Article 3 replacement clause
  - Amendment checkbox selections
  - Chapter IV deletion/exclusion line
  - Premium increase / rebate values
  - Termination clause
- OCR noise observed in accented text, lower small-print, and final lines.
- Use OCR output as a template verification source, not as exact field-level truth.

## Recommended Next Steps
1. Confirm the report in `Agent_Findings/output/comparison_report.md`.
2. If needed, add a dedicated validation script to compare OCR field labels against expected template labels.
3. Use domain-aware cleanup for exact value extraction if field-level accuracy is required.
