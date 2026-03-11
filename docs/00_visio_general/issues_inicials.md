# Backlog inicial d’issues prioritzades

Este document recull les issues candidates per publicar a GitHub en format operatiu i ordenades per prioritat.

## Prioritat alta

### A1-01 Completar la rúbrica base de reptes
- **Objectiu:** disposar d’una rúbrica base reutilitzable per als reptes 1-5, alineada amb evidències autèntiques i ús verificable de la IA.
- **Fitxers afectats:** `docs/03_avaluacio/rubrica_base_reptes.md`.
- **Definition of done:** inclou dimensions comunes, nivells de domini, taula central amb pesos orientatius i criteris d’adaptació per repte.
- **Dependències:** `docs/00_visio_general/mapa_ra_reptes.md` validat i coherent amb la fase curricular.

### R1-01 Completar la fitxa docent del Repte 1
- **Objectiu:** tancar una fitxa docent completa i executable del kickoff backend com a model per a la resta de reptes.
- **Fitxers afectats:** `docs/02_reptes/repte_01_kickoff_backend.md`.
- **Definition of done:** incorpora context, encàrrec, microtasques, evidències, instruments, verificació de IA i definition of done del repte.
- **Dependències:** `docs/00_visio_general/mapa_ra_reptes.md` i `docs/01_programacio_modul/criteris_metodologics_reptes.md`.

### M1-01 Completar el mapa de materials actuals
- **Objectiu:** assegurar correspondència clara entre materials existents i reptes 1-5 per facilitar la planificació docent real.
- **Fitxers afectats:** `docs/04_materials/mapa_materials_actuals.md`.
- **Definition of done:** cada bloc de materials queda mapejat a reptes, ús didàctic i adaptació prevista sense duplicitats.
- **Dependències:** `docs/00_visio_general/mapa_modul_reptes.md` i `docs/00_visio_general/mapa_ra_reptes.md`.

### P1-01 Consolidar el document de projecte backend base
- **Objectiu:** establir el marc inicial del projecte tècnic backend com a línia de continuïtat del curs.
- **Fitxers afectats:** `docs/05_projectes_tecnics/projecte_base_backend.md`.
- **Definition of done:** document amb finalitat clara, límits de fase i orientacions de valor formatiu.
- **Dependències:** arquitectura curricular de fase 1 i seqüenciació general dels reptes.
- **Orientació futura:** en fase de projectes tècnics es valorarà una línia vinculada a “tokenitzar alguna cosa”, sense definir encara arquitectura ni implementació completa.

## Prioritat mitjana

### R2-01 Fitxa docent del Repte 2 (sessions i autenticació)
- **Objectiu:** definir la fitxa completa del repte orientada a RA2-RA4 en context backend real.
- **Fitxers afectats:** `docs/02_reptes/repte_02_sessions_i_autenticacio.md`.
- **Definition of done:** inclou encàrrec, seqüència, evidències, instrumentació i verificació d’IA amb criteri operatiu.
- **Dependències:** R1-01 i A1-01 tancades.

### R3-01 Fitxa docent del Repte 3 (MVC i persistència)
- **Objectiu:** concretar el repte de consolidació arquitectònica i persistència segura.
- **Fitxers afectats:** `docs/02_reptes/repte_03_mvc_i_persistencia.md`.
- **Definition of done:** fitxa completa amb focus en RA5-RA6 i qualitat backend (testing/debugging).
- **Dependències:** R2-01 tancada i rúbrica base disponible.

### R4-01 Fitxa docent del Repte 4 (API i consum)
- **Objectiu:** definir la unitat docent de publicació i consum d’API amb contractes clars.
- **Fitxers afectats:** `docs/02_reptes/repte_04_api_i_consum.md`.
- **Definition of done:** incorpora producte API verificable, evidències de proves d’endpoints i documentació tècnica.
- **Dependències:** R3-01 tancada i mapeig de materials revisat.

### R5-01 Fitxa docent del Repte 5 (integració híbrida i manteniment)
- **Objectiu:** tancar la fase de reptes amb integració externa, manteniment i defensa tècnica.
- **Fitxers afectats:** `docs/02_reptes/repte_05_integracio_hibrida_n8n.md`.
- **Definition of done:** fitxa completa amb focus en RA8-RA9, integració de IA verificable i tancament de producte evolutiu.
- **Dependències:** R4-01, A1-01 i P1-01.

## Prioritat de gestió

### G1-01 Crear issues reals a GitHub a partir del backlog
- **Objectiu:** convertir este backlog documental en issues publicades, assignables i traçables dins del repositori.
- **Fitxers afectats:** `docs/00_visio_general/issues_inicials.md` (font), GitHub Issues del repositori.
- **Definition of done:** issues creades a GitHub amb títol, descripció, checklist mínima, labels i prioritat; enllaçades als fitxers afectats.
- **Dependències:** revisió del backlog per part de coordinació del mòdul.

### G1-02 Planificar ordre d’execució i responsables
- **Objectiu:** establir ordre realista de treball entre avaluació, reptes, materials i projectes tècnics.
- **Fitxers afectats:** `docs/00_visio_general/issues_inicials.md`.
- **Definition of done:** cada issue prioritzada té responsable, data orientativa i bloquejos identificats.
- **Dependències:** G1-01 completada.

### G1-03 Revisar coherència transversal de fases
- **Objectiu:** verificar que els lliurables de reptes, rúbrica i materials mantenen alineació amb RA i criteris de IA.
- **Fitxers afectats:** `docs/00_visio_general/mapa_ra_reptes.md`, `docs/03_avaluacio/rubrica_base_reptes.md`, `docs/04_materials/mapa_materials_actuals.md`, fitxes de `docs/02_reptes/`.
- **Definition of done:** informe breu de coherència amb ajustos menors aplicats o issues noves obertes.
- **Dependències:** A1-01, R1-01 i M1-01.
