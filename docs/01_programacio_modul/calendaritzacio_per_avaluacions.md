# Calendarització per avaluacions del mòdul

## Finalitat del document

Convertir la seqüència d'implantació del mòdul en una peça usable per a programació d'aula real, reagrupant les fases del curs en avaluacions o trimestres amb producte parcial, evidències i instruments recognoscibles.

Este document no substituïx [pla_implantacio_docent.md](pla_implantacio_docent.md), [calendaritzacio_orientativa_aula.md](calendaritzacio_orientativa_aula.md) ni [matriu_evidencies_i_instruments_per_fase.md](../03_avaluacio/matriu_evidencies_i_instruments_per_fase.md). La seua funció és reagrupar eixa seqüència en trams administrables per avaluacions, mantenint el treball per reptes, el projecte base del curs i el mateix marc d'evidències autèntiques.

En este model, el projecte base del mòdul s'ha de desenvolupar i tancar dins de les dues primeres avaluacions. La tercera no es planteja com a tram central de desenvolupament, sinó com a espai residual, de connexió amb empresa o `FCT`, o de tancament puntual si el context del centre ho requerix.

La planificació es calibra sobre un escenari orientatiu d'unes `20` setmanes amb `6` hores setmanals, és a dir, unes `120` hores lectives aproximades concentrades en les dues primeres avaluacions.

## Criteris d'ús

- està pensat com a model orientatiu per a un curs on el desenvolupament lectiu principal del projecte es resol dins de les dues primeres avaluacions
- l'escenari de referència és `Avaluació 1 = 10 setmanes / 60 hores aproximades` i `Avaluació 2 = 10 setmanes / 60 hores aproximades`
- cada avaluació s'ha d'entendre com un tram de producte i d'evidència, no només com un tall administratiu
- la calendarització per avaluacions ha de llegir-se junt amb el pla d'implantació docent i la calendarització orientativa per no perdre la lògica interna de fases `0-5`
- Git/GitHub es treballa com a repàs metodològic i criteri de traçabilitat professional, no com a iniciació des de zero
- els itineraris tecnològics no alteren la seqüència d'exigència; només concreten la implementació del mateix producte base
- el pas d'una avaluació a la següent ha d'estar sostingut per evidències mínimes verificables i no només pel calendari
- API, integració i defensa final han de quedar absorbides en la segona avaluació lectiva ordinària i no desplaçar-se a una tercera avaluació residual

## Lectura del model en 2 avaluacions

- **Avaluació 1**: posa en marxa el marc comú, deixa el producte funcional i obri arquitectura i persistència
- **Avaluació 2**: tanca arquitectura i persistència, resol `API`, integració i defensa final
- **Avaluació 3**: no funciona com a tercer tram de desenvolupament del projecte, sinó com a marge residual o de connexió amb empresa o `FCT`

## Distribució per avaluacions

| Avaluació | Setmanes orientatives | Fases connectades | Reptes o focus | Materials activats | Evidències clau | Instrument principal | Producte o lliurament parcial |
|---|---|---|---|---|---|---|---|
| **Avaluació 1** | `setmanes lectives 1-10 (~60h)` | Fase 0, Fase 1, Fase 2 i inici de Fase 3 | marc comú, kickoff tècnic, base funcional i primera consolidació d'arquitectura | materials comuns, sistema d'evidències, projecte base, enunciat base, materials del Repte 2 i activació inicial del Repte 3, entrada controlada d'itineraris | repositori usable, `README` inicial, ADR inicial, autenticació funcional, validacions mínimes, primers passos de persistència | `rubrica_base_reptes.md` | base funcional real del producte i arquitectura inicial prou sòlida per completar persistència en la 2a avaluació |
| **Avaluació 2** | `setmanes lectives 11-20 (~60h)` | tancament de Fase 3, Fase 4, Fase 5 i defensa final | persistència consolidada, API, integració híbrida i tancament del producte | materials del Repte 3, materials del Repte 4, materials del Repte 5, materials comuns, itineraris `Laravel`, `Express/Nest` i `FastAPI` com a suport principal | model de dades complet, API documentada, proves, flux híbrid, documentació final, defensa tècnica i AI log si aplica | `rubrica_defensa_tecnica.md` | producte final del curs complet, publicat, integrat i defensable dins de la segona avaluació |
| **Avaluació 3** | `període residual o de connexió amb empresa/FCT` | sense desenvolupament central del projecte | connexió amb context professional, seguiment puntual o tancament administratiu | reutilització puntual de documentació i evidències ja generades, si cal | seguiment residual, connexió amb empresa, ajustos menors o tancament puntual | instrument contextual del centre | no s'ha de situar ací el desenvolupament principal del projecte del mòdul |

## Desenvolupament per avaluacions

### Avaluació 1

Setmanes orientatives: `setmanes lectives 1-10` amb unes `60` hores aproximades

Focus:

- activar el marc comú de treball, evidències i ús verificable de la IA
- arrancar el projecte base del curs amb domini, stack i primer criteri d'arquitectura
- completar el Repte 2 i obrir el Repte 3 amb una primera base de persistència i arquitectura

Materials activats:

- materials comuns del mòdul
- projecte base i enunciat base del projecte del curs
- sistema d'evidències i instruments inicials de revisió
- materials del Repte 2
- activació inicial dels materials del Repte 3
- primer ús controlat de l'itinerari triat per a bootstrap, auth i estructura bàsica

Evidències clau:

- repositori creat amb traça inicial coherent
- primer `README` i ADR o registre equivalent
- entorn funcional i decisió de domini documentada
- fluxos d'usuari operatius
- autenticació, sessions o estat equivalent funcionals
- primera capa de persistència o model de dades en construcció explicable

Instrument principal:

- `rubrica_base_reptes.md`

Producte o lliurament parcial:

- base funcional real del producte, amb el nucli de `R2` complet i l'entrada a `R3` ja oberta abans del canvi d'avaluació

### Avaluació 2

Setmanes orientatives: `setmanes lectives 11-20` amb unes `60` hores aproximades

Focus:

- tancar el Repte 3 perquè la base persistent i mantenible quede resolta
- completar el Repte 4 amb contracte API, documentació i consum verificable
- completar el Repte 5 amb integració híbrida i defensa final del producte
- usar l'itinerari tecnològic com a suport directe per persistència, API, integració i qualitat final

Materials activats:

- materials del Repte 3, del Repte 4 i del Repte 5
- materials comuns com a suport transversal de proves, documentació i IA verificable
- itineraris `Laravel`, `Express/Nest` i `FastAPI` com a suport principal de stack

Evidències clau:

- model de dades i persistència coherents amb el domini
- separació per capes o equivalent i refactorització explicable
- endpoints principals publicats i documentats
- col·lecció de proves, consum verificat i flux híbrid complet
- `README` final, defensa tècnica i AI log si s'ha usat IA

Instrument principal:

- `rubrica_defensa_tecnica.md`

Producte o lliurament parcial:

- producte final del curs complet i tancat dins de la segona avaluació lectiva, sense deixar API, integració ni defensa per a una tercera avaluació residual

### Avaluació 3

Setmanes orientatives: `període residual o de connexió amb empresa/FCT`

Focus:

- mantindre la connexió entre el producte del mòdul i el context professional de l'alumnat
- absorbir, només si cal, ajustos puntuals de documentació o seguiment
- evitar que esta avaluació es convertisca en el període central de desenvolupament del projecte

Materials activats:

- no s'activa un paquet central nou del projecte
- es poden reutilitzar evidències, documentació i materials ja consolidats si el centre necessita tancament puntual o connexió amb empresa/FCT

Evidències clau:

- connexió amb context d'empresa o reflexió de transferència, si aplica
- ajustos menors o tancament administratiu, si el centre ho necessita
- no s'hauria de concentrar ací cap lliurable nuclear pendent de `R4`, `R5` o defensa final

Instrument principal:

- instrument contextual del centre o seguiment tutorial

Producte o lliurament parcial:

- no hi ha nou lliurament central del projecte: el producte base del mòdul ha d'haver quedat completat en les dues primeres avaluacions

## Relació amb els materials

- els materials comuns entren des de l'Avaluació 1 i no desapareixen en cap moment del curs
- els materials del Repte 2 es concentren en l'Avaluació 1
- els materials del Repte 3 s'obrin en l'Avaluació 1 i es tanquen en l'Avaluació 2
- els materials del Repte 4 i del Repte 5 s'han d'absorbir dins de l'Avaluació 2
- els itineraris `Laravel`, `Express/Nest` i `FastAPI` apareixen de manera controlada en l'Avaluació 1 i passen a ser suport principal durant l'Avaluació 2
- la tercera avaluació no funciona com a nou bloc de materials del projecte, sinó com a marge residual de context o seguiment

Lectura conjunta amb els altres documents:

- [pla_implantacio_docent.md](pla_implantacio_docent.md) fixa la lògica general de fases i principis d'implantació
- [calendaritzacio_orientativa_aula.md](calendaritzacio_orientativa_aula.md) concreta la seqüència setmana a setmana
- [matriu_evidencies_i_instruments_per_fase.md](../03_avaluacio/matriu_evidencies_i_instruments_per_fase.md) fixa què s'ha de revisar i amb quin instrument en cada fase

## Relació amb l'avaluació

| Avaluació | Instrument principal | Instruments de suport | Criteri de tancament |
|---|---|---|---|
| **Avaluació 1** | `rubrica_base_reptes.md` | `checklist_revisio_repo.md`, checklist del Repte 2, `plantilla_ai_log.md` | existix base funcional real, repositori usable i entrada efectiva a arquitectura i persistència |
| **Avaluació 2** | `rubrica_defensa_tecnica.md` | checklist del Repte 3, checklist del Repte 4, checklist del Repte 5, `rubrica_base_reptes.md`, `plantilla_ai_log.md` | el producte final queda persistent, usable, integrable, documentat i defensable dins del període lectiu ordinari |
| **Avaluació 3** | instrument contextual del centre | seguiment tutorial o connexió amb empresa/FCT | no es reserva esta avaluació per al desenvolupament nuclear del projecte |

## Checkpoints de pas entre avaluacions

| Checkpoint | Moment | Decisió docent associada |
|---|---|---|
| **CP-A1** | tancament de l'Avaluació 1 | no passar a l'Avaluació 2 sense `R2` complet i entrada real a `R3` |
| **CP-A2** | tram central de l'Avaluació 2 | no obrir integració ni defensa si `R3` i `R4` no deixen persistència i API prou estables |
| **CP-A3** | tancament de l'Avaluació 2 | el producte ha de quedar completat, defensable i documentat abans del pas a la tercera avaluació |

Lectura operativa:

- les avaluacions no substituïxen les fases; les reagrupen per fer-les gestionables en programació d'aula
- el tall d'avaluació ha de coincidir amb un estat de producte recognoscible i no amb un tall arbitrari de calendari
- el projecte base del curs s'ha de completar dins de les dues primeres avaluacions

## Marges d'adaptació

- si el centre treballa amb calendarització trimestral asimètrica, convé absorbir la major part del temps lectiu útil dins de les dues primeres avaluacions
- si el grup necessita més temps de consolidació tècnica, convé reforçar o compactar l'Avaluació 2 abans que desplaçar API o integració a una tercera avaluació residual
- si el centre treballa per blocs més curts, el document pot usar-se com a calendarització per períodes d'avaluació parcial mantenint el mateix ordre de producte
- els itineraris no han de generar calendaritzacions separades; la seqüència temporal ha de continuar sent comuna
- si el centre partix d'una càrrega diferent de les `120` hores aproximades, cal recalcular la densitat de cada avaluació sense alterar el model `A1 -> A2 -> tancament abans de FCT`

## Definition of done del document

Este document es considera completat quan:

- convertix la seqüència d'implantació en una calendarització usable per avaluacions o trimestres
- organitza el curs, com a mínim, en Avaluació 1, Avaluació 2 i Avaluació 3
- indica per a cada avaluació setmanes orientatives, focus, materials activats, evidències clau, instrument principal i producte o lliurament parcial
- connecta explícitament amb el pla d'implantació docent, la calendarització orientativa d'aula i la matriu d'evidències i instruments
- manté Git/GitHub com a repàs metodològic i criteri de traçabilitat, no com a iniciació bàsica
- deixa explícit que el projecte base del mòdul s'ha de completar dins de les dues primeres avaluacions
- és reutilitzable en context real de programació docent sense obrir noves estructures innecessàries
