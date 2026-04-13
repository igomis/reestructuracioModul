# Matriu d'evidències i instruments per fase

## Finalitat del document

Concretar quines evidències s'esperen en cada fase temporal del curs i amb quins instruments s'han de revisar, per tal que la implantació docent no depenga només del calendari sinó també d'un seguiment observable i comparable.

Este document completa la calendarització orientativa d'aula. La calendarització indica quan s'activa cada fase; esta matriu indica què s'ha de veure, amb quin instrument s'ha de revisar i quin és el punt crític de verificació en cada moment.

## Principis generals

- cada fase ha de deixar evidències verificables de producte i de procés
- l'instrument principal no substituïx la revisió professional del repositori, la documentació i la defensa
- Git i GitHub es tracten com a metodologia de treball, traçabilitat i repàs de criteris clau, no com a iniciació des de zero
- els itineraris tecnològics no canvien el tipus d'evidència exigida, només la forma d'implementació
- l'ús de la IA només compta com a evidència vàlida si queda registrat, contrastat i defensable
- el pas d'una fase a la següent ha d'estar recolzat per un mínim d'evidències suficients, no només per calendari
- `R2` manté una base comuna en `PHP` abans d'obrir el contrast de frameworks

## Matriu global per fases

| Fase | Evidències principals | Instrument principal | Instrument secundari | Punt crític de verificació |
|---|---|---|---|---|
| **Fase 0. Arrancada i marc comú** | repositori creat, estructura mínima, primer `README`, criteri de commits, AI log assumit | `checklist_revisio_repo.md` | `sistema_evidencies.md`, `plantilla_ai_log.md` | verificar que el grup usa Git/GitHub com a traçabilitat professional i no com a simple còpia de seguretat |
| **Fase 1. Kickoff tècnic** | entorn funcional, domini triat, ADR inicial, primera decisió tècnica, primers commits útils | `rubrica_base_reptes.md` | `checklist_revisio_repo.md`, `plantilla_ai_log.md` | evitar que el kickoff quede en infraestructura sense producte ni justificació tècnica |
| **Fase 2. Base funcional del producte** | registre/login/logout, accés protegit, validacions mínimes, errors controlats, proves bàsiques sobre base comuna en `PHP` | `rubrica_base_reptes.md` | checklist del Repte 2, `plantilla_ai_log.md` | comprovar que la funcionalitat és real, reproduïble i no una demo puntual |
| **Fase 3. Arquitectura i persistència** | arquitectura per capes o equivalent, persistència coherent, model de dades, proves de regressió amb entrada de framework | `rubrica_base_reptes.md` | checklist del Repte 3, `plantilla_ai_log.md` | no obrir API sense base persistent i mantenible suficient |
| **Fase 4. Publicació i consum d'API** | endpoints clau, contracte API, documentació d'endpoints, col·lecció de proves, consum verificat | `rubrica_base_reptes.md` | checklist del Repte 4, `checklist_revisio_repo.md` | assegurar coherència entre contracte, proves, errors i documentació real |
| **Fase 5. Integració híbrida i tancament** | flux híbrid complet, prova de punta a punta, documentació final, defensa tècnica, AI log tancat | `rubrica_defensa_tecnica.md` | `rubrica_base_reptes.md`, checklist del Repte 5, `plantilla_ai_log.md` | evitar tancaments ornamentals sense valor funcional, manteniment ni autoria verificable |

## Desenvolupament per fases

### Fase 0. Arrancada i marc comú

Evidències principals:

- repositori creat i estructura mínima recognoscible
- primer `README` amb sentit operatiu
- historial inicial de commits amb criteri mínim
- repàs assumit de traçabilitat, AI log i ús professional del repositori

Instrument principal:

- `checklist_revisio_repo.md`

Instrument secundari:

- `sistema_evidencies.md`
- `plantilla_ai_log.md`

Punt crític de verificació:

- el grup no ha de demostrar alfabetització des de zero en GitHub, sinó criteri metodològic suficient per usar-lo com a evidència professional del procés

### Fase 1. Kickoff tècnic

Evidències principals:

- entorn funcional del backend
- domini triat i primera decisió tècnica explicable
- ADR inicial o registre equivalent
- primers artefactes de projecte alineats amb l'encàrrec base del curs

Instrument principal:

- `rubrica_base_reptes.md`

Instrument secundari:

- `checklist_revisio_repo.md`
- `plantilla_ai_log.md`

Punt crític de verificació:

- comprovar que existix producte inicial defensable i no només un esquelet de framework sense criteri ni context

### Fase 2. Base funcional del producte

Evidències principals:

- autenticació funcional o estat equivalent
- operació protegida del domini
- validacions mínimes i tractament d'errors rellevants
- proves bàsiques i `README` actualitzat

Instrument principal:

- `rubrica_base_reptes.md`

Instrument secundari:

- checklist del Repte 2
- `plantilla_ai_log.md`

Punt crític de verificació:

- revisar si el flux és realment executable, si els errors són comprensibles i si la traça del repositori acompanya el resultat

### Fase 3. Arquitectura i persistència

Evidències principals:

- separació per capes o equivalent
- model de dades i persistència coherents
- refactorització documentada
- proves de regressió o verificacions equivalents

Instrument principal:

- `rubrica_base_reptes.md`

Instrument secundari:

- checklist del Repte 3
- `plantilla_ai_log.md`

Punt crític de verificació:

- verificar que el sistema és ja mantenible i que no depén d'una arquitectura improvisada o d'estat efímer

### Fase 4. Publicació i consum d'API

Evidències principals:

- API amb endpoints principals publicats
- contracte i documentació d'API
- col·lecció de proves o peticions verificades
- consum real de la funcionalitat publicada

Instrument principal:

- `rubrica_base_reptes.md`

Instrument secundari:

- checklist del Repte 4
- `checklist_revisio_repo.md`

Punt crític de verificació:

- revisar si el contracte d'API coincidix amb el comportament real del backend i amb el model de dades construït en fases anteriors

### Fase 5. Integració híbrida i tancament

Evidències principals:

- integració externa o workflow híbrid amb valor real
- prova de punta a punta del flux
- documentació final i manteniment mínim
- defensa tècnica coherent amb repositori, proves i AI log

Instrument principal:

- `rubrica_defensa_tecnica.md`

Instrument secundari:

- `rubrica_base_reptes.md`
- checklist del Repte 5
- `plantilla_ai_log.md`

Punt crític de verificació:

- comprovar que el tancament del curs és defensable com a producte real i no com a suma de captures o automatitzacions ornamentals

## Evidències transversals

Independentment de la fase, s'han de mantindre actives estes evidències:

- repositori i historial de commits
- documentació tècnica (`README`, ADR o equivalent)
- proves i registre de debugging o validació
- AI log quan hi haja ús de la IA
- defensa tècnica del treball realitzat

Lectura docent:

- el pes principal recau en allò que l'alumnat pot explicar, provar, corregir i defensar
- la coherència entre evidències transversals i lliurable específic de cada fase és obligatòria

## Instruments disponibles

- `checklist_revisio_repo.md`: revisió ràpida de base tècnica, traçabilitat i documentació mínima
- `rubrica_base_reptes.md`: instrument principal per avaluar el nucli de treball dels reptes
- `rubrica_defensa_tecnica.md`: instrument principal per al tancament, autoria i capacitat de justificació
- `sistema_evidencies.md`: marc general per llegir què compta com a evidència en tot el curs
- `plantilla_ai_log.md`: suport per a registrar l'ús verificable de la IA
- checklists específiques dels Reptes 2-5: instruments de contrast operatiu sobre mínims tècnics i estat real del producte

## Relació amb la calendarització

Esta matriu s'ha de llegir conjuntament amb `docs/01_programacio_modul/calendaritzacio_orientativa_aula.md`:

- la calendarització indica quan entra cada fase i quan s'activen materials i itineraris
- la matriu indica quines evidències s'han d'esperar en eixe moment i amb quin instrument convé revisar-les
- la calendarització és el mapa temporal
- la matriu és el mapa de seguiment i verificació

## Riscos de seguiment i com corregir-los

| Risc de seguiment | Senyal d'alerta | Correcció recomanada |
|---|---|---|
| avançar de fase sense evidència suficient | el calendari avança però el repositori i les proves no acompanyen | retardar la fase següent i exigir tancament mínim amb instrument principal i secundari |
| revisar només demos finals | hi ha presentació però poca traça de procés | tornar al repositori, `README`, proves i AI log com a base de revisió |
| infraavaluar la documentació | el codi avança però les instruccions no reflectixen l'estat real | revisar `README`, ADR i contractes API en el tancament de cada fase |
| ús opac de la IA | el resultat sembla correcte però no es pot explicar ni justificar | exigir AI log, prova posterior i preguntes de contrast |
| desigualtat entre itineraris | la stack triada canvia el nivell d'exigència percebut | aplicar la mateixa matriu d'evidències i instruments a `Laravel`, `Symfony` i `NestJS`, i només obrir `FastAPI` si hi ha marc docent clar |

## Definition of done del document

Este document es considera completat quan:

- definix una matriu usable d'evidències i instruments per fase temporal
- organitza el seguiment almenys en les fases 0-5 acordades
- indica per a cada fase evidències principals, instrument principal, instrument secundari i punt crític de verificació
- manté Git/GitHub com a metodologia de traçabilitat i repàs de criteris clau, no com a iniciació des de zero
- es pot llegir conjuntament amb la calendarització orientativa d'aula sense duplicar-la
