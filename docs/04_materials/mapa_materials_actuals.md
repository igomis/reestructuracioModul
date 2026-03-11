# Mapa de materials actuals -> nova estructura

## Finalitat del document
Convertir els materials actuals del mòdul DWES en un mapa operatiu que permeta planificar, adaptar i reutilitzar continguts dins del model de treball per reptes, mantenint coherència amb els RA, l’entorn professional backend i l’ús verificable de la IA.

## Criteris d’ús del mapa
- cada bloc de materials s’ha de connectar almenys amb un repte i un RA principal
- els materials deixen de funcionar com a “tema tancat” i passen a ser suport tècnic per resoldre reptes
- s’evita duplicar explicacions; quan hi ha solapament, es defineix bloc principal i bloc de reforç
- l’ús de la IA s’integra com a suport de treball, sempre amb verificació tècnica (proves, repo, documentació, defensa)
- la transformació de materials prioritza transferència al producte evolutiu del curs

## Taula general de correspondència

| Bloc de materials actuals | Repte/s associat/s | RA que ajuda a treballar | Ús dins del repte | Adaptació necessària | Paper possible de la IA | Observacions |
|---|---|---|---|---|---|---|
| Bloc 1. Arquitectures web | Repte 1 (principal), Repte 3 (reforç) | RA1, inici de RA5 | Comparar alternatives, justificar stack i definir base d’arquitectura inicial. | Passar d’exercicis teòrics a ADR i decisions tècniques de kickoff. | Comparativa guiada d’alternatives i síntesi de trade-offs. | Material clau d’entrada; convé reduir teoria repetida i augmentar aplicació directa. |
| Bloc 2. PHP | Repte 2 (principal) | RA2, RA3, RA4 | Implementar lògica de servidor, formularis, sessions i autenticació inicial. | Integrar activitats disperses en casos d’ús continus de producte. | Suport en snippets, debugging de peticions i generació de dades de prova. | Part del contingut passa de “tema” a “caixa d’eines” reutilitzable en reptes posteriors. |
| Blocs 3 i 4. Laravel MVC + dades | Repte 3 (principal), Repte 4 (reforç) | RA5, RA6, reforç de RA7 | Consolidar arquitectura MVC, persistència i base de serveis per API. | Fusionar pedagògicament en un únic itinerari de backend mantenible. | Ajuda en refactorització guiada, estructura de capes i proves bàsiques. | És el nucli tècnic del curs; cal eliminar duplicitats entre conceptes MVC i accés a dades. |
| Bloc 5. Seguretat i reactivitat | Repte 3 (reforç), Repte 5 (principal) | RA8, reforç de RA3 i RA6 | Aplicar mesures de seguretat, qualitat i estabilitat sobre codi ja funcional. | Redistribuir contingut: una part al control de qualitat (R3) i una part a manteniment/integració (R5). | Revisió de vulnerabilitats, propostes de tests i checklist de hardening. | Evitar tractar-lo com a bloc final aïllat; ha d’aparéixer en iteracions curtes. |
| Blocs 6a i 6b. APIs | Repte 4 (principal), Repte 5 (reforç) | RA7, reforç de RA6 i RA9 | Dissenyar, publicar, documentar i provar endpoints; preparar integracions externes. | Delimitar via principal (publicació API) i via complementària (consum/integració). | Suport en documentació d’API, exemples de contractes i generació de col·leccions de prova. | Cal evitar repetició de teoria HTTP entre 6a i 6b; concentrar-ho en pràctica d’endpoints. |
| Bloc 7. Webs híbrides | Repte 5 (principal) | RA9, consolidació de RA7 | Integrar serveis externs i fluxos híbrids en un escenari de manteniment realista. | Reorientar a casos de negoci concrets amb evidència d’integració backend. | Assistència per prototipar fluxos d’automatització i validar escenaris d’integració. | Passa de bloc especialitzat a tancament integrador del producte evolutiu. |

## Desenvolupament per blocs

### Bloc 1. Arquitectures web
- **Paper didàctic:** bloc de decisió inicial per al kickoff tècnic.
- **Transformació clau:** de teoria d’arquitectures a justificació aplicada (ADR, elecció de stack, conseqüències tècniques).
- **Evidències recomanades:** ADR, README de posada en marxa, defensa curta de decisió.

### Bloc 2. PHP
- **Paper didàctic:** bloc d’implementació funcional de servidor en context real.
- **Transformació clau:** de col·lecció d’exercicis independents a flux funcional continu (formulari -> validació -> sessió -> resposta).
- **Evidències recomanades:** commits de funcionalitats, proves bàsiques, incidències resoltes.

### Blocs 3 i 4. Laravel MVC + dades
- **Paper didàctic:** nucli d’arquitectura professional i persistència.
- **Transformació clau:** tractar-los com un únic itinerari de refactorització, modelat de dades i mantenibilitat.
- **Evidències recomanades:** estructura MVC, proves d’integració de dades, revisió de qualitat del codi.

### Bloc 5. Seguretat i reactivitat
- **Paper didàctic:** eix de qualitat transversal, no tema aïllat.
- **Transformació clau:** repartir continguts entre controls preventius (R3) i manteniment evolutiu (R5).
- **Evidències recomanades:** checklist de seguretat, registre de debugging, correccions justificades.

### Blocs 6a i 6b. APIs
- **Paper didàctic:** obertura del producte backend a consum extern.
- **Transformació clau:** separar clarament “publicació” i “consum/integració” sense duplicar teoria bàsica.
- **Evidències recomanades:** documentació d’API, proves d’endpoints, client de consum funcional.

### Bloc 7. Webs híbrides
- **Paper didàctic:** tancament del curs amb integració externa i visió de producte.
- **Transformació clau:** de bloc de contingut final a capítol d’integració real sobre backend existent.
- **Evidències recomanades:** demo d’integració, registre de manteniment, defensa tècnica final.

## Repeticions o solapaments detectats
- solapament entre Blocs 3 i 4 en explicació de patrons MVC i capa de dades
- repetició de contingut conceptual entre Blocs 6a i 6b (definició d’endpoint, verbs HTTP, estructures de resposta)
- reiteració de contingut de sessions/autenticació entre Bloc 2 i Bloc 5 sense criteri de progressió
- duplicació de documentació introductòria quan README i apunts teòrics expliquen el mateix sense connexió al producte

## Continguts que convé redistribuir
- criteris de seguretat del Bloc 5 cap a Repte 3 (base) i Repte 5 (consolidació)
- teoria comuna d’APIs (HTTP, estats, errors) concentrada a Repte 4 per evitar repetició
- parts introductòries d’arquitectura del Bloc 1 reutilitzades com a reforç en refactorització de Repte 3
- fragments de PHP bàsic reutilitzats com a suport puntual en debugging i manteniment

## Prioritats de transformació de materials
1. **Prioritat alta:** convertir Bloc 2 i Blocs 3-4 en itineraris pràctics continus (R2 i R3).
2. **Prioritat alta:** consolidar Bloc 5 com a eix transversal de qualitat i verificació (R3-R5).
3. **Prioritat mitjana:** reorganitzar Blocs 6a/6b en seqüència clara de publicació + consum (R4).
4. **Prioritat mitjana:** reorientar Bloc 7 a integració aplicada sobre producte existent (R5).
5. **Prioritat de manteniment:** simplificar teoria inicial del Bloc 1 perquè funcione com a suport de decisió, no com a tema extens.

## Definition of done del document
Este mapa es considera completat quan:
- cada bloc de materials té correspondència explícita amb reptes i RA
- s’indica ús dins del repte, adaptació necessària i paper possible de la IA
- s’identifiquen solapaments i continguts a fusionar/redistribuir
- queda clar quins materials passen de “tema” a “suport tècnic”
- el document permet planificar la transformació dels apunts sense duplicacions
