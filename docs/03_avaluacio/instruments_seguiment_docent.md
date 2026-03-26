# Instruments de seguiment docent

## Finalitat del document

Definir el sistema mínim de seguiment docent del curs perquè la implantació no depenga només de calendarització, entrega final o impressió general del professorat, sinó d'una revisió periòdica basada en evidències, checkpoints i decisions docents registrades.

Este document es llig conjuntament amb [matriu_evidencies_i_instruments_per_fase.md](matriu_evidencies_i_instruments_per_fase.md), [sistema_evidencies.md](sistema_evidencies.md) i [curs_executable_dwes_2_avaluacions.md](../01_programacio_modul/curs_executable_dwes_2_avaluacions.md). La matriu diu què cal veure per fase; esta peça diu amb quins instruments fer-ne el seguiment real i en quin moment convé activar-los.

Marc estable d'ús:

- poden existir contextos de treball compartit, sincronitzat o parcialment comuns
- però el seguiment, la verificació, la defensa i la decisió docent s'han de resoldre amb criteri individual
- un producte comú no substituïx l'acreditació individual de funcionalitat, traçabilitat, autoria i ús verificable de la IA

## Quan usar cada instrument

| Instrument | Quan s'usa | Funció principal |
|---|---|---|
| `checklist_revisio_repo.md` | arrancada del curs, primers checkpoints i revisions ràpides de traçabilitat | comprovar repositori usable, `README`, criteri de commits i base metodològica compartida |
| `rubrica_base_reptes.md` | seguiment ordinari dels Reptes `1`, `2`, `3` i `4` | valorar progrés tècnic, coherència del producte i qualitat mínima del lliurable |
| `rubrica_defensa_tecnica.md` | tancament del Repte `5` i defensa final | verificar producte final, autoria, justificació tècnica i coherència global |
| `sistema_evidencies.md` | durant tot el curs | recordar què compta com a evidència vàlida de producte i de procés |
| `plantilla_ai_log.md` | sempre que hi haja ús rellevant de la IA | registrar ús, contrast i verificació humana |
| [plantilla_registre_seguiment_per_equip.md](plantilla_registre_seguiment_per_equip.md) | seguiment setmanal o quinzenal per alumne, encara que hi haja context compartit | deixar traça breu de l'estat individual real i de la decisió docent següent |
| [plantilla_acta_checkpoint.md](plantilla_acta_checkpoint.md) | checkpoints de canvi de fase o tancament de repte | deixar constància formal del que s'ha revisat i decidit per alumne |

## Relació amb fases 0-5

| Fase | Instrument principal | Instruments de suport | Ús docent recomanat |
|---|---|---|---|
| **Fase 0. Arrancada i marc comú** | `checklist_revisio_repo.md` | `sistema_evidencies.md`, `plantilla_registre_seguiment_per_equip.md` | verificar base de treball, traçabilitat i repàs metodològic de Git/GitHub amb rastre individual |
| **Fase 1. Kickoff tècnic** | `rubrica_base_reptes.md` | `checklist_revisio_repo.md`, `plantilla_acta_checkpoint.md` | comprovar domini, stack, entorn funcional i primera decisió tècnica amb verificació individual |
| **Fase 2. Base funcional del producte** | `rubrica_base_reptes.md` | checklist del Repte 2, `plantilla_registre_seguiment_per_equip.md`, `plantilla_ai_log.md` | validar auth o estat equivalent, validacions, errors i proves bàsiques per alumne |
| **Fase 3. Arquitectura i persistència** | `rubrica_base_reptes.md` | checklist del Repte 3, `plantilla_acta_checkpoint.md`, `plantilla_ai_log.md` | decidir si la base persistent i l'arquitectura permeten obrir `API`, amb defensa individual del flux |
| **Fase 4. Publicació i consum d'API** | `rubrica_base_reptes.md` | checklist del Repte 4, `plantilla_registre_seguiment_per_equip.md` | revisar contracte, endpoints, documentació i proves d'`API` amb acreditació individual |
| **Fase 5. Integració híbrida i tancament** | `rubrica_defensa_tecnica.md` | checklist del Repte 5, `plantilla_acta_checkpoint.md`, `plantilla_ai_log.md` | tancar integració, documentació final, autoria i defensa individual |

## Relació amb reptes 1-5

| Repte | Focus de seguiment | Instruments mínims |
|---|---|---|
| **Repte 1** | domini, stack, entorn funcional i decisió tècnica inicial | `rubrica_base_reptes.md`, `checklist_revisio_repo.md`, `plantilla_registre_seguiment_per_equip.md` |
| **Repte 2** | flux funcional, auth o estat equivalent, validacions i errors mínims | `rubrica_base_reptes.md`, checklist del Repte 2, `plantilla_registre_seguiment_per_equip.md` |
| **Repte 3** | arquitectura per capes o equivalent, persistència i mantenibilitat | `rubrica_base_reptes.md`, checklist del Repte 3, `plantilla_acta_checkpoint.md` |
| **Repte 4** | contracte d'`API`, documentació, proves i coherència de respostes | `rubrica_base_reptes.md`, checklist del Repte 4, `plantilla_registre_seguiment_per_equip.md` |
| **Repte 5** | integració híbrida, prova de punta a punta, tancament i defensa | `rubrica_defensa_tecnica.md`, checklist del Repte 5, `plantilla_acta_checkpoint.md` |

Regla comuna:

- els instruments es poden activar en un mateix moment de classe per a diversos alumnes sobre un producte parcialment compartit
- però la comprovació ha de deixar clar què pot explicar, reproduir i defensar cada alumne

## Evidències que ha de revisar el professorat

- repositori actiu i amb traçabilitat real
- rastre individual recognoscible dins del repositori, encara que hi haja context compartit
- `README` actualitzat segons el moment del curs
- decisions tècniques rellevants registrades amb `ADR` o equivalent
- funcionalitat executable del producte en el repte o fase actual
- part del producte que cada alumne pot explicar i defensar
- proves bàsiques, comprovacions o col·leccions de peticions segons corresponga
- tractament mínim d'errors i depuració observable
- model de dades, persistència i capes o equivalents quan s'arriba a `R3`
- contracte, documentació i consum real d'`API` quan s'arriba a `R4`
- integració externa o workflow híbrid amb valor real quan s'arriba a `R5`
- `AI log` verificable quan la IA haja intervingut en parts rellevants, amb rastre individual

Lectura docent:

- no n'hi ha prou amb veure una demo final
- el criteri principal és si el que afirma cada alumne es pot localitzar, reproduir, revisar i defensar

## Moments mínims de checkpoint

| Checkpoint | Moment recomanat | Què s'ha de validar com a mínim | Instrument formal recomanat |
|---|---|---|---|
| **CP0** | final de Fase 0 | repositori usable, `README` inicial i criteri de traçabilitat assumit | `checklist_revisio_repo.md` + [plantilla_acta_checkpoint.md](plantilla_acta_checkpoint.md) |
| **CP1** | final de Repte 1 | domini triat, stack definit, entorn funcional i primera decisió tècnica | `rubrica_base_reptes.md` + [plantilla_acta_checkpoint.md](plantilla_acta_checkpoint.md) |
| **CP2** | final de Repte 2 | auth o estat equivalent real, validacions, errors mínims i proves bàsiques, acreditats per alumne | checklist del Repte 2 + [plantilla_registre_seguiment_per_equip.md](plantilla_registre_seguiment_per_equip.md) |
| **CP3** | final de Repte 3 | persistència coherent, arquitectura explicable i base suficient per obrir `API` | checklist del Repte 3 + [plantilla_acta_checkpoint.md](plantilla_acta_checkpoint.md) |
| **CP4** | final de Repte 4 | `API` publicada, documentada i provada, amb part defensable per alumne | checklist del Repte 4 + [plantilla_registre_seguiment_per_equip.md](plantilla_registre_seguiment_per_equip.md) |
| **CP5** | final de Repte 5 | integració completa, documentació final, `AI log` tancat i defensa preparada individualment | `rubrica_defensa_tecnica.md` + [plantilla_acta_checkpoint.md](plantilla_acta_checkpoint.md) |

## Criteris per detectar riscos de seguiment

| Risc | Senyal observable | Resposta docent recomanada |
|---|---|---|
| avançar només per calendari | el grup diu que canvia de fase però no hi ha evidència individual suficient | bloquejar el pas i obrir acta de checkpoint amb acció correctora |
| repositori sense valor metodològic | hi ha codi però poca traça, `README` pobre o commits irrellevants | fer revisió específica de repositori i registrar decisió de normalització |
| demo sense producte real | el lliurable funciona només en presentació o sense proves mínimes | exigir reproducció, proves i registre de problemes abans de donar el repte per tancat |
| ús opac de la IA | hi ha codi o decisions que l'alumne no sap explicar | revisar `AI log`, fer preguntes de contrast i deixar constància en el registre de seguiment |
| diferències d'exigència entre itineraris | el stack triat rebaixa artificialment el nivell de control | aplicar el mateix instrument i la mateixa evidència mínima a `Laravel`, `Express/Nest` i `FastAPI` |
| acumulació de bloquejos | el mateix problema apareix en dos registres seguits | retallar abast, redefinir objectiu immediat i fixar checkpoint curt de recuperació |

## Definition of done del sistema de seguiment

El sistema de seguiment es considera completat quan:

- existix un criteri clar de quin instrument s'usa, quan i per a què
- el seguiment cobrix les fases `0-5` i els reptes `1-5`
- els checkpoints mínims del curs queden definits i documentables
- el professorat pot registrar estat, riscos, decisions i accions següents per alumne, encara que hi haja context compartit
- Git/GitHub es revisa com a metodologia de treball i traçabilitat, no com a iniciació bàsica
- el sistema permet detectar desviacions abans que el problema arribe al tancament del curs
