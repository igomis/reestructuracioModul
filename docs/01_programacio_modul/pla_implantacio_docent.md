# Pla d'implantació docent del mòdul

## Finalitat del document
Convertir la reestructuració del mòdul en una seqüència d'aula executable, connectant programació, reptes, projecte base, materials, itineraris i avaluació en un recorregut docent realista.

Este document no redefinix el currículum ni substituïx les fitxes de repte. La seua funció és baixar a nivell d'implantació: indicar en quin moment s'activa cada bloc, quines evidències s'esperen, quin instrument principal s'utilitza i quins punts crítics s'han de controlar perquè el curs avance com a producte evolutiu i no com a suma de peces aïllades.

## Principis d'implantació
- treballar per fases que acumulen producte, no per temes desconnectats
- mantindre el projecte base del curs com a fil conductor de totes les decisions d'aula
- activar materials comuns abans d'exigir producte específic de repte o d'itinerari
- no plantejar GitHub com una alfabetització des de zero, sinó com una posada a punt metodològica i professional
- introduir els itineraris com a variació guiada, no com a fragmentació del grup
- prioritzar evidències autèntiques: repositori, proves, documentació, AI log i defensa tècnica
- usar la IA com a suport verificable, mai com a substitut de comprensió, validació o autoria
- aproximar el ritme d'aula a un entorn professional realista: planificar, implementar, provar, documentar i defensar

## Seqüència global del curs
| Fase | Propòsit docent | Reptes connectats | Materials activats | Evidències principals | Instrument principal |
|---|---|---|---|---|---|
| **Fase 0. Arrancada i marc comú** | establir criteris compartits de treball, evidència i ús de la IA abans d'entrar al producte | marc previ al Repte 1 | materials comuns de mòdul (`Git`, `README/ADR`, testing/debugging, IA verificable), sistema d'evidències, projecte base del curs | repositori inicial, criteris de treball assumits, primer `README`, traça mínima d'organització | `checklist_revisio_repo.md` |
| **Fase 1. Kickoff tècnic** | preparar el servei backend base i fixar domini, entorn i primera decisió tècnica | Repte 1 | fitxa del Repte 1, enunciat base del projecte, materials comuns, model d'itineraris com a marc | repo funcional, decisió d'arquitectura, `README`, ADR inicial, AI log si cal | `rubrica_base_reptes.md` |
| **Fase 2. Base funcional del producte** | construir identitat, sessions, validacions i primera funcionalitat real del producte | Repte 2 | materials del Repte 2, materials comuns, suport controlat de l'itinerari triat per a bootstrap i auth | registre/login/logout, accés protegit, validacions, primers casos de prova, documentació actualitzada | `rubrica_base_reptes.md` |
| **Fase 3. Arquitectura i persistència** | convertir el backend funcional en una base mantenible, persistent i preparada per créixer | Repte 3 | materials del Repte 3, materials comuns, itineraris tecnològics com a suport principal de stack | refactorització per capes o equivalent, persistència funcional, proves de regressió, model de dades, AI log si hi ha suport de IA | `rubrica_base_reptes.md` |
| **Fase 4. Publicació i consum d'API** | exposar el producte com a API usable i provar-ne el consum | Repte 4 | materials del Repte 4, materials comuns, reutilització dels itineraris per aplicar auth, estructura i proves al contracte API | endpoints principals, documentació d'API, col·lecció de proves, consum verificat, `README` actualitzat | `rubrica_base_reptes.md` |
| **Fase 5. Integració híbrida i tancament** | connectar el producte amb automatització o servei extern i tancar-lo com a resultat defensable de curs | Repte 5 | materials del Repte 5, materials comuns, itineraris com a suport de stack per al tancament tècnic | workflow híbrid documentat, prova completa del flux, evidències de manteniment, AI log, defensa final | `rubrica_defensa_tecnica.md` |

## Activació de materials per fases
### Fase 0. Arrancada i marc comú
- s'activa la base comuna del mòdul: Git, `README/ADR`, testing/debugging i ús verificable de la IA
- no es fa una introducció des de zero a GitHub; es fa una posada a punt metodològica amb repàs de traçabilitat, commits, `README`, `ADR` i AI log
- s'introduïx el sistema d'evidències com a criteri transversal
- es presenta el projecte base com a marc professional del curs

### Fase 1. Kickoff tècnic
- s'activa la fitxa del Repte 1 com a porta d'entrada al producte
- s'usa l'enunciat base del projecte del curs per fixar domini, actors i objectiu tècnic
- els itineraris encara no són el centre de la fase, però sí el marc que delimita stacks autoritzats

### Fase 2. Base funcional del producte
- s'activen els materials específics del Repte 2 sobre flux d'usuari, sessions, validació i errors
- es mantenen com a base obligatòria els materials comuns de documentació, proves i IA
- l'itinerari triat pot usar-se com a suport controlat per arrancada i auth, sense trencar el nucli comú

### Fase 3. Arquitectura i persistència
- s'activen els materials del Repte 3 com a nucli de treball
- els itineraris passen a ser suport docent directe per aplicar capes, persistència i validació segons stack
- el projecte base queda ja alineat amb model persistent i mantenibilitat mínima

### Fase 4. Publicació i consum d'API
- s'activen els materials del Repte 4 per contracte API, documentació i proves
- els itineraris s'utilitzen com a patró reusable per aplicar auth, estructura i validacions al context d'API
- es mantenen actius `README`, testing/debugging i AI log com a materials transversals

### Fase 5. Integració híbrida i tancament
- s'activen els materials del Repte 5 per flux híbrid, n8n o equivalent i manteniment
- els itineraris es reutilitzen com a suport tècnic, no com a eix de variació nova
- tota la base comuna continua activa perquè el tancament exigix repositori, proves, documentació i defensa

## Evidències d'aprenentatge per fase
| Fase | Evidències mínimes |
|---|---|
| **Fase 0** | repositori creat, estructura mínima, primer `README`, criteris de Git i AI log assumits |
| **Fase 1** | entorn funcional, decisió tècnica inicial, ADR o registre equivalent, traça de primers commits |
| **Fase 2** | flux funcional d'usuaris i sessions, validacions mínimes, errors controlats, proves bàsiques |
| **Fase 3** | arquitectura per capes o equivalent, persistència funcional, model de dades, regressió mínima documentada |
| **Fase 4** | API publicada, contracte clar, documentació d'endpoints, col·lecció de proves i consum verificat |
| **Fase 5** | integració externa o workflow híbrid, prova de punta a punta, documentació final, defensa tècnica del producte |

## Instruments d'avaluació per fase
| Fase | Instrument principal | Instruments de suport |
|---|---|---|
| **Fase 0** | `checklist_revisio_repo.md` | `sistema_evidencies.md`, `plantilla_ai_log.md` |
| **Fase 1** | `rubrica_base_reptes.md` | `checklist_revisio_repo.md`, `plantilla_ai_log.md` |
| **Fase 2** | `rubrica_base_reptes.md` | checklist del Repte 2, `plantilla_ai_log.md` |
| **Fase 3** | `rubrica_base_reptes.md` | checklist del Repte 3, `plantilla_ai_log.md` |
| **Fase 4** | `rubrica_base_reptes.md` | checklist del Repte 4, `checklist_revisio_repo.md` |
| **Fase 5** | `rubrica_defensa_tecnica.md` | `rubrica_base_reptes.md`, checklist del Repte 5, `plantilla_ai_log.md` |

## Punts crítics d'implantació
- no obrir els itineraris com a mons separats; han de continuar lògica comuna de reptes i projecte base
- no perdre el fil de producte: cada fase ha d'afegir una capa real al backend del curs
- no reduir l'avaluació a la demo final; cal recollir evidència de procés, prova i documentació
- no deixar els materials comuns només al principi; han de continuar actius durant tot el curs
- no convertir la IA en drecera invisible; ha de quedar sempre vinculada a execució, contrast i defensa
- controlar bé la transició entre Fase 2 i Fase 3, perquè és on es juga la qualitat del producte i la compatibilitat entre itineraris

## Riscos previsibles i mesures de control
| Risc previsible | Impacte | Mesura de control |
|---|---|---|
| fragmentació excessiva entre itineraris | pèrdua de comparabilitat i sobrecàrrega docent | mantindre nucli comú, checklist equivalent i activació principal dels itineraris a partir de Fase 3 |
| sobrecàrrega de materials sense seqüència clara | dispersió d'aula i baix ús real dels documents | activar materials per fases i no com a catàleg complet des del primer dia |
| ús de la IA sense verificació | pèrdua d'autoria i de defensa tècnica | exigir AI log, prova posterior i preguntes de contrast sobre el treball entregat |
| pas massa ràpid a API o integració sense base estable | producte fràgil i regressions constants | no obrir Fase 4 o Fase 5 sense tancament mínim de Fase 3 i evidències de persistència funcional |
| documentació desalineada amb el codi | dificultat de seguiment i defensa | revisar `README`, ADR i contractes API en el tancament de cada fase |
| repositoris amb poca traça real | dificultat per avaluar procés i evolució | usar checklist de repositori i revisió periòdica de commits, proves i issues |

## Resultat esperat al tancament del curs
En tancar el curs, l'alumnat hauria d'haver construït i defensat un backend realista, evolutiu i verificable:
- amb domini clar i casos d'ús recognoscibles
- amb autenticació, persistència, API i una integració híbrida o automatització funcional
- amb documentació tècnica usable, proves mínimes i historial de treball autèntic
- amb una implementació comparable en qualsevol dels itineraris autoritzats
- amb capacitat de justificar decisions, explicar errors, defensar l'ús de la IA i proposar continuïtat del producte

## Definition of done del document
Este document es considera completat quan:
- definix una seqüència d'implantació docent executable i no només un mapa de fases
- organitza el curs en les fases 0-5 acordades
- connecta explícitament cada fase amb reptes, materials activats, evidències i instrument principal
- integra projecte base, treball per reptes, itineraris tecnològics i ús verificable de la IA
- identifica punts crítics, riscos previsibles i mesures de control
- deixa visible que el repositori entra en fase d'implantació docent
