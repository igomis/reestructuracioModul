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
| Repte 1 | arrencada funcional del backend | entorn executable, Docker, punt d'entrada i primera decisió tècnica |
| Repte 2 | primera funcionalitat protegida | checkpoint `R1 -> R2`, flux autenticat, validacions i proves bàsiques |
| Repte 3 | reconstrucció en framework i persistència | dos fluxos end-to-end, model de dades, migracions, seeders i proves mínimes |
| Repte 4 | publicació i consum d'API | contracte, endpoints, consum verificat i documentació d'API |
| Repte 5 | integració híbrida | funcionalitat integrada, tractament d'errors i prova de punta a punta |
| Defensa tècnica | tancament del curs | evidències finals, repositori coherent i defensa tècnica individual |

## Checkpoints i moments de revisió

- inici de curs: activació del repositori i comprovació del marc de treball
- tancament de `R1`: verificació de base executable
- pas `R1 -> R2`: comprovació de flux de dades i entrada a funcionalitat protegida
- tancament de `R2`: funcionalitat protegida reproduïble i codi mínimament ordenat
- tancament de `R3`: persistència real i dos fluxos end-to-end
- tancament de `R4`: API usable i consum verificat
- tancament de `R5`: integració híbrida amb valor funcional
- defensa tècnica final: tancament individual del producte i de les evidències

## Documents operatius que s'activen

- [Visió del model](visio-model-dwes.md): només com a marc general
- [Enunciat base del projecte](05_projectes_tecnics/enunciat_projecte_base.md): encàrrec del producte
- [Projecte backend base](05_projectes_tecnics/projecte_base_backend.md): base tècnica comuna
- [Reptes 1-5](02_reptes/repte_01_kickoff_backend.md): desplegament del curs per reptes
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
- si `R3` no deixa persistència i arquitectura explicables, no s'obri `R4`
- si `R4` no està documentat ni provat, no s'avança cap a `R5`
- si la integració final no és verificable, es retalla abast abans de la defensa tècnica

## Criteri de tancament

El curs queda executable quan el producte final és recognoscible, el calendari permet tancar `R1-R5` dins de dues avaluacions, els checkpoints diferencien pas real de pas aparent i la defensa tècnica es pot preparar sense carregar el tram final amb treball no tancat.
