# Guia d'auth i persistència en FastAPI

## Finalitat

Traduir els mínims dels Reptes 3 i 4 a l'itinerari `FastAPI`, de manera que autenticació, control d'accés, persistència, validació i separació entre models i esquemes queden resolts amb una estructura defensable dins de l'ecosistema Python.

Esta guia no imposa una llibreria única, però sí fixa el mínim operatiu perquè el projecte del curs siga coherent amb el domini triat, el projecte base i les evidències autèntiques del repositori.

`FastAPI` només s'hauria d'usar ací com a via avançada o excepcional.

## Contingut operatiu

### Enfocament recomanat d'autenticació i control d'accés

Per al curs, l'enfocament recomanat és:

- autenticació basada en un mecanisme estàndard i explicable dins de `FastAPI`
- separació recognoscible entre autenticació, autorització i lògica del domini
- control d'accés aplicat sobre dependències, operacions o capes equivalents de manera coherent
- almenys una operació del domini protegida de manera real

Criteri pràctic:

- no cal inventar una autenticació artesanal si l'ecosistema oferix una via sòlida i mantenible
- tampoc s'ha de delegar tota la comprensió en dependències o helpers: cal saber on es valida l'usuari, on es comprova l'accés i què passa quan falla
- el mecanisme triat ha de poder evolucionar cap a API i integració sense reescriptura crítica

### Persistència i modelat de dades bàsic

La base del model hauria d'incloure:

- `User` o entitat equivalent vinculada al flux d'autenticació
- una entitat principal del domini: incidència, reserva, cita, recurs o inventari
- camps obligatoris justificats pel cas d'ús
- relació mínima entre usuari i entitat principal quan siga funcional
- operacions bàsiques de creació, lectura i actualització sobre el domini prioritari

Criteri docent:

- el model no ha de reproduir tot el domini final, sinó la part mínima que sosté els reptes
- l'equip ha d'entendre la diferència entre model persistent, esquema de validació i operació de negoci
- les regles del domini han de ser visibles en servei, repositori o cas d'ús recognoscible

### Validacions mínimes

S'hauria de validar, com a mínim:

- camps obligatoris del registre, login o cas d'ús principal
- tipus o format bàsic de dades rellevants
- restriccions del domini que afecten persistència o accés
- coherència mínima abans de crear o actualitzar dades

Formes vàlides de resoldre-ho:

- `Pydantic` o esquemes equivalents per a entrada i eixida
- validació complementària en servei o operació quan depenga d'estat persistent
- tractament d'errors coherent quan la validació falla, quan falla la regla de domini o quan falla l'accés a dades

### Criteri propi de l'itinerari FastAPI

En `FastAPI` convé deixar clar:

- `schemas`: definixen contractes d'entrada i eixida
- `models`: representen l'estat persistent del domini
- `operations`, `services` o casos d'ús: apliquen regles i coordinen persistència
- `routers`: exposen el contracte HTTP, però no haurien d'absorbir tota la lògica

Criteri comú:

- un `schema` no substituïx un model persistent
- un model persistent no hauria de convertir-se en contracte HTTP sense revisió explícita
- una operació de negoci no hauria de quedar dissolta dins del `router`

### Evidències mínimes

S'espera trobar evidències com:

- flux funcional de registre o autenticació dins de `FastAPI`
- almenys una operació del domini protegida per control d'accés
- model mínim recognoscible i alineat amb el projecte base
- persistència funcional amb lectura, creació o actualització sobre el domini
- validacions visibles en el codi i verificades amb casos correctes i de fallada
- `README` i documentació tècnica actualitzats
- AI log si la IA ha ajudat a resoldre auth, models, esquemes, persistència o validacions

## Riscos habituals

- deixar tota la lògica de negoci dins dels `routers`
- confondre model persistent, esquema d'entrada i esquema de resposta
- assumir que l'ORM o la capa de dades resol automàticament coherència, permisos o casos límit
- dispersar validacions entre massa punts sense criteri clar
- modelar dades sense relació recognoscible amb el domini del projecte base
- arribar al Repte 4 sense saber quins recursos i errors passaran després al contracte API

## Checklist final

- l'autenticació és funcional i el control d'accés està aplicat amb criteri
- el domini disposa d'un model mínim coherent en la via `FastAPI`
- la persistència o evolució d'esquema és recognoscible i usable en els fluxos prioritaris
- hi ha validacions mínimes alineades amb el comportament real del projecte
- la relació entre models, esquemes i operacions és clara i defensable
- la base resultant és prou estable per adaptar-se als Reptes 3 i 4 i preparar el salt cap a API
