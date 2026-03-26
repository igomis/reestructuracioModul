# Mapa de materials actuals -> transformació operativa

## Finalitat del document

Convertir els materials actuals del mòdul DWES en un mapa operatiu de transformació perquè cada bloc deixe de funcionar com a “tema tancat” i passe a donar servei directe als reptes del curs, amb evidències observables, ús verificable de la IA i coherència amb el projecte docent de reestructuració.

## Criteris d’ús del mapa

- el mapa s’utilitza per planificar la transformació de materials abans de redactar activitats o microtasques de repte
- cada bloc s’ha de vincular, com a mínim, amb un repte principal, un RA principal i una evidència concreta
- quan hi ha solapament, s’establix un únic bloc base i la resta queden com a reforç o suport tècnic
- les adaptacions de materials s’han de traduir en artefactes professionals: README, ADR, checklist, proves, documentació API, registre de debugging
- la IA s’integra com a assistent de treball i no com a substitut: tota proposta ha d’estar validada en codi, proves i defensa tècnica
- la priorització de transformació seguix el focus immediat del repositori: connectar cada repte amb materials adaptats prioritaris

## Taula general de correspondència

| Bloc de materials actuals | Repte/s associat/s | RA que ajuda a treballar | Ús dins del repte | Adaptació necessària | Paper possible de la IA | Observacions |
|---|---|---|---|---|---|---|
| Bloc 1. Arquitectures web | Repte 1 (principal), Repte 3 (reforç) | RA1, inici de RA5 | Justificar stack, entorn i decisions de kickoff; recuperar criteri arquitectònic en la refactorització MVC. | Reduir teoria enciclopèdica i convertir-la en guia de decisió amb ADR i criteris de trade-off. | Comparar alternatives, generar esborrany d’ADR i qüestionari de riscos tècnics. | Material d’entrada; una part passa de “tema” a “suport de decisió” reutilitzable en R1 i R3. |
| Bloc 2. PHP | Repte 2 (principal), Repte 3 (reforç), Repte 5 (manteniment puntual) | RA2, RA3, RA4 (reforç RA8) | Construir funcionalitat de servidor (formularis, validacions, sessions, autenticació) i mantindre-la quan el producte evoluciona. | Fusionar exercicis dispersos en una seqüència contínua de cas d’ús de producte (registre/login/perfil/logout). | Proposar casos de prova, detectar errors habituals de sessió i generar dades de test controlades. | Els apartats de sintaxi bàsica passen a “caixa d’eines” de suport, no a bloc principal autònom. |
| Blocs 3 i 4. Laravel MVC + dades | Repte 3 (principal), Repte 4 (reforç), Repte 5 (consolidació) | RA5, RA6 (reforç RA8 i RA7) | Refactoritzar a MVC, consolidar persistència segura i deixar preparada la capa de servei per a API. | Tractar 3 i 4 com un únic itinerari: arquitectura per capes, modelat de dades, validació i proves d’integració. | Assistir en refactorització guiada, generar esquelets de proves i revisar coherència entre models/controladors. | Nucli tècnic del mòdul; cal eliminar duplicació entre teoria MVC i accés a dades. |
| Bloc 5. Seguretat i reactivitat | Repte 3 (base de qualitat), Repte 5 (principal), reforç en Repte 2 i 4 | RA8 (reforç RA3, RA6 i RA7) | Aplicar hardening, debugging i testing sobre codi real en cada iteració del producte. | Redistribuir en dos nivells: mínims obligatoris per repte + paquet avançat per manteniment final. | Revisió de vulnerabilitats comunes, proposta de checklists i suport en reproducció d’errors. | Deixa de ser “tema final”: passa a eix transversal de control de qualitat i evidències. |
| Blocs 6a i 6b. APIs | Repte 4 (principal), Repte 5 (consolidació) | RA7 (reforç RA6 i RA9) | Publicar, documentar i provar endpoints; consumir APIs externes amb contractes clars. | Concentrar teoria HTTP comuna en una sola base i separar clarament publicació API vs consum/integració. | Esborrany de contractes OpenAPI, col·leccions de prova i verificació de coherència resposta/error. | Materials a fusionar parcialment; evitar repetir definicions bàsiques en 6a i 6b. |
| Bloc 7. Webs híbrides | Repte 5 (principal), Repte 4 (preparació) | RA9 (consolidació RA7 i RA8) | Integrar backend amb serveis externs i automatitzacions (n8n o equivalents) en escenari de manteniment realista. | Reorientar de “tema d’ampliació” a “cas integrador” amb flux de negoci complet i monitoratge bàsic. | Prototipar fluxos d’automatització, mapar payloads i generar escenaris de fallada per validació. | Material de tancament del producte evolutiu; exigix evidència tècnica, no només demo visual. |

## Desenvolupament per blocs

### Bloc 1. Arquitectures web

- objectiu de transformació: convertir teoria inicial en decisions tècniques justificades per al kickoff
- de “tema” a “suport tècnic”: comparatives d’arquitectura, plantilla d’ADR i checklist d’arrancada
- materials a fusionar/retallar: introduccions llargues repetides entre apunts d’arquitectura i orientacions de kickoff
- evidències d’ús: ADR, README executable, defensa tècnica curta de la decisió
- integració de IA: suport en comparativa de trade-offs, amb validació docent i justificació final de l’equip

### Bloc 2. PHP

- objectiu de transformació: passar d’exercicis separats a un flux funcional complet orientat a Repte 2
- de “tema” a “suport tècnic”: sintaxi i exemples bàsics com a repositori de consultes ràpides per debugging
- materials a fusionar/redistribuir: sessions i autenticació bàsica coordinades amb criteris de seguretat del Bloc 5
- evidències d’ús: commits funcionals, proves de validació, registre d’incidències resoltes
- integració de IA: suport en diagnòstic d’errors de peticions/sessions i proposta de tests reproduïbles

### Blocs 3 i 4. Laravel MVC + dades

- objectiu de transformació: establir una única ruta de migració a arquitectura mantenible amb persistència segura
- de “tema” a “suport tècnic”: patrons MVC i accés a dades com a guies de refactorització aplicada
- materials a fusionar/redistribuir: unificar explicacions de models, controladors, ORM i transaccions que ara apareixen duplicades
- evidències d’ús: estructura MVC coherent, proves d’integració de dades, justificació de decisions de capa
- integració de IA: assistència en refactorització, revisió de consultes i detecció de incoherències entre codi i model

### Bloc 5. Seguretat i reactivitat

- objectiu de transformació: convertir la seguretat/qualitat en pràctica contínua des de Repte 2 fins a Repte 5
- de “tema” a “suport tècnic”: checklists de seguretat, guies de debugging i pauta de regressió per iteració
- materials a fusionar/redistribuir: separar contingut base (R2-R3) de contingut avançat (R5) per evitar saturació inicial
- evidències d’ús: checklist completat, traça de debugging, correccions amb impacte mesurat
- integració de IA: anàlisi de vectors de risc i suggeriments de proves, sempre contrastats amb execució real

### Blocs 6a i 6b. APIs

- objectiu de transformació: definir un itinerari net de publicació i consum sense repetició de teoria bàsica
- de “tema” a “suport tècnic”: guia comuna de contracte API i guies específiques per productor/consumidor
- materials a fusionar/redistribuir: teoria HTTP, codis d’estat i errors en una base única; exemples separats per rol
- evidències d’ús: documentació d’API, proves d’endpoints, client de consum operatiu
- integració de IA: suport en drafts OpenAPI, col·leccions de proves i detecció de incoherències de contracte

### Bloc 7. Webs híbrides

- objectiu de transformació: convertir el bloc final en una integració de negoci executable sobre el backend del curs
- de “tema” a “suport tècnic”: patrons d’integració, gestió d’errors i monitoratge bàsic com a guies de manteniment
- materials a fusionar/redistribuir: connexió directa amb APIs del Bloc 6 i criteris de qualitat del Bloc 5
- evidències d’ús: workflow exportat, prova d’integració backend, registre de manteniment i defensa tècnica final
- integració de IA: suport en disseny de fluxos híbrids i simulació d’escenaris de fallada abans de la demo

## Repeticions o solapaments detectats

- solapament clar entre Blocs 3 i 4 en patrons MVC, modelat i accés a dades: convé tractar-los com una mateixa unitat de transformació
- repetició en Blocs 6a i 6b de teoria base d’API (verbs HTTP, codis d’estat, estructura de resposta): convé una única base comuna
- repetició parcial de sessions/autenticació entre Bloc 2 i Bloc 5: convé separar “implementació funcional” (B2) de “hardening i control” (B5)
- redundància entre introduccions generals de Bloc 1 i documentació de kickoff (README/ADR): convé deixar una sola peça de decisió tècnica

## Continguts que convé redistribuir

| Contingut actual | Origen principal | Destí recomanat | Acció de transformació |
|---|---|---|---|
| Teoria base HTTP i contractes de resposta | Blocs 6a i 6b | Repte 4 (base comuna) + suport Repte 5 | Fusionar en una fitxa única de contracte API i mantindre exemples separats per publicació/consum. |
| Sessions, autenticació i control d’accés | Bloc 2 + Bloc 5 | Repte 2 (implementació) + Repte 3/5 (hardening) | Mantindre el flux funcional en B2 i traslladar controls avançats a B5. |
| Introducció a decisions arquitectòniques | Bloc 1 | Repte 1 (kickoff) + reforç Repte 3 | Reduir teoria llarga i convertir-la en plantilla d’ADR + checklist de decisió. |
| Patrons MVC i persistència | Blocs 3 i 4 | Repte 3 (nucli) + reforç Repte 4 | Fusionar itineraris i evitar classes duplicades de concepte. |
| Integració amb serveis externs | Bloc 7 + Blocs 6a/6b | Repte 5 (nucli), amb prerequisit en Repte 4 | Reordenar perquè R4 deixe l’API preparada i R5 resolga el cas híbrid complet. |

### Materials que passen de “tema” a “suport tècnic”

- sintaxi i receptes bàsiques de PHP (Bloc 2) -> suport de consulta ràpida per incidències
- comparatives teòriques d’arquitectura (Bloc 1) -> suport per a decisions i defensa tècnica
- teoria repetida d’HTTP (Blocs 6a/6b) -> suport comú de contracte API
- checklists de seguretat i debugging (Bloc 5) -> suport transversal obligatori en tots els reptes
- patrons d’integració híbrida (Bloc 7) -> suport de manteniment i operació del producte final

## Prioritats de transformació de materials

1. **Prioritat alta (impacte immediat en focus del README):** Bloc 2 + Blocs 3-4, per connectar ràpidament Reptes 2 i 3 amb itineraris pràctics continus i evidències verificables.
2. **Prioritat alta (coherència d’avaluació per evidències):** Bloc 5, per convertir qualitat/seguretat en criteri transversal observable en repositori, proves i defensa.
3. **Prioritat mitjana-alta (obertura professional del producte):** Blocs 6a/6b, amb fusió de teoria comuna i separació operativa de publicació vs consum d’API.
4. **Prioritat mitjana (tancament integrador):** Bloc 7, orientat a un cas realista d’integració híbrida sobre backend ja madur.
5. **Prioritat de manteniment (simplificació curricular):** Bloc 1, retallant redundància teòrica i reforçant ús pràctic en decisions tècniques.

## Definition of done del document

Este mapa es considera completat quan:

- incorpora tots els blocs actuals prioritaris i els vincula amb reptes i RA de manera explícita
- la taula general inclou ús real, adaptació necessària, paper de la IA i observacions operatives
- identifica de forma explícita solapaments, materials a fusionar i continguts a redistribuir
- deixa documentat quins materials passen de “tema” a “suport tècnic”
- orienta la transformació cap a entorn professional realista i avaluació per evidències
- permet executar el següent pas de projecte: adaptar materials prioritaris per repte sense duplicacions
