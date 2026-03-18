# Seqüenciació de sessions en 2 avaluacions

## Finalitat del document
Baixar la programació d'aula operativa del mòdul a una seqüència fina de sessions o blocs curts, de manera que el professorat dispose d'una guia executable per distribuir activitats, materials, evidències i seguiment al llarg de les dues primeres avaluacions lectives.

Este document es llig conjuntament amb [pla_implantacio_docent.md](pla_implantacio_docent.md), [calendaritzacio_orientativa_aula.md](calendaritzacio_orientativa_aula.md), [calendaritzacio_per_avaluacions.md](calendaritzacio_per_avaluacions.md), [programacio_aula_operativa_2_avaluacions.md](programacio_aula_operativa_2_avaluacions.md) i [matriu_evidencies_i_instruments_per_fase.md](../03_avaluacio/matriu_evidencies_i_instruments_per_fase.md). La diferència és de gra: aquells documents fixen el marc, esta peça proposa el ritme concret de desplegament del curs.

## Criteris d'ús
- està pensat per a contextos on el projecte del mòdul s'ha de completar dins de les dues primeres avaluacions lectives
- la unitat real és la sessió o bloc curt de treball; es pot correspondre amb una classe o amb una agrupació de sessions segons la càrrega horària del centre
- Git i GitHub es tracten com a repàs metodològic, traçabilitat i criteri professional, no com a alfabetització inicial
- els itineraris `Laravel`, `Express/Nest` i `FastAPI` s'integren dins de la mateixa seqüència, sense generar calendaris paral·lels
- cada sessió ha de deixar una evidència observable o preparar explícitament el checkpoint següent
- si una sessió crítica no deixa el mínim esperat, s'ha de reabsorbir temps dins de la mateixa avaluació i no desplaçar el nucli del projecte a la tercera

## Estructura general
| Tronc temporal | Sessions orientatives | Fases i reptes | Producte acumulat |
|---|---|---|---|
| **Avaluació 1** | `Sessions 1-8` | `Fase 0`, `Fase 1`, `Fase 2` i inici de `Fase 3` | base funcional real del producte i entrada efectiva a arquitectura i persistència |
| **Avaluació 2** | `Sessions 9-16` | tancament de `Fase 3`, `Fase 4`, `Fase 5` i defensa final | producte persistent, publicat com a API, integrat i defensable |
| **Avaluació 3** | període residual | sense desenvolupament central del projecte | seguiment puntual, connexió amb empresa o `FCT`, ajustos menors si cal |

## Seqüenciació detallada per sessions o blocs curts
### Avaluació 1
| Sessió | Objectiu | Activitats | Materials activats | Evidències esperades | Instrument de seguiment | Punt crític |
|---|---|---|---|---|---|---|
| **Sessió 1** | obrir el marc comú del curs | presentar el projecte base, dominis admesos, criteris de treball per reptes i sistema d'evidències | materials comuns, projecte base, sistema d'evidències | repositori creat, estructura mínima, criteris compartits | `checklist_revisio_repo.md` | evitar un inici només expositiu sense activació real del repositori |
| **Sessió 2** | normalitzar traçabilitat i documentació base | revisar criteri de commits, `README`, `ADR`, proves i `AI log`; repàs de Git/GitHub com a metodologia | materials comuns | primer `README`, primers commits útils, criteri d'ús de IA explicitat | `checklist_revisio_repo.md` | comprovar que Git/GitHub no es tracta com a introducció bàsica ni com a simple còpia de seguretat |
| **Sessió 3** | concretar domini i decisió tècnica inicial | triar domini, casos d'ús bàsics, stack i primera decisió d'arquitectura | fitxa del Repte 1, enunciat base, model d'itineraris | domini triat, ADR inicial o equivalent, orientació tècnica clara | `rubrica_base_reptes.md` | evitar que el domini es trie sense impacte real en el producte |
| **Sessió 4** | deixar una base tècnica executable | arrancar el backend, ordenar estructura inicial i verificar l'entorn de treball | Repte 1, materials comuns, itinerari triat com a suport inicial | esquelet executable, entorn funcional, primers artefactes estables | `rubrica_base_reptes.md` | no tancar el kickoff amb un esquelet buit o no executat |
| **Sessió 5** | obrir el flux funcional d'usuari | implementar registre, login i accés inicial protegit o mecanisme equivalent | materials del Repte 2, materials comuns | primera funcionalitat d'autenticació operativa | `rubrica_base_reptes.md` | comprovar que hi ha producte real i no només formularis o captures |
| **Sessió 6** | consolidar validacions i errors mínims | reforçar validació de servidor, control d'accés, errors previsibles i primeres proves | Repte 2, guia de testing/debugging | validacions mínimes, errors controlats, proves bàsiques | checklist del Repte 2 | evitar fluxos aparentment funcionals però sense control d'errors |
| **Sessió 7** | tancar `R2` com a base usable | revisar `README`, proves i traça del repositori; verificar que el flux funcional és reproduïble | Repte 2, materials comuns | nucli de `R2` complet, documentació actualitzada | `rubrica_base_reptes.md` | no avançar a `R3` amb auth fràgil o documentació desalineada |
| **Sessió 8** | obrir `R3` abans del canvi d'avaluació | començar model de dades, capes o equivalent i persistència inicial | materials del Repte 3, itinerari triat, materials comuns | primer model de dades, refactorització inicial, persistència en construcció | `rubrica_base_reptes.md` | no deixar la primera avaluació tancada sobre estat efímer sense entrada real a arquitectura |

### Avaluació 2
| Sessió | Objectiu | Activitats | Materials activats | Evidències esperades | Instrument de seguiment | Punt crític |
|---|---|---|---|---|---|---|
| **Sessió 9** | consolidar persistència del domini | completar entitats, relacions i persistència funcional | materials del Repte 3, itineraris com a suport principal | model de dades coherent i persistència operativa | checklist del Repte 3 | evitar models inconsistents o persistència parcial només per a demo |
| **Sessió 10** | consolidar mantenibilitat i regressió mínima | reforçar capes, serveis o equivalents, revisar regressions i ajustar documentació tècnica | Repte 3, materials comuns | arquitectura explicable, proves mínimes, `README` tècnic actualitzat | `rubrica_base_reptes.md` | no obrir `R4` sense base persistent i mantenible suficient |
| **Sessió 11** | definir contracte API usable | identificar recursos, endpoints, codis d'estat i errors esperats | materials del Repte 4, itineraris reutilitzats en context d'API | contracte API mínim clar | `rubrica_base_reptes.md` | evitar una API improvisada que no reflectisca el model del producte |
| **Sessió 12** | implementar i publicar endpoints principals | desenvolupar endpoints nuclears, auth d'API i criteri de resposta coherent | Repte 4, materials comuns | endpoints principals funcionals | `rubrica_base_reptes.md` | comprovar que l'API no trenca la lògica ja validada en el backend |
| **Sessió 13** | documentar i provar l'API | preparar col·lecció de proves, documentació d'endpoints i consum verificat | Repte 4, guia de proves i documentació API | documentació coherent, proves i consum verificat | checklist del Repte 4 | assegurar coherència entre documentació, proves i comportament real |
| **Sessió 14** | dissenyar la integració híbrida | triar integració externa o workflow amb `n8n`, definir entrada, eixida i control mínim d'errors | materials del Repte 5, materials comuns | flux híbrid dissenyat i justificat | `rubrica_base_reptes.md` | evitar integracions ornamentals o sense valor de negoci clar |
| **Sessió 15** | executar i provar la integració final | implementar el workflow, provar el flux complet i revisar incidències | Repte 5, itineraris reutilitzats, materials comuns | prova de punta a punta, integració operativa, evidències finals | checklist del Repte 5 | no arribar a defensa amb integració no provada o no reproduïble |
| **Sessió 16** | tancar i defensar el producte | revisar repositori, documentació, `AI log`, narrativa tècnica i defensa final | `rubrica_defensa_tecnica.md`, materials comuns, sistema d'evidències | producte final complet, defensa tècnica coherent, repositori tancat | `rubrica_defensa_tecnica.md` | evitar defenses desconnectades del repositori, de les proves o del procés real |

## Checkpoints de seguiment
| Checkpoint | Moment recomanat | Verificació mínima |
|---|---|---|
| **CP1** | després de la sessió 2 | repositori usable, `README` inicial i criteri de traçabilitat assumit |
| **CP2** | després de la sessió 4 | entorn funcional, domini triat i primera decisió tècnica documentada |
| **CP3** | després de la sessió 7 | `R2` complet com a base funcional real |
| **CP4** | després de la sessió 10 | `R3` consolidat amb persistència i mantenibilitat mínimes |
| **CP5** | després de la sessió 13 | API documentada i provada |
| **CP6** | després de la sessió 16 | producte final integrat, documentat i defensable |

## Evidències acumulatives
- **tram inicial**: repositori, primer `README`, ADR o registre equivalent, criteri de Git/GitHub i `AI log`
- **tram funcional**: flux d'autenticació, validacions, errors mínims i proves bàsiques
- **tram arquitectònic**: model de dades, persistència, capes o equivalent i regressió mínima
- **tram API**: contracte, documentació, proves i consum verificat
- **tram final**: integració híbrida, documentació final, autoria verificable i defensa tècnica

Lectura acumulativa:
- cada tram se sosté sobre l'anterior
- si falla una evidència nuclear, no s'hauria de donar per tancat el checkpoint següent

## Intervencions docents clau
- tallar desviacions primerenques si el grup usa el repositori sense criteri de traçabilitat
- intervenir abans d'obrir `R3` si `R2` encara és només una demo puntual
- frenar el pas a API quan persistència i arquitectura no siguen prou estables
- exigir contrast explícit quan l'ús de la IA augmente o afecte parts nuclears del producte
- usar els itineraris com a suport de resolució i no com a justificació per relaxar exigències
- reforçar defensa, documentació i proves abans de la sessió final, no només al tancament

## Marges d'adaptació
- si el centre té més càrrega horària, cada sessió es pot desplegar en dos moments mantenint els mateixos checkpoints
- si el centre té menys hores, convé compactar sessions contigües dins del mateix tram, però no fusionar checkpoints crítics
- si un grup mostra bloqueig en `Sessions 5-7`, convé absorbir temps de la sessió 8 abans que empényer el problema a la segona avaluació
- si la base persistent encara no és suficient en `Sessions 9-10`, s'ha de retardar `R4`
- la seqüència és comuna per a tots els itineraris; l'adaptació és tècnica, no curricular

## Paper de la tercera avaluació
La tercera avaluació no s'ha de reservar per al desenvolupament nuclear del projecte del mòdul. En este model:
- el producte base ha d'haver quedat completat al final de la sessió `16`
- la tercera avaluació només pot assumir seguiment residual, connexió amb empresa o `FCT`, transferència d'aprenentatge o ajustos puntuals si el centre els necessita
- no s'han de traslladar a este període ni `R4`, ni `R5`, ni la defensa final

## Definition of done del document
Este document es considera completat quan:
- convertix la programació d'aula operativa en una seqüència fina de sessions o blocs curts
- manté el desenvolupament i tancament del projecte dins de les dues primeres avaluacions lectives
- indica per a cada sessió objectiu, activitats, materials activats, evidències esperades, instrument de seguiment i punt crític
- incorpora checkpoints, evidències acumulatives, intervencions docents i marges d'adaptació
- deixa explícit que Git/GitHub és repàs metodològic i criteri de traçabilitat, no iniciació bàsica
- deixa clar el paper no central de la tercera avaluació
