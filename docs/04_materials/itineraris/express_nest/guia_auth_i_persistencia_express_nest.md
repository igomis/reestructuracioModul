# Guia d'auth i persistència en NestJS

## Finalitat

Traduir els mínims dels Reptes 3 i 4 a l'itinerari `NestJS`, de manera que autenticació, control d'accés, persistència i validació queden resolts amb una estructura defensable.

Esta guia no pretén imposar una llibreria concreta, sinó fixar el mínim operatiu perquè el projecte del curs siga coherent amb el domini triat, el projecte base i l'entorn professional realista del repositori.

## Contingut operatiu

### Enfocament recomanat d'autenticació i control d'accés

Per al curs, l'enfocament recomanat és:

- autenticació basada en un mecanisme estàndard i explicable per a `Node.js`
- separació recognoscible entre autenticació, autorització i lògica del domini
- control d'accés aplicat sobre rutes, controladors o guards segons la via triada
- almenys una operació del domini protegida de manera real

Criteri pràctic:

- no cal inventar una autenticació artesanal si el stack permet una via més sòlida i mantenible
- tampoc s'ha de delegar tota la comprensió en middleware, guard o paquet extern: cal saber on es valida l'usuari, on es comprova l'accés i com es respon quan falla
- el mecanisme triat ha de permetre passar després a API i integració sense reescriptura crítica

### Persistència i modelat de dades bàsic

La base del model hauria d'incloure:

- `User` o entitat equivalent vinculada al flux d'autenticació
- una entitat principal del domini: incidència, reserva, cita, recurs o inventari
- camps obligatoris justificats pel cas d'ús
- relació mínima entre usuari i entitat principal quan siga funcional
- operacions bàsiques de creació, lectura i actualització sobre el domini prioritari

Criteri docent:

- el model no ha de reproduir tot el domini final, sinó la part mínima que sosté els reptes
- l'equip ha d'entendre la diferència entre esquema, model, repositori i cas d'ús
- les regles del domini han de ser visibles en codi, validació o servei recognoscible

### Validacions mínimes

S'hauria de validar, com a mínim:

- camps obligatoris del registre, login o cas d'ús principal
- tipus o format bàsic de dades rellevants
- restriccions del domini que afecten persistència o accés
- coherència mínima abans de crear o actualitzar dades

Formes vàlides de resoldre-ho:

- `DTO` i `ValidationPipe` en `Nest` quan l'equip puga defensar el flux
- validació complementària en servei o cas d'ús quan depenga d'estat persistent

### Criteri propi de l'itinerari NestJS

En `Nest` és habitual trobar:

- `controller` com a punt d'entrada
- `service` com a nucli de negoci
- `guard` per control d'accés
- `dto` i `pipe` per validació
- `module` per agrupar domini i dependències

Criteri comú:

- `Nest` exigix entendre infraestructura del framework
- la persistència i l'autenticació només són vàlides si el flux queda clar, provable i alineat amb el domini

### Evidències mínimes

S'espera trobar evidències com:

- flux funcional de registre o autenticació dins de `NestJS`
- almenys una operació del domini protegida per control d'accés
- model mínim recognoscible i alineat amb el projecte base
- persistència funcional amb lectura, creació o actualització sobre el domini
- validacions visibles en el codi i verificades amb casos correctes i de fallada
- `README` i documentació tècnica actualitzats
- AI log si la IA ha ajudat a resoldre auth, esquemes, models, persistència o validacions

## Riscos habituals

- confiar en `Nest` com si la presència de `guard` o `dto` garantira per si sola una bona arquitectura
- confondre autenticació amb autorització
- modelar dades sense relació clara amb el domini del projecte base
- dispersar les validacions entre massa punts sense criteri
- arribar al Repte 4 sense saber quins recursos i errors passaran després al contracte API

## Checklist final

- l'autenticació és funcional i el control d'accés està aplicat amb criteri
- el domini disposa d'un model mínim coherent en la via `NestJS`
- la persistència o evolució d'esquema és recognoscible i usable en els fluxos prioritaris
- hi ha validacions mínimes alineades amb el comportament real del projecte
- la base resultant és prou estable per adaptar-se als Reptes 3 i 4 i preparar el salt cap a API
