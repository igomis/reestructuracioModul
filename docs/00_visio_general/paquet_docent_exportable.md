# Paquet docent exportable del mòdul

## Finalitat del document

Definir què constitueix el paquet docent complet del mòdul una vegada tancada la fase de reestructuració, materials, itineraris, implantació i seguiment, de manera que el treball realitzat es puga reutilitzar com a conjunt coherent i no només com a suma de documents independents.

Este document no torna a descriure el curs peça per peça, sinó que fixa quins blocs formen el paquet docent, quins són imprescindibles, quins són adaptables i com hauria de llegir-los o activar-los un docent que vulga implantar el model.

## Què forma part del paquet docent del mòdul

| Bloc del paquet | Peces principals | Funció dins del model |
|---|---|---|
| **Visió general** | `mapa_modul_reptes.md`, `mapa_ra_reptes.md`, `issues_inicials.md` | donar lectura global del model, del seu encaix i de l'estat real de producció |
| **Projecte base i context tècnic** | `enunciat_projecte_base.md`, documents de `docs/05_projectes_tecnics/` | fixar l'encàrrec base del producte del curs i el marc tècnic de referència |
| **Reptes del curs** | fitxes de `docs/02_reptes/` | ordenar el desenvolupament del curs com a seqüència de reptes amb producte real |
| **Materials comuns** | `docs/04_materials/materials_comuns/` | normalitzar metodologia, documentació, proves, debugging i ús verificable de la IA |
| **Materials per repte** | `docs/04_materials/repte_02/`, `repte_03/`, `repte_04/`, `repte_05/` | donar suport tècnic operatiu als punts crítics de cada repte |
| **Itineraris tecnològics** | `docs/04_materials/itineraris/laravel/`, `express_nest/`, `fastapi/` | permetre implementar el mateix model docent en stacks diferents sense canviar exigència |
| **Implantació docent** | `pla_implantacio_docent.md`, `calendaritzacio_orientativa_aula.md`, `calendaritzacio_per_avaluacions.md`, `programacio_aula_operativa_2_avaluacions.md`, `seqüenciacio_sessions_2_avaluacions.md`, `curs_executable_dwes_2_avaluacions.md` | convertir el model en seqüència real de curs en dues avaluacions |
| **Avaluació i seguiment** | `matriu_evidencies_i_instruments_per_fase.md`, `instruments_seguiment_docent.md`, rúbriques, checklists i plantilles | controlar evidències, checkpoints, progrés real i defensa tècnica |
| **Plantilles reutilitzables** | `docs/06_plantilles/` | facilitar adaptació, replicació i creació de noves peces a partir d'un patró comú |

## Quines peces són imprescindibles

Sense estes peces el model no és realment implantable:

- [enunciat_projecte_base.md](../05_projectes_tecnics/enunciat_projecte_base.md) com a encàrrec base del producte
- fitxes de reptes com a seqüència obligatòria del curs
- materials comuns del mòdul
- materials nuclears dels Reptes `2`, `3`, `4` i `5`
- almenys un itinerari tecnològic usable, encara que el model ideal en manté tres
- [pla_implantacio_docent.md](../01_programacio_modul/pla_implantacio_docent.md)
- [calendaritzacio_per_avaluacions.md](../01_programacio_modul/calendaritzacio_per_avaluacions.md)
- [curs_executable_dwes_2_avaluacions.md](../01_programacio_modul/curs_executable_dwes_2_avaluacions.md)
- [matriu_evidencies_i_instruments_per_fase.md](../03_avaluacio/matriu_evidencies_i_instruments_per_fase.md)
- [instruments_seguiment_docent.md](../03_avaluacio/instruments_seguiment_docent.md)

Lectura pràctica:

- si falta projecte base, seqüència per reptes, curs executable o sistema de seguiment, el paquet queda incomplet
- la resta de peces milloren robustesa, adaptació i transferibilitat

## Quines peces són adaptables

Estes peces poden canviar sense trencar el nucli del model:

- domini concret del producte, sempre que es mantinguen els dominis admesos o una lògica equivalent
- itinerari tecnològic concret, sempre que es mantinguen exigències homologables
- detall de calendarització fina segons la càrrega real del centre
- profunditat o format dels materials complementaris
- forma específica de checkpoints, sempre que no desaparega el seguiment basat en evidències
- distribució en dues avaluacions o equivalent, sempre que el desenvolupament principal continue tancant-se abans de la fase no lectiva o de pràctiques externes

## Ordre recomanat de lectura o ús per al professorat

1. Llegir [paquet_docent_exportable.md](paquet_docent_exportable.md) per entendre què s'està adoptant.
2. Llegir [enunciat_projecte_base.md](../05_projectes_tecnics/enunciat_projecte_base.md) per fixar l'encàrrec del producte.
3. Llegir [pla_implantacio_docent.md](../01_programacio_modul/pla_implantacio_docent.md) i [calendaritzacio_per_avaluacions.md](../01_programacio_modul/calendaritzacio_per_avaluacions.md) per entendre l'estructura temporal.
4. Passar a [curs_executable_dwes_2_avaluacions.md](../01_programacio_modul/curs_executable_dwes_2_avaluacions.md) com a peça principal d'ús docent real.
5. Revisar [instruments_seguiment_docent.md](../03_avaluacio/instruments_seguiment_docent.md) i les plantilles de seguiment abans d'iniciar el curs.
6. Activar materials comuns i després materials per repte segons la seqüència docent.
7. Seleccionar o permetre itineraris `Laravel`, `Express/Nest` o `FastAPI` sense alterar el nivell d'exigència.

## Què necessita un docent per implantar-lo

- entendre que el model està calibrat sobre `20` setmanes, `6` hores setmanals i unes `120` hores lectives aproximades
- assumir que el projecte s'ha de completar dins de les dues primeres avaluacions
- compartir des de l'inici el criteri que Git/GitHub és metodologia de treball i traçabilitat, no iniciació bàsica
- tindre visible el projecte base, els reptes, els materials i els instruments de seguiment abans de començar
- decidir com s'organitzaran equips, checkpoints i revisió d'evidències
- triar si es treballarà amb un únic itinerari o amb diversos itineraris tecnològics simultanis
- estar disposat a fer seguiment real del repositori, documentació, proves i ús verificable de la IA

## Què es pot exportar a altres mòduls

El que és més reutilitzable no és el contingut tècnic concret de DWES, sinó el patró docent:

- seqüència de treball per reptes amb producte base comú
- model d'evidències autèntiques i seguiment per checkpoints
- separació entre materials comuns, materials per repte i variants tecnològiques
- tractament de la IA com a eina guiada i verificable
- ús del repositori com a prova de procés i no només com a contenidor
- capa d'implantació docent escalonada: pla, calendarització, programació, seqüenciació i curs executable
- paquet d'instruments finals de seguiment docent

## Limitacions i punts a contextualitzar

- este paquet està pensat per a un context on la 3a avaluació no és central perquè l'alumnat està en empresa o `FCT`
- el model assumix base prèvia en Git/GitHub; si el grup no la té, caldria obrir una capa d'alfabetització que ací no està contemplada
- els itineraris actuals responen a `Laravel`, `Express/Nest` i `FastAPI`; altres stacks requeririen una adaptació explícita
- el calendari està calibrat a `120` hores aproximades; si la càrrega baixa molt, caldrà retallar abast sense tocar el nucli del model
- el paquet és exportable, però no automàticament transplantable: cada centre ha de contextualitzar horari, resultats d'aprenentatge, autonomia de l'alumnat i marge real de seguiment

## Definition of done del paquet

El paquet docent es considera completat quan:

- es pot descriure com un conjunt coherent i no com una suma d'arxius independents
- deixa clar què és imprescindible i què és adaptable
- ofereix un ordre de lectura o adopció usable per al professorat
- identifica què cal tindre preparat per implantar el model
- explicita què és exportable a altres mòduls i què depén del context de DWES
- manté el nucli del repositori: treball per reptes, entorn professional realista, evidències autèntiques i IA verificable
