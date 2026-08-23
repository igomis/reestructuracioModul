# Curs executable

## Classificació documental

Este és un **document canònic**. Regula l'execució del curs: seqüència, hitos, checkpoints, ritmes, entregables i moments d'avaluació. No reexplica el marc del model, el règim d'avaluació ni el criteri d'ús assistit per IA, que depenen d'altres documents canònics.

## Finalitat

Este és el centre canònic per conduir el curs. Substitueix com a entrada principal el pla d'implantació, les calendaritzacions, la guia de 20 setmanes, la preparació docent directa i els kits de pilotatge.

Els documents de planificació continuen existint com a annexos o arxiu, però la decisió docent operativa ha de començar ací.

## Condicions operatives de partida

- el curs està calibrat sobre unes `20` setmanes i `120` hores lectives aproximades
- el desenvolupament principal del projecte es tanca en dues avaluacions
- la tercera avaluació queda com a espai residual, connexió amb empresa o tancament puntual
- Git/GitHub funciona com a metodologia de treball i traçabilitat
- `R2` es resol sobre base comuna en `PHP`
- el contrast d'itineraris s'obri a partir de `R3`
- `Laravel`, `Symfony` i `NestJS` són les vies base del contrast
- `FastAPI` queda com a via avançada o excepcional

## Seqüència executable del curs

| Moment | Hito operatiu | Checkpoint o entregable mínim |
|---|---|---|
| Inici | activació del curs i del projecte base | repositori inicial, README, domini triat i criteri de treball |
| Repte 1 | arrencada funcional del backend | entorn executable, Docker, landing inicial i primera decisió tècnica |
| Repte 2 | primera funcionalitat protegida | checkpoint `R1 -> R2`, flux autenticat, validacions i proves bàsiques |
| Repte 3 | reconstrucció en framework i persistència | dos fluxos end-to-end, model de dades, migracions, seeders i proves mínimes |
| Repte 4 | publicació i consum d'API | contracte, endpoints, consum verificat i documentació d'API |
| Repte 5 | integració híbrida | funcionalitat integrada, tractament d'errors i prova de punta a punta |
| Defensa tècnica | tancament del curs | evidències finals, repositori coherent i defensa tècnica individual |

## Funció didàctica de cada repte

| Repte | Funció principal | Focus real | Decisió d'abast docent |
|---|---|---|---|
| `R1` | iniciació / arranque | entorn, repositori, `README`, Docker i primera decisió tècnica | no carregar-lo amb formularis, persistència o arquitectura avançada |
| `R2` | construcció nuclear | flux de dades, lògica bàsica, estat, autenticació i primera funcionalitat protegida | és el nucli funcional compartit; encara no és `MVC` ni persistència com a focus |
| `R3` | consolidació | framework, separació de responsabilitats, persistència mínima real i flux **server-rendered** | dividir-lo en dues validacions i reduir l'ambició del segon flux si cal |
| `R4` | integració | contracte d'API, consum real, autenticació i documentació usable | evitar que `RA6` torne a convertir-lo en un repte de persistència |
| `R5` | síntesi amb nucli obligatori de `RA9` | integració externa amb valor de producte, reutilització de serveis i verificació final | mantindre un mínim nuclear obligatori i deixar múltiples integracions o automatitzacions com a ampliació |

## Checkpoints com a control pedagògic real

| Moment | Verificació tècnica mínima | Contrast de comprensió | Traçabilitat de la IA | Decisió docent que habilita |
|---|---|---|---|---|
| Inici de curs | repositori, `README` i criteri de treball actius | el grup sap explicar domini, eines i flux de treball | només si hi ha ús assistit inicial | obertura de `R1` |
| Tancament de `R1` | arrencada reproduïble i landing inicial servida pel backend | justificació de la decisió tècnica i microcanvi simple | revisió d'`AI log` si n'hi ha | pas real a `R2` |
| Tancament de `R2` | flux complet amb cas autoritzat i denegat | explicació de dades, estat i autenticació | contrast entre solució inicial, ajuda d'IA i solució final quan corresponga | pas real a `R3` |
| `CP-R3A` | framework + Docker + BBDD + `migrations`/`seeders` + primer flux **server-rendered** | defensa del circuit petició -> controlador -> dades -> resposta | revisió d'evidències d'ús assistit sobre estructura i modelat | continuïtat de `R3` |
| `CP-R3B` | segon flux, proves mínimes, `README` i backlog curt | justificació de decisions d'arquitectura i de què queda fora | contrast entre codi, `AI log` i demo | obertura de `R4` |
| Tancament de `R4` | contracte d'API, servei funcional i consum real | explicació d'endpoints, autenticació i errors | traçabilitat de contracte, proves i documentació assistida per IA | obertura de `R5` |
| Tancament de `R5` | integració externa amb cas positiu i cas d'error | explicació del mapping, del valor real al producte i del mapa d'integració | comprovació de la comprensió del contracte extern, de la transformació i del nucli de `RA9` | pas a defensa tècnica |
| Defensa final | producte coherent i evidències alineades | autoria individual, criteri tècnic i transferència | revisió final de coherència amb el document canònic d'IA | tancament del curs |

## Checkpoints i moments de revisió

- inici de curs: activació del repositori i comprovació del marc de treball
- tancament de `R1`: verificació de base executable i defensa breu d'arrencada
- tancament de `R2`: funcionalitat protegida reproduïble, registre d'errors i mini defensa tècnica
- `CP-R3A`: base de framework, BBDD i primer flux **server-rendered**
- `CP-R3B`: segon flux, proves mínimes, `README` i decisions d'arquitectura
- tancament de `R4`: API usable, consum verificat i contrast entre contracte i resposta real
- tancament de `R5`: integració híbrida amb valor funcional, cas positiu i cas d'error
- defensa tècnica final: tancament individual del producte i de les evidències

## Documents operatius que s'activen

- [Visió del model](visio-model-dwes.md): només com a marc general
- [Enunciat base del projecte](05_projectes_tecnics/enunciat_projecte_base.md): encàrrec del producte
- [Projecte backend base](05_projectes_tecnics/projecte_base_backend.md): base tècnica comuna
- [Reptes 1-5](02_reptes/repte_01_kickoff_backend.md): desplegament del curs per reptes
- [Ampliacions 9 a 10 per repte](ampliacions-9-a-10-per-repte.md): capa d'excel·lència activable quan el nucli ja està validat

Nota: les integracions externes (p. ex. WordPress) s'entenen com ampliacions o integracions possibles dins de `R5`, no com a vies principals del curs.
- [Avaluació i evidències](03_avaluacio/index.md): instruments i criteri d'acreditació
- [Ús de la IA per a professorat i alumnat](us-ia-professorat-i-alumnat.md): criteri únic sobre ús assistit per IA
- [Recursos d'aula](04_materials/index.md): peces derivades de suport

## Annexos útils

Estos documents aporten detall, però no han de competir amb este centre executable:

- [Pla d'implantació docent](01_programacio_modul/pla_implantacio_docent.md)
- [Calendarització per avaluacions](01_programacio_modul/calendaritzacio_per_avaluacions.md)
- [Guia sessió a sessió de 20 setmanes](01_programacio_modul/guia_sessio_a_sessio_20_setmanes.md)
- [Annex de ritmes](01_programacio_modul/annex_suport_i_ampliacio_ritmes.md)
- [Preparació docent directa](01_programacio_modul/preparacio_docent_directa_curs_que_ve.md)
- [Ajustos finals abans d'inici de curs](01_programacio_modul/ajustos_finals_abans_inici_curs.md)
- [Curs executable original ampliat](01_programacio_modul/curs_executable_dwes_2_avaluacions.md)

## Decisions de control

- si no hi ha repositori traçable, no es dona per estabilitzat l'inici
- si `R2` no és reproduïble, no s'obri `R3`
- si `R3` no supera `CP-R3A`, es reduïx l'ambició del segon flux i no s'obri `R4`
- si `R3` no deixa persistència i arquitectura explicables en `CP-R3B`, no s'obri `R4`
- si `R4` no està documentat ni provat, no s'avança cap a `R5`
- si `R5` tensiona massa el calendari, es retalla a una sola integració externa verificable que continue cobrint el mínim nuclear de `RA9` abans de la defensa tècnica

## Via d'excel·lència 9→10

Cada repte pot activar una ampliació `9→10`, però amb una regla simple:

- primer, nucli del repte complet i validat
- després, ampliació tècnica amb valor real

Esta capa no obri una segona programació paral·lela. Servix per donar recorregut a alumnat que acaba prompte o que vol aprofundir fora de classe, reutilitzant instruments ja existents: checklist curta, revisió de repositori, demo funcional i mini defensa tècnica.

## Criteri de tancament

El curs queda executable quan el producte final és recognoscible, el calendari permet tancar `R1-R5` dins de dues avaluacions, els checkpoints diferencien pas real de pas aparent i la defensa tècnica es pot preparar sense carregar el tram final amb treball no tancat.
