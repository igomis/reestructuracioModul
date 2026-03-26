# Fase 1. Arquitectura curricular del mòdul DWES

## Finalitat de la fase

Establir l’arquitectura curricular del mòdul DWES en una seqüència de 5 reptes connectats, mantenint la cobertura completa del currículum i incorporant ús habitual però verificable de la IA en un context professional backend.

## Objectius específics

- definir un fil conductor únic per a tot el curs basat en un producte backend evolutiu
- distribuir els RA del mòdul en reptes principals i espais de reforç
- concretar criteris metodològics comuns per a tots els reptes
- fixar criteris de verificació de l’ús de la IA vinculats a l’avaluació
- assegurar la coherència entre programació, reptes, avaluació i materials

## Decisions estructurals adoptades

- s’organitza el curs en 5 reptes consecutius amb dependències explícites
- cada repte té finalitat, producte i evidències observables
- els RA1-RA9 es mantenen íntegrament, sense eliminacions
- Git, debugging, testing, documentació i APIs es tracten com a eixos transversals
- la IA es considera una eina de suport professional, mai una substitució de comprensió

## Mapa general dels reptes

| Repte | Nom | Finalitat | RA principals | Producte clau |
|---|---|---|---|---|
| 1 | Kickoff tècnic d’un servei web backend | Preparar base tècnica i decisions inicials del projecte. | RA1, inici de RA5 | Repo base funcional + README tècnic + ADR inicial. |
| 2 | Mòdul de gestió d’usuaris i sessions | Implementar funcionalitat dinàmica amb autenticació i estat. | RA2, RA3, RA4 | Mòdul d’usuaris/sessions operatiu i testable. |
| 3 | Migració a MVC i persistència segura | Escalar a arquitectura mantenible amb dades persistents. | RA5, RA6, RA8 | Backend MVC amb capa de dades i proves de regressió. |
| 4 | Publicació i consum d’API | Obrir el producte a integració mitjançant API documentada. | RA7, reforç de RA6 | API REST documentada + client de consum. |
| 5 | Integració híbrida, automatització i manteniment | Consolidar integracions externes i sostenibilitat del producte. | RA9, reforç de RA7 i RA8 | Integració híbrida (n8n/serveis externs) + pla de manteniment. |

## Correspondència general amb resultats d’aprenentatge

- RA1: punt d’entrada al Repte 1.
- RA2-RA4: nucli funcional del Repte 2.
- RA5-RA6: consolidació arquitectònica al Repte 3.
- RA7: desplegament i contracte de serveis al Repte 4.
- RA8: control de qualitat i seguretat transversal, amb focus al Repte 3.
- RA9: integració híbrida i automatització al Repte 5.

## Paper transversal de la IA

La IA s’utilitza durant tot el curs per accelerar tasques de comparativa tècnica, generació de base de codi, debugging, tests i documentació. L’ús sempre queda condicionat a:

- registre mínim d’interaccions (AI log)
- justificació de decisions adoptades
- validació tècnica amb proves i execució real
- defensa individual del que s’ha implementat

## Entorn professional com a eix transversal

L’activitat de tots els reptes es dissenya en clau d’entorn backend real:

- repositori Git amb commits significatius, branques i revisió
- ús sistemàtic de debugging i proves
- documentació tècnica operativa (README, API docs, decisions)
- treball amb APIs com a part del flux normal del producte
- gestió d’incidències i millores mitjançant issues

## Resultats esperats de la fase

- arquitectura curricular consensuada i documentada
- seqüenciació general de 5 reptes amb dependències clares
- mapa complet RA -> reptes -> evidències -> instruments
- criteris metodològics i criteris de verificació de IA publicats
- backlog inicial d’issues menudes per executar la Fase 2

## Dependències cap a la fase 2

La Fase 2 depén d’esta arquitectura per completar la fitxa de cada repte amb:

- context professional i enunciat operatiu
- activitats guiades i activitats de consolidació
- evidències obligatòries i rúbrica específica
- connexió detallada amb materials i projectes tècnics
