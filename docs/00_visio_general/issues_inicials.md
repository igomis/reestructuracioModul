# Realineació del backlog d'issues

## Situació actual
- El backlog inicial de bootstrap ja ha quedat superat i les issues `#1` a `#6` s'han tancat perquè no representaven el focus real de la fase actual.
- Els documents base que originaven aquelles issues ja funcionen com a base usable del projecte:
  - `docs/03_avaluacio/rubrica_base_reptes.md`
  - `docs/02_reptes/repte_01_kickoff_backend.md`
  - `docs/04_materials/mapa_materials_actuals.md`
  - `docs/05_projectes_tecnics/projecte_base_backend.md`
- Les fitxes dels reptes 2, 4 i 5 ja tenen una base docent desenvolupada i el Repte 3 és ara la fitxa pendent més clara de consolidació.
- El següent focus útil del projecte és doble:
  - consolidar definitivament les fitxes dels reptes que ja tenen base
  - redactar l'enunciat base del projecte i planificar materials nous per repte

## Issues tancades en la realineació

### #1 A1-01 · Completar la rúbrica base de reptes
- **Estat:** tancada.
- **Motiu:** la rúbrica base ja està redactada i usable com a marc comú per als reptes del mòdul.

### #2 R1-01 · Completar la fitxa docent del Repte 1
- **Estat:** tancada.
- **Motiu:** la fitxa del Repte 1 ja està completada i és reutilitzable com a model per a la resta de reptes.

### #3 M1-01 · Completar el mapa de materials actuals
- **Estat:** tancada.
- **Motiu:** el mapa de materials ja està consolidat com a document operatiu i connecta blocs, reptes, RA i prioritats de transformació.

### #4 P1-01 · Consolidar el document de projecte backend base
- **Estat:** tancada.
- **Motiu:** el document de projecte backend base ja és prou madur per actuar com a referència del producte evolutiu del curs.

### #5 G1-01 · Crear issues reals a GitHub a partir del backlog
- **Estat:** tancada.
- **Motiu:** l'objectiu inicial ja havia quedat superat; la necessitat actual era realinear el backlog, no crear-lo des de zero.

### #6 R2-01 · Revisar i consolidar la fitxa docent del Repte 2
- **Estat:** tancada.
- **Motiu:** el Repte 2 ja està desenvolupat i no és el següent pas coherent de la fase actual.

## Issues noves recomanades

### R3-01 · Revisar i consolidar la fitxa docent del Repte 3
- **Prioritat:** alta
- **Objectiu:** portar el Repte 3 al mateix nivell de concreció docent que la resta de fitxes completes del projecte i estabilitzar la seua connexió amb el Repte 4.
- **Fitxers afectats:** `docs/02_reptes/repte_03_mvc_i_persistencia.md`
- **Definition of done:** fitxa revisada i consolidada, alineada amb RA5-RA6, qualitat tècnica, persistència i continuïtat cap al Repte 4.
- **Dependències:** `docs/03_avaluacio/rubrica_base_reptes.md`, `docs/05_projectes_tecnics/projecte_base_backend.md`.

### R4-01 · Revisar i consolidar la fitxa docent del Repte 4
- **Prioritat:** mitjana
- **Objectiu:** validar que la fitxa del Repte 4 queda integrada dins de la seqüència global i en coherència amb el Repte 5 i amb els materials d'API.
- **Fitxers afectats:** `docs/02_reptes/repte_04_api_i_consum.md`
- **Definition of done:** fitxa consolidada, amb contracte docent clar d'API, consum, proves, instruments i relació amb el producte base.
- **Dependències:** `R3-01`, `docs/04_materials/mapa_materials_actuals.md`.

### R5-01 · Revisar i consolidar la fitxa docent del Repte 5
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
1. Consolidar `R3-01`, perquè el Repte 3 continua sent la peça de transició arquitectònica central que convé estabilitzar.
2. Revisar `R4-01` i `R5-01` per deixar coherent la seqüència final dels reptes 3-5.
3. Redactar `PB-01` per disposar d'un enunciat base del projecte del curs coherent amb els reptes ja estabilitzats.
4. Executar `MG-01` per passar del mapa de materials a una planificació operativa de desenvolupament de materials nous.

## Definition of done de la realineació
Esta realineació es considera completada quan:
- el document deixa constància que el backlog inicial ha quedat superat
- les issues de bootstrap i `R2-01` ja no apareixen com a focus de treball actual
- el backlog actiu queda orientat a `R3-01`, `R4-01`, `R5-01`, `PB-01` i `MG-01`
- l'ordre recomanat de treball reflectix el focus real del repositori: consolidar reptes, redactar l'enunciat base i planificar materials nous
