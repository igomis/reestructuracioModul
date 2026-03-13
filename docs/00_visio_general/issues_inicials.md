# Realineació del backlog d'issues

## Situació actual
- El backlog inicial responia a una fase de bootstrap del projecte docent i ja no descriu bé l'estat real del repositori.
- Els documents base que originaven les primeres issues han avançat de manera significativa i, en diversos casos, ja funcionen com a base usable del projecte:
  - `docs/03_avaluacio/rubrica_base_reptes.md`
  - `docs/02_reptes/repte_01_kickoff_backend.md`
  - `docs/04_materials/mapa_materials_actuals.md`
  - `docs/05_projectes_tecnics/projecte_base_backend.md`
- El focus actual del projecte no és completar el bootstrap inicial, sinó consolidar les fitxes de reptes pendents o recentment tancades, redactar l'enunciat base del projecte del curs i planificar materials nous prioritaris per repte.
- En conseqüència, les issues obertes de la fase inicial han quedat desfasades i convé substituir-les per un backlog orientat a la fase actual del projecte docent DWES.

## Proposta de tancament d'issues existents

### #5 G1-01 · Crear issues reals a GitHub a partir del backlog
- **Proposta:** tancar.
- **Motiu:** l'objectiu inicial ja ha quedat superat; el repositori ja treballa amb issues reals i ara cal realinear-les, no crear-les des de zero.

### #1 A1-01 · Completar la rúbrica base de reptes
- **Proposta:** tancar.
- **Motiu:** la rúbrica base ja està redactada i usable com a marc comú per als reptes del mòdul.

### #2 R1-01 · Completar la fitxa docent del Repte 1
- **Proposta:** tancar.
- **Motiu:** la fitxa del Repte 1 ja està completada i és reutilitzable com a model per a la resta de reptes.

### #3 M1-01 · Completar el mapa de materials actuals
- **Proposta:** tancar.
- **Motiu:** el mapa de materials ja està consolidat com a document operatiu i connecta blocs, reptes, RA i prioritats de transformació.

### #4 P1-01 · Consolidar el document de projecte backend base
- **Proposta:** tancar.
- **Motiu:** el document de projecte backend base ja està prou madur per actuar com a referència del producte evolutiu del curs.

## Issues noves recomanades

### R2-01 · Revisar i consolidar la fitxa docent del Repte 2
- **Prioritat:** mitjana-alta
- **Objectiu:** revisar la fitxa del Repte 2 per assegurar coherència final amb Repte 3, avaluació i materials associats.
- **Fitxers afectats:** `docs/02_reptes/repte_02_sessions_i_autenticacio.md`
- **Definition of done:** fitxa revisada, coherent amb el projecte base, amb enllaços i formulacions alineades amb la seqüència actual de reptes.
- **Dependències:** tancament formal de `#2 R1-01`, `#1 A1-01` i `#3 M1-01`.

### R3-01 · Completar la fitxa docent del Repte 3
- **Prioritat:** alta
- **Objectiu:** portar el Repte 3 al mateix nivell de concreció docent que la resta de fitxes completes del projecte.
- **Fitxers afectats:** `docs/02_reptes/repte_03_mvc_i_persistencia.md`
- **Definition of done:** fitxa completa, revisada i alineada amb RA5-RA6, qualitat tècnica, persistència i continuïtat cap al Repte 4.
- **Dependències:** `R2-01`, `docs/03_avaluacio/rubrica_base_reptes.md`, `docs/05_projectes_tecnics/projecte_base_backend.md`.

### R4-01 · Consolidar la fitxa docent del Repte 4
- **Prioritat:** mitjana
- **Objectiu:** validar que la fitxa del Repte 4 queda integrada dins de la seqüència global i en coherència amb el Repte 5 i amb els materials d'API.
- **Fitxers afectats:** `docs/02_reptes/repte_04_api_i_consum.md`
- **Definition of done:** fitxa consolidada, amb contracte docent clar d'API, consum, proves, instruments i relació amb el producte base.
- **Dependències:** `R3-01`, `docs/04_materials/mapa_materials_actuals.md`.

### R5-01 · Completar la fitxa docent del Repte 5
- **Prioritat:** mitjana
- **Objectiu:** validar i ajustar la fitxa del Repte 5 com a tancament coherent del producte evolutiu del curs.
- **Fitxers afectats:** `docs/02_reptes/repte_05_integracio_hibrida_n8n.md`
- **Definition of done:** fitxa completada i alineada amb RA9, integració híbrida, manteniment i materials de bloc 7.
- **Dependències:** `R4-01`, `docs/05_projectes_tecnics/integracio_n8n.md`.

### PB-01 · Redactar l’enunciat base del projecte del curs
- **Prioritat:** alta
- **Objectiu:** transformar el projecte backend base en un enunciat docent usable com a peça transversal del curs.
- **Fitxers afectats:** document nou o derivat dins de `docs/05_projectes_tecnics/`
- **Definition of done:** enunciat base redactat amb context, requisits mínims, dominis possibles, criteris d'evidència i connexió amb els reptes 2-5.
- **Dependències:** `docs/05_projectes_tecnics/projecte_base_backend.md`, `R3-01`, `R4-01`, `R5-01`.

### MG-01 · Planificar materials nous prioritaris per repte
- **Prioritat:** alta
- **Objectiu:** concretar el següent paquet de materials nous o adaptats que el projecte necessita per passar de mapa general a planificació executable.
- **Fitxers afectats:** principalment `docs/04_materials/` i documents de suport relacionats
- **Definition of done:** llistat prioritzat de materials per repte, criteri de transformació i seqüència de treball per fases.
- **Dependències:** `docs/04_materials/mapa_materials_actuals.md`, `PB-01`, estat consolidat de `R3-01`, `R4-01` i `R5-01`.

## Ordre recomanat de treball
1. Tancar formalment les issues inicials desfasades: `#5`, `#1`, `#2`, `#3` i `#4`.
2. Obrir i abordar `R2-01` com a revisió ràpida de coherència sobre una fitxa ja avançada.
3. Completar `R3-01`, perquè el Repte 3 encara actua com a peça de transició arquitectònica central.
4. Consolidar `R4-01` i `R5-01` per deixar tancada la seqüència completa dels reptes 1-5.
5. Redactar `PB-01` per disposar d'un enunciat base del projecte del curs coherent amb les fitxes ja estabilitzades.
6. Executar `MG-01` per passar del mapa de materials a una planificació operativa de desenvolupament de materials nous.

## Definition of done de la realineació
Esta realineació es considera completada quan:
- el document deixa constància que el backlog inicial ha quedat desfasat i explica per què
- s'identifica explícitament quines issues existents convé tancar i amb quin motiu
- es proposa un nou backlog d'issues alineat amb la fase actual del projecte docent
- l'ordre recomanat de treball reflectix el focus real del repositori: consolidar reptes, redactar l'enunciat base i planificar materials nous
- les noves issues recomanades poden traslladar-se directament a GitHub sense redissenyar el backlog
