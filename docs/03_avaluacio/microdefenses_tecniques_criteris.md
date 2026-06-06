# Microdefenses tècniques de criteris aplicats al projecte

## Finalitat

Este instrument verifica autoria, comprensió i aplicació real dels criteris d'avaluació després d'un repte. No és una exposició teòrica sobre criteris: és una defensa breu d'una part concreta del projecte amb codi, demo, traçabilitat i declaració d'ús de la IA.

S'activa al final de `R2`, `R3`, `R4` i `R5` com a checkpoint docent abans d'obrir el bloc següent o abans de la defensa final.

## Format comú

- Individual preferentment.
- En parella només si cada membre defensa una responsabilitat, un criteri o una decisió diferenciada.
- `5-7` minuts de defensa.
- `2-3` minuts de preguntes de contrast.
- `3-5` diapositives o una pàgina equivalent de suport.
- Demo, prova funcional o execució reproduïble.
- Codi, fitxer o fragment rellevant obert durant la defensa.
- Commits o traçabilitat del canvi defensat.
- `AI log` o registre breu d'ús d'IA.
- Mini justificació tècnica de la decisió principal.

## Plantilla per a l'alumnat

Cada alumne ha d'arribar amb una resposta curta a estes quatre preguntes:

| Pregunta | Resposta esperada |
|---|---|
| Què he fet jo? | Part concreta del projecte, fitxers tocats i responsabilitat pròpia. |
| Què m'ha suggerit la IA? | Prompt o ajuda rebuda: alternatives, revisió, proves, explicació o esborrany. |
| Què he validat jo? | Prova, demo, comparació amb documentació, execució local o correcció del suggeriment. |
| Quin criteri defense? | Criteri d'avaluació aplicat a una evidència real del projecte. |

No és suficient dir que s'ha usat IA "per ajudar". Cal indicar en què ha ajudat, què s'ha acceptat, què s'ha rebutjat o modificat i com s'ha comprovat.

## Checklist docent de verificació ràpida

| Punt | Evidència mínima |
|---|---|
| Producte real | El fragment defensat existeix en el repositori i forma part del flux del projecte. |
| Codi o configuració | L'alumne pot localitzar i explicar el fitxer rellevant. |
| Demo | Hi ha execució, prova, captura reproduïble o cas verificable. |
| Traçabilitat | Els commits, issues o registre de treball mostren evolució del canvi. |
| IA | L'ús d'IA està declarat i l'alumne pot explicar què ha validat. |
| Criteri | La defensa connecta explícitament una evidència amb un criteri d'avaluació. |
| Autoria | L'alumne respon preguntes de contrast sense dependre d'un text memoritzat. |

## Rúbrica curta

| Nivell | Indicadors |
|---|---|
| No acreditat | No hi ha demo funcional, no localitza el codi, no declara ús d'IA o no pot explicar la decisió defensada. |
| Bàsic | Mostra una evidència real i funcional, però la justificació és limitada o la traçabilitat és feble. |
| Adequat | Connecta criteri, codi, prova i decisió; declara ús d'IA i respon preguntes de contrast. |
| Avançat | A més, compara alternatives, explica errors corregits, mostra prova negativa o de regressió i delimita clarament autoria pròpia. |

## Preguntes de contrast

- Per què has triat esta solució?
- Quin error vas tindre i com el vas corregir?
- Quina part et va suggerir la IA?
- Què has canviat tu respecte a la proposta inicial?
- Com demostraries que açò funciona de veritat?
- Quin criteri d'avaluació queda més clar amb esta evidència?
- Què passaria si canviara esta dada, rol, endpoint o configuració?

## Riscos d'ús inadequat de la IA

- Presentació correcta però desconnectada del repositori.
- Codi generat que l'alumne no pot modificar ni explicar.
- `AI log` genèric sense prompts, decisions ni validació.
- Demo preparada només per al cas feliç, sense error ni contrast.
- Defensa memoritzada que cau quan el docent demana un microcanvi.

## Mesures de control

- Obrir el repositori durant la defensa, no només les diapositives.
- Demanar un canvi menut, una prova negativa o una explicació d'un error real.
- Fer una pregunta individual encara que el treball siga en parella.
- Contrastar el relat amb commits, issues, `README`, proves i `AI log`.
- Registrar en acta si la defensa acredita, queda pendent o requerix recuperació.

## Adaptació realista a l'aula

Si no hi ha temps per defensar tot el grup en una sessió, el docent pot combinar:

- defenses completes per mostreig;
- defensa de `5` minuts per alumnat amb risc;
- revisió ràpida de repo i `AI log` per a la resta;
- recuperació curta en la sessió següent abans d'obrir funcionalitats noves.

La sessió no s'ha de convertir en una presentació ornamental. Si no hi ha evidència real, demo o contrast, no verifica autoria ni comprensió.
