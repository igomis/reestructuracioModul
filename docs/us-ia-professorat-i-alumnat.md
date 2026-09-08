# Ús de la IA per a professorat i alumnat

## Finalitat

Este és el **document canònic** que regula l'ús assistit per IA en el model DWES. La seua funció és fixar què es considera acceptable, què exigix evidència, què entra en delegació excessiva i com es verifica des del professorat.

La resta del repositori ha de remetre a este document quan parle d'IA i no reexplicar-lo de manera paral·lela.

## Àmbit del document

Este document afecta:

- alumnat que usa IA per idear, codificar, documentar, provar o revisar
- professorat que planifica activitats, checkpoints, revisió de repositori i defensa tècnica
- reptes, projecte base, evidències i instruments d'avaluació

## Norma comuna per a l’alumnat

La IA pot explicar teoria, aportar exemples menuts diferents del repte, revisar un intent propi, donar pistes de depuració i suggerir casos límit. L’alumnat ha de comprendre la teoria, fer un intent propi, formular un dubte concret, implementar i comprovar personalment el resultat. Es pot preguntar teoria abans del primer intent de codi.

No està permés delegar la implementació de servidor, la configuració avaluable ni les proves del repte: ni amb una solució completa en un xat, ni amb fragments successius, ni amb agents que editen, executen i corregisquen fins a acabar. Acceptar automàticament canvis o entendre’ls a posteriori no convertix la delegació en ús permés. La regla depén de l’ús, no de la marca de la ferramenta.

Es permet generar HTML estàtic i CSS de presentació complets, registrant els fitxers i revisant-los. L’alumne decidix i comprén camps, `name`, `method` i `action`. L’excepció no inclou PHP incrustat, plantilles amb lògica, escapament, validació, sessions, autenticació, persistència, APIs ni JavaScript que resolga funcionalitat avaluable.

Es pot millorar la redacció d’una explicació pròpia o del registre, però mai inventar decisions, converses, proves o resultats. Si la IA proporciona una solució no demanada, cal descartar-la i demanar una pista conceptual més limitada.

La guia operativa per a l’alumnat, amb preguntes model, casos prohibits i exemple de registre, és [Ús de la IA: què pots fer i com demanar ajuda](https://cipfpbatoi.github.io/dwes2627/04_materials/guia_us_verificable_ia.html).

## Aplicació a l’aula

Presentar esta norma abans del treball assistit i recordar-la a l’inici de cada repte. Les referències de les sessions a «ajuda», «revisió» o «suggeriments» s’interpreten dins d’estos límits; no autoritzen generar la funcionalitat avaluable. Les mateixes regles afecten les ampliacions.

El registre habitual és `docs/ai-log.md`. Ha d’incloure teoria i intent previs, pregunta literal, ajuda rebuda, decisió pròpia, comprovació i dubtes pendents. No cal duplicar-lo en un report.

No és obligatori usar IA i no usar-la no penalitza. Quan es demane el registre, una declaració de no ús substituïx les consultes; no s’exigixen converses fictícies. La comprensió es contrasta amb una explicació o modificació breu sense IA. Cap estil de codi ni nom de ferramenta prova per si sol un incompliment: les incidències requerixen contrast docent, sense sancions automàtiques noves.

## Evidències que ha de deixar l'alumnat

Quan la IA haja participat en una part rellevant del treball, l'alumnat ha de deixar evidències suficients per a revisió docent:

- commits coherents amb l'evolució real del codi
- issues, tasques o notes de treball quan ajuden a entendre el procés
- README, nota tècnica de decisió o documentació actualitzada quan hi haja decisions tècniques
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

## IA en ampliacions 9→10

Les ampliacions d'excel·lència també queden dins d'este marc.

La IA es pot usar per:

- contrastar enfocaments
- proposar alternatives
- revisar codi
- suggerir proves
- ajudar a documentar
- comparar implementacions

Però no pot substituir:

- la decisió tècnica de l'alumne
- la validació
- la prova
- ni la defensa de l'ampliació

Una ampliació molt ambiciosa però opaca, no verificada o excessivament delegada en IA no ha de computar com a `9→10`.

## Vocabulari fixat

- `ús assistit per IA`: suport verificable que no substituïx el criteri de l'alumnat
- `delegació excessiva`: cessió opaca de la part nuclear del treball a la IA
- `document canònic`: peça de referència que regula un àmbit i a la qual remeten les peces derivades
