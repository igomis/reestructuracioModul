# Curs executable

## Finalitat

Este és el centre canònic per conduir el curs. Substitueix com a entrada principal el pla d'implantació, les calendaritzacions, la guia de 20 setmanes, la preparació docent directa i els kits de pilotatge.

Els documents de planificació continuen existint com a annexos o arxiu, però la decisió docent operativa ha de començar ací.

## Condicions de partida

- el curs està calibrat sobre unes `20` setmanes i `120` hores lectives aproximades
- el desenvolupament principal del projecte es tanca en dues avaluacions
- la tercera avaluació queda com a espai residual, connexió amb empresa o tancament puntual
- Git/GitHub funciona com a metodologia de treball i traçabilitat
- la IA s'usa com a suport verificable, no com a substitució de criteri tècnic
- els itineraris `Laravel`, `Express/Nest` i `FastAPI` són variants homologables del mateix model

## Seqüència executable

| Moment | Acció docent | Evidència mínima |
|---|---|---|
| Inici | presentar model, projecte base, dominis i criteris d'evidència | repositori inicial, README i criteri d'IA |
| Repte 1 | decidir domini, stack i esquelet tècnic | entorn funcional i primera decisió tècnica |
| Repte 2 | construir flux amb estat, sessions o autenticació | funcionalitat protegida, validacions i proves bàsiques |
| Repte 3 | estabilitzar arquitectura i persistència | model de dades, capes o equivalent, regressió mínima |
| Repte 4 | exposar i consumir API | contracte, endpoints, proves i documentació |
| Repte 5 | integrar servei extern, n8n o flux híbrid | integració funcional i prova de punta a punta |
| Defensa | verificar autoria i criteri tècnic | defensa individual, evidències finals i repo coherent |

## Materials que s'activen

- inici: [visió del model](visio-model-dwes.md), [enunciat base](05_projectes_tecnics/enunciat_projecte_base.md), [sistema d'evidències](03_avaluacio/sistema_evidencies.md)
- conducció: [projecte backend base](05_projectes_tecnics/projecte_base_backend.md) i fitxes dels reptes
- suport d'aula: [recursos d'aula](04_materials/index.md)
- seguiment: [instruments de seguiment](03_avaluacio/instruments_seguiment_docent.md), checklists i plantilles
- tancament: [rúbrica de defensa tècnica](03_avaluacio/rubrica_defensa_tecnica.md)

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
- si la integració final no és verificable, es retalla abast abans de la defensa

## Criteri de tancament

El curs queda executable quan el producte final és recognoscible, el repositori mostra procés real, les evidències expliquen el treball i l'alumnat pot defensar decisions tècniques pròpies amb ús d'IA verificable.
