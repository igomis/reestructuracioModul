# Calendarització per avaluacions del mòdul

## Finalitat del document
Convertir la seqüència d'implantació del mòdul en una peça usable per a programació d'aula real, reagrupant les fases del curs en avaluacions o trimestres amb producte parcial, evidències i instruments recognoscibles.

Este document no substituïx [pla_implantacio_docent.md](pla_implantacio_docent.md), [calendaritzacio_orientativa_aula.md](calendaritzacio_orientativa_aula.md) ni [matriu_evidencies_i_instruments_per_fase.md](../03_avaluacio/matriu_evidencies_i_instruments_per_fase.md). La seua funció és reagrupar eixa seqüència en trams administrables per avaluacions, mantenint el treball per reptes, el projecte base del curs i el mateix marc d'evidències autèntiques.

## Criteris d'ús
- està pensat com a model orientatiu per a un curs desplegat en `3` avaluacions sobre unes `18` setmanes lectives
- cada avaluació s'ha d'entendre com un tram de producte i d'evidència, no només com un tall administratiu
- la calendarització per avaluacions ha de llegir-se junt amb el pla d'implantació docent i la calendarització orientativa per no perdre la lògica interna de fases `0-5`
- Git i GitHub es treballen com a repàs metodològic i criteri de traçabilitat professional, no com a iniciació des de zero
- els itineraris tecnològics no alteren la seqüència d'exigència; només concreten la implementació del mateix producte base
- el pas d'una avaluació a la següent ha d'estar sostingut per evidències mínimes verificables i no només pel calendari

## Distribució per avaluacions
| Avaluació | Setmanes orientatives | Fases connectades | Reptes o focus | Materials activats | Evidències clau | Instrument principal | Producte o lliurament parcial |
|---|---|---|---|---|---|---|---|
| **Avaluació 1** | `1-6` | Fase 0, Fase 1 i obertura de Fase 2 | marc comú, kickoff tècnic, primer flux funcional | materials comuns, sistema d'evidències, projecte base, enunciat base, materials inicials del Repte 2, entrada controlada d'itineraris | repositori usable, `README` inicial, ADR inicial, entorn funcional, autenticació o estat equivalent en marxa | `rubrica_base_reptes.md` | base funcional inicial del producte amb traçabilitat i criteri metodològic |
| **Avaluació 2** | `7-12` | tancament de Fase 2 i Fase 3 | autenticació estable, arquitectura i persistència | materials del Repte 2, materials del Repte 3, materials comuns, itineraris `Laravel`, `Express/Nest` i `FastAPI` com a suport principal | flux d'usuari complet, persistència coherent, arquitectura per capes o equivalent, proves mínimes, documentació actualitzada | `rubrica_base_reptes.md` | backend funcional i mantenible, preparat per exposar-se com a API |
| **Avaluació 3** | `13-18` | Fase 4 i Fase 5 | publicació i consum d'API, integració híbrida i tancament | materials del Repte 4, materials del Repte 5, materials comuns, reutilització final dels itineraris | contracte API, documentació d'endpoints, col·lecció de proves, flux híbrid complet, defensa tècnica i AI log si aplica | `rubrica_defensa_tecnica.md` | producte final del curs publicat, integrat i defensable |

## Desenvolupament per avaluacions
### Avaluació 1
Setmanes orientatives: `1-6`

Focus:
- activar el marc comú de treball, evidències i ús verificable de la IA
- arrancar el projecte base del curs amb domini, stack i primer criteri d'arquitectura
- obrir el Repte 2 amb una primera funcionalitat real d'autenticació, sessió o estat equivalent

Materials activats:
- materials comuns del mòdul
- projecte base i enunciat base del projecte del curs
- sistema d'evidències i instruments inicials de revisió
- primer ús controlat de l'itinerari triat per a bootstrap i auth

Evidències clau:
- repositori creat amb traça inicial coherent
- primer `README` i ADR o registre equivalent
- entorn funcional i decisió de domini documentada
- primers fluxos d'usuari operatius o clarament encaminats

Instrument principal:
- `rubrica_base_reptes.md`

Producte o lliurament parcial:
- base funcional inicial del producte, amb criteris comuns assumits i prova que el grup treballa sobre producte i no només sobre infraestructura

### Avaluació 2
Setmanes orientatives: `7-12`

Focus:
- consolidar el Repte 2 perquè la base funcional siga estable i verificable
- activar el Repte 3 com a pas de funcionalitat a mantenibilitat
- usar l'itinerari tecnològic com a suport directe per capes, persistència i validacions

Materials activats:
- materials del Repte 2 i del Repte 3
- materials comuns com a suport transversal de proves, documentació i IA verificable
- itineraris `Laravel`, `Express/Nest` i `FastAPI` com a suport principal de stack

Evidències clau:
- autenticació funcional i control d'accés mínim
- model de dades i persistència coherents amb el domini
- separació per capes o equivalent i refactorització explicable
- proves mínimes, `README` actualitzat i AI log si s'ha usat IA

Instrument principal:
- `rubrica_base_reptes.md`

Producte o lliurament parcial:
- backend funcional, persistent i mantenible, amb base suficient per passar a contracte API sense improvisació estructural

### Avaluació 3
Setmanes orientatives: `13-18`

Focus:
- publicar el backend com a API usable i provar-ne el consum
- connectar el producte amb una integració externa, automatització o flux híbrid amb valor real
- tancar documentació, proves i defensa tècnica del producte del curs

Materials activats:
- materials del Repte 4 i del Repte 5
- materials comuns encara actius per `README`, debugging, proves i AI log
- reutilització final dels itineraris per aplicar el mateix nivell de qualitat a API i integració

Evidències clau:
- endpoints principals publicats i documentats
- col·lecció de proves o consum verificat de l'API
- workflow híbrid complet amb control mínim d'errors
- documentació final, defensa tècnica i AI log tancat si aplica

Instrument principal:
- `rubrica_defensa_tecnica.md`

Producte o lliurament parcial:
- producte final del curs amb API usable, integració realista i conjunt d'evidències suficient per avaluació final i defensa

## Relació amb els materials
- els materials comuns entren des de l'Avaluació 1 i no desapareixen en cap moment del curs
- els materials del Repte 2 es despleguen entre l'Avaluació 1 i l'Avaluació 2 perquè la base funcional es consolide abans d'obrir arquitectura i persistència
- els materials del Repte 3 tenen el pes principal en l'Avaluació 2
- els materials del Repte 4 i del Repte 5 es concentren en l'Avaluació 3
- els itineraris `Laravel`, `Express/Nest` i `FastAPI` apareixen de manera controlada en l'Avaluació 1 i passen a ser suport principal a partir de l'Avaluació 2

Lectura conjunta amb els altres documents:
- [pla_implantacio_docent.md](pla_implantacio_docent.md) fixa la lògica general de fases i principis d'implantació
- [calendaritzacio_orientativa_aula.md](calendaritzacio_orientativa_aula.md) concreta la seqüència setmana a setmana
- [matriu_evidencies_i_instruments_per_fase.md](../03_avaluacio/matriu_evidencies_i_instruments_per_fase.md) fixa què s'ha de revisar i amb quin instrument en cada fase

## Relació amb l'avaluació
| Avaluació | Instrument principal | Instruments de suport | Criteri de tancament |
|---|---|---|---|
| **Avaluació 1** | `rubrica_base_reptes.md` | `checklist_revisio_repo.md`, `plantilla_ai_log.md` | existix base funcional inicial, repositori usable i criteri comú de treball assumit |
| **Avaluació 2** | `rubrica_base_reptes.md` | checklist del Repte 2, checklist del Repte 3, `plantilla_ai_log.md` | el producte és persistent, explicable i prou estable per exposar API |
| **Avaluació 3** | `rubrica_defensa_tecnica.md` | checklist del Repte 4, checklist del Repte 5, `rubrica_base_reptes.md`, `plantilla_ai_log.md` | el producte final és usable, integrable, documentat i defensable |

Lectura operativa:
- les avaluacions no substituïxen les fases; les reagrupen per fer-les gestionables en programació d'aula
- el tall d'avaluació ha de coincidir amb un estat de producte recognoscible i no amb un tall arbitrari de calendari

## Marges d'adaptació
- si el centre treballa amb calendarització trimestral asimètrica, l'Avaluació 1 es pot ampliar una o dues setmanes sense alterar la lògica interna
- si el grup necessita més temps de consolidació tècnica, convé moure càrrega de l'Avaluació 3 cap a l'Avaluació 2 abans que obrir una API o una integració feble
- si el centre treballa per blocs més curts, el document pot usar-se com a calendarització per períodes d'avaluació parcial mantenint el mateix ordre de producte
- els itineraris no han de generar calendaritzacions separades; la seqüència temporal ha de continuar sent comuna

## Definition of done del document
Este document es considera completat quan:
- convertix la seqüència d'implantació en una calendarització usable per avaluacions o trimestres
- organitza el curs, com a mínim, en Avaluació 1, Avaluació 2 i Avaluació 3
- indica per a cada avaluació setmanes orientatives, focus, materials activats, evidències clau, instrument principal i producte o lliurament parcial
- connecta explícitament amb el pla d'implantació docent, la calendarització orientativa d'aula i la matriu d'evidències i instruments
- manté Git/GitHub com a repàs metodològic i criteri de traçabilitat, no com a iniciació bàsica
- és reusable en context real de programació docent sense obrir noves estructures innecessàries
