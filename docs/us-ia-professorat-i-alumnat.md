# Ús de la IA per a professorat i alumnat

## Finalitat

Este és el **document canònic** que regula l'ús assistit per IA en el model DWES. La seua funció és fixar què es considera acceptable, què exigix evidència, què entra en delegació excessiva i com es verifica des del professorat.

La resta del repositori ha de remetre a este document quan parle d'IA i no reexplicar-lo de manera paral·lela.

## Àmbit del document

Este document afecta:

- alumnat que usa IA per idear, codificar, documentar, provar o revisar
- professorat que planifica activitats, checkpoints, revisió de repositori i defensa tècnica
- reptes, projecte base, evidències i instruments d'avaluació

## Usos permesos

L'ús assistit per IA és compatible amb el model quan ajuda a:

- explorar opcions tècniques
- resumir documentació
- suggerir esquelets de codi, proves o documentació
- detectar errors, punts cecs o regressions
- comparar alternatives de disseny
- millorar la claredat d'un README, una ADR o una explicació tècnica

## Usos guiats

L'ús assistit per IA exigix control reforçat quan afecta:

- arquitectura del projecte
- autenticació, autorització o control d'accés
- persistència, migracions o model de dades
- contractes API
- integracions externes
- proves que acrediten comportaments crítics

En estos casos, l'alumnat ha de poder explicar:

- què va demanar
- què va acceptar o descartar
- què va modificar
- com ho va verificar

## Evidències que ha de deixar l'alumnat

Quan la IA haja participat en una part rellevant del treball, l'alumnat ha de deixar evidències suficients per a revisió docent:

- commits coherents amb l'evolució real del codi
- issues, tasques o notes de treball quan ajuden a entendre el procés
- README, ADR o documentació actualitzada quan hi haja decisions tècniques
- proves, execucions o verificacions sobre el comportament resultant
- `AI log` o registre equivalent quan la intervenció de la IA afecte decisions, implementació o depuració no trivial

## Treball autònom, ús assistit per IA i delegació excessiva

### Treball autònom

L'alumnat pren les decisions tècniques, escriu o adapta el codi amb criteri propi, verifica el resultat i el pot defensar sense dependre d'un text extern.

### Ús assistit per IA

La IA actua com a suport. L'alumnat continua decidint, adaptant, comprovant i explicant el resultat final. Hi ha traçabilitat suficient i verificació real.

### Delegació excessiva

Hi ha delegació excessiva quan l'alumnat:

- accepta solucions sense entendre-les
- no pot explicar per què funcionen
- no detecta limitacions, errors o riscos bàsics
- presenta documentació decorativa no coherent amb el codi
- substituïx la decisió tècnica pròpia per una resposta generada
- usa la IA per resoldre de manera opaca la part nuclear del repte o de la defensa tècnica

## Criteris bàsics per a verificació docent

El professorat ha de poder verificar, com a mínim:

- que el comportament executat coincidix amb el que s'afirma
- que l'alumnat identifica les peces crítiques del seu codi
- que sap distingir entre decisió pròpia, ús assistit per IA i proposta descartada
- que pot fer microcanvis o respondre preguntes de transferència
- que el repositori, la documentació i les proves sostenen la defensa tècnica

## Relació amb avaluació i defensa tècnica

L'ús assistit per IA no és un problema en si mateix. El que s'avalua és:

- autoria verificable
- criteri tècnic
- qualitat de l'evidència
- coherència entre codi, proves, documentació i defensa tècnica

Per això:

- l'avaluació remet a este document quan necessite criteri sobre IA
- la defensa tècnica ha de permetre distingir treball autònom, ús assistit per IA i delegació excessiva
- una solució funcional però no defensable no acredita el mateix nivell d'aprenentatge

## Vocabulari fixat

- `ús assistit per IA`: suport verificable que no substituïx el criteri de l'alumnat
- `delegació excessiva`: cessió opaca de la part nuclear del treball a la IA
- `document canònic`: peça de referència que regula un àmbit i a la qual remeten les peces derivades
