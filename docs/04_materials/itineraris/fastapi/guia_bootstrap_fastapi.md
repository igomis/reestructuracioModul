# Guia de bootstrap FastAPI

## Finalitat

Oferir una base operativa perquè l'itinerari `FastAPI` es puga arrancar amb criteri tècnic i orientació directa al projecte del curs, sense convertir l'entrada a l'ecosistema Python en un front separat dels Reptes 2-5.

Esta guia no busca resumir tot `FastAPI`. El seu objectiu és deixar una base prou clara perquè l'equip puga construir un backend mantenible, autenticable, persistent i preparat per publicar API i arribar després a integració híbrida.

En este repositori, `FastAPI` no és itinerari base general. S'ha de llegir com a via avançada o excepcional.

## Contingut operatiu

### Quan té sentit usar FastAPI dins del projecte

Convé usar `FastAPI` quan:

- l'equip ha rebut autorització per treballar una via avançada
- es vol una via de backend Python clara per a autenticació, persistència, API i proves
- el domini triat necessita una separació recognoscible entre entrada HTTP, esquemes, lògica i dades
- l'equip pot defensar l'ús de `FastAPI` com a stack real i no només com a generador ràpid d'endpoints

No té sentit usar-lo si:

- el projecte depén només de snippets o plantilles no enteses
- l'equip no sap distingir entre `router`, dependència, esquema, model i operació de negoci
- es delega tota la comprensió del stack a la IA o a l'ORM

### Estructura mínima del projecte

Per al curs, un projecte `FastAPI` usable hauria de tindre com a mínim:

- arrencada funcional de l'aplicació
- configuració clara d'entorn i dependències
- punt d'entrada recognoscible de l'aplicació
- separació mínima entre `routers`, esquemes, lògica i persistència
- model mínim del domini
- validació mínima de dades d'entrada i eixida
- proves o verificacions equivalents sobre fluxos crítics

Estructura orientativa:

- `app/main.py`
- `app/api/` o `app/routers/`
- `app/schemas/`
- `app/models/`
- `app/services/` o `app/use_cases/`
- `app/db/` o capa equivalent de persistència
- `tests/`

Si hi ha migracions, convé tindre també:

- `alembic/` o mecanisme equivalent de versionat d'esquema

### Peces clau que cal entendre

L'equip hauria d'entendre, com a mínim:

- `main.py` com a punt d'entrada i muntatge de l'aplicació
- `routers` com a capa d'exposició HTTP
- `schemas` com a contracte d'entrada i eixida
- `models` com a representació persistent del domini
- `services` o operacions equivalents com a nucli de negoci
- configuració de base de dades, dependències i entorn
- capa de proves o verificacions mínimes

Criteri docent:

- no cal desplegar totes les capacitats avançades de `FastAPI`
- sí que cal entendre el recorregut mínim entre petició, validació, negoci, persistència i resposta
- qualsevol peça generada per tutorial, CLI o IA ha de ser explicable i revisable

### Criteri propi de l'itinerari FastAPI

Convé mantindre clara la separació pròpia de l'ecosistema Python:

- `routers` com a contracte HTTP
- `schemas` com a contracte d'entrada i eixida
- `models` com a representació persistent del domini
- `services` o operacions equivalents com a nucli de negoci
- dependències i configuració d'accés a dades sense dissoldre la lògica en el `router`

Criteri comú:

- no s'ha de convertir `FastAPI` en una col·lecció d'endpoints sense arquitectura
- cal entendre què és validació, què és persistència i què és operació de negoci
- la base ha de quedar preparada per continuar cap a auth, API i integració sense reescriptura crítica

### Evidències mínimes

S'espera trobar evidències com:

- projecte `FastAPI` que arranca amb instruccions reproduïbles
- `README` actualitzat amb instal·lació, execució i comandaments mínims
- estructura recognoscible de `router`, esquema, model i persistència
- primera verificació funcional del flux inicial
- commits que mostren una arrancada real i no una pujada final opaca
- AI log si la IA ha ajudat a triar estructura, configuració o dependències

## Errors habituals d'arrancada

- posar tota la lògica dins dels `routers`
- confondre `schema` de validació amb model persistent del domini
- deixar la connexió a base de dades només aparentment preparada
- muntar `FastAPI` com una col·lecció d'endpoints sense estructura de projecte
- no distingir què és infraestructura del framework i què és lògica pròpia del domini
- acceptar codi suggerit per IA sense provar que encaixa amb el projecte del curs

## Checklist final

- el projecte `FastAPI` arranca i es pot reproduir amb instruccions clares
- l'equip entén el recorregut mínim entre `router`, esquema, negoci i persistència
- l'estructura mínima està adaptada al domini del curs
- l'ús de convencions pròpies de `FastAPI` està justificat i és defensable
- hi ha evidències reals d'arrancada i primera verificació
- la base queda preparada per connectar-se amb autenticació, persistència, API i integració en els reptes següents sense alterar el criteri d'autoria individual
