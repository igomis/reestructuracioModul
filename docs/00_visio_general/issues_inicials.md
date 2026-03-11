# Backlog operatiu d’issues prioritzades

## Estat actual del projecte
- La Fase 1 curricular està documentada i disponible com a base de treball.
- Encara no hi ha issues reals obertes a GitHub per executar el backlog.
- Els punts més incomplets i bloquejants per avançar en fase de reptes són:
  - `docs/03_avaluacio/rubrica_base_reptes.md`
  - `docs/02_reptes/repte_01_kickoff_backend.md`
  - `docs/04_materials/mapa_materials_actuals.md`
  - `docs/05_projectes_tecnics/projecte_base_backend.md`

## Criteri de priorització
- **Prioritat alta:** documents que desbloquegen directament disseny de reptes i avaluació.
- **Prioritat mitjana:** continuació natural una vegada tancats els mínims del primer repte.
- **Prioritat de gestió:** tasques de coordinació per convertir backlog en execució real a GitHub.

## Issues prioritàries per crear ja a GitHub

### A1-01 · Completar la rúbrica base de reptes
- **Prioritat:** alta
- **Objectiu:** disposar d’una rúbrica comuna per als reptes 1-5, basada en evidències observables i ús verificable de la IA.
- **Fitxers afectats:** `docs/03_avaluacio/rubrica_base_reptes.md`
- **Definition of done:** inclou dimensions comunes, nivells de domini, pesos orientatius, taula central i criteris d’adaptació per repte.
- **Dependències:** `docs/00_visio_general/mapa_ra_reptes.md` validat.

### R1-01 · Completar la fitxa docent del Repte 1
- **Prioritat:** alta
- **Objectiu:** convertir el Repte 1 en una fitxa docent completa i reutilitzable com a model per als reptes següents.
- **Fitxers afectats:** `docs/02_reptes/repte_01_kickoff_backend.md`
- **Definition of done:** inclou context, encàrrec, seqüència, microtasques, evidències, instruments d’avaluació, verificació de IA i definition of done.
- **Dependències:** `docs/00_visio_general/mapa_ra_reptes.md`, `docs/01_programacio_modul/criteris_metodologics_reptes.md`.

### M1-01 · Completar el mapa de materials actuals
- **Prioritat:** alta
- **Objectiu:** deixar tancada la relació entre materials actuals i reptes per facilitar aplicació docent real.
- **Fitxers afectats:** `docs/04_materials/mapa_materials_actuals.md`
- **Definition of done:** cada bloc de materials queda mapejat a reptes, ús didàctic i acció d’adaptació prevista, sense duplicacions.
- **Dependències:** `docs/00_visio_general/mapa_modul_reptes.md`, `docs/00_visio_general/mapa_ra_reptes.md`.

### P1-01 · Consolidar el projecte backend base
- **Prioritat:** alta
- **Objectiu:** definir el marc mínim del projecte tècnic backend que done continuïtat als reptes del curs.
- **Fitxers afectats:** `docs/05_projectes_tecnics/projecte_base_backend.md`
- **Definition of done:** document amb finalitat, abast inicial i línies didàctiques de treball sense detall d’arquitectura completa.
- **Dependències:** seqüenciació general del mòdul i criteris de fase 1.
- **Nota de futur:** en la fase de projectes tècnics es valorarà una possible línia vinculada a “tokenitzar alguna cosa”, sempre amb enfocament backend i valor didàctic, sense desplegar encara el projecte complet.

## Issues de continuació

### R2-01 · Fitxa docent del Repte 2 (sessions i autenticació)
- **Prioritat:** mitjana
- **Objectiu:** definir fitxa completa del repte amb focus en RA2-RA4.
- **Fitxers afectats:** `docs/02_reptes/repte_02_sessions_i_autenticacio.md`
- **Definition of done:** fitxa completa amb encàrrec, activitats, evidències i verificació d’IA.
- **Dependències:** R1-01, A1-01.

### R3-01 · Fitxa docent del Repte 3 (MVC i persistència)
- **Prioritat:** mitjana
- **Objectiu:** concretar el repte de consolidació arquitectònica i persistència segura.
- **Fitxers afectats:** `docs/02_reptes/repte_03_mvc_i_persistencia.md`
- **Definition of done:** fitxa completa amb focus en RA5-RA6, qualitat de codi i validació tècnica.
- **Dependències:** R2-01, A1-01.

### R4-01 · Fitxa docent del Repte 4 (API i consum)
- **Prioritat:** mitjana
- **Objectiu:** definir unitat docent d’API publicable i consumible amb criteris de documentació i proves.
- **Fitxers afectats:** `docs/02_reptes/repte_04_api_i_consum.md`
- **Definition of done:** fitxa completa amb evidències de contracte API, proves d’endpoints i consum.
- **Dependències:** R3-01, M1-01.

### R5-01 · Fitxa docent del Repte 5 (integració híbrida i manteniment)
- **Prioritat:** mitjana
- **Objectiu:** tancar la seqüència de reptes amb integració externa, manteniment i defensa tècnica.
- **Fitxers afectats:** `docs/02_reptes/repte_05_integracio_hibrida_n8n.md`
- **Definition of done:** fitxa completa amb focus en RA8-RA9 i evidències finals de producte evolutiu.
- **Dependències:** R4-01, P1-01, A1-01.

## Pas de gestió immediat

### G1-01 · Crear issues reals a GitHub a partir del backlog
- **Prioritat:** gestió
- **Objectiu:** traslladar este backlog a issues reals de GitHub amb assignació i seguiment.
- **Fitxers afectats:** `docs/00_visio_general/issues_inicials.md` (origen del backlog) + GitHub Issues del repositori.
- **Definition of done:** issues creades a GitHub per A1-01, R1-01, M1-01, P1-01, R2-01, R3-01, R4-01 i R5-01 amb labels de prioritat i dependències.
- **Dependències:** validació interna del backlog per coordinació del mòdul.
