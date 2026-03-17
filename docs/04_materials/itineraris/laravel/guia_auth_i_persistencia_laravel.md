# Guia d'auth i persistència en Laravel

## Finalitat
Traduir els mínims dels Reptes 2 i 3 a un recorregut clar dins de `Laravel`, de manera que autenticació, control d'accés, persistència i modelat de dades no queden dispersos ni resolts només per convenció superficial del framework.

Esta guia ha de servir perquè l'equip construïsca una base defensable sobre `Laravel` per al projecte del curs, no només un conjunt de peces generades automàticament.

## Contingut operatiu

### Enfocament recomanat d'autenticació i control d'accés
Per al curs, l'enfocament recomanat és:
- autenticació basada en mecanismes estàndard de `Laravel` o implementació equivalent ben explicada
- control d'accés aplicat sobre rutes, controladors o middleware de manera coherent
- separació recognoscible entre autenticació, autorització i lògica de negoci
- almenys una operació del domini protegida de manera real

Criteri pràctic:
- l'equip no ha d'inventar una autenticació artesanal si `Laravel` ja oferix una via sòlida i comprensible
- tampoc ha de delegar tota la comprensió al framework: cal saber on es valida l'usuari, on es comprova l'accés i què passa quan falla
- el mecanisme triat ha de poder evolucionar cap a API i integració sense reescriptura crítica

### Persistència i modelat de dades bàsic
La base del model hauria d'incloure:
- `User` o entitat equivalent vinculada al flux d'autenticació
- una entitat principal del domini: incidència, reserva, cita, recurs o inventari
- camps obligatoris clarament justificats pel cas d'ús
- relació mínima entre usuari i entitat principal quan tinga sentit funcional
- operacions bàsiques de creació, lectura i actualització sobre el domini prioritari

Criteri docent:
- el model no ha de reproduir tot el domini final, sinó la part mínima que sosté els reptes
- convé aprofitar `Eloquent` com a capa de model, però evitant confiar cegament en convencions no enteses
- les regles del domini han de ser visibles en codi, validació o casos d'ús recognoscibles

### Validacions mínimes
S'hauria de validar, com a mínim:
- camps obligatoris del registre, login o cas d'ús principal
- tipus o format bàsic de les dades rellevants
- restriccions del domini que afecten persistència o accés
- coherència mínima abans de crear o actualitzar dades

Formes vàlides de resoldre-ho:
- `Form Request` quan ajude a desacoblar validació
- validació directa en controlador quan el cas siga molt reduït i es puga defensar
- regles complementàries al model o al cas d'ús quan la validació depenga d'estat persistent

### Criteri propi de l'itinerari Laravel
Com a mínim, la via `Laravel` hauria de deixar clar:
- migració d'usuaris o equivalent
- migració de l'entitat principal del domini
- claus o referències bàsiques quan el cas d'ús les necessite
- relacions mínimes definides al model quan realment s'usen
- ús defensable de `Eloquent`, `Form Request` o `middleware` quan aporten claredat real

Punts de control útils:
- si es crea un recurs del domini, a quin usuari o actor queda associat
- si es recupera un recurs inexistent, quina resposta funcional dona el sistema
- si falla la persistència, on es detecta i com es deixa rastre

### Evidències mínimes
S'espera trobar evidències com:
- flux de registre o autenticació funcional dins de `Laravel`
- almenys una operació del domini protegida per control d'accés
- migracions executades i model mínim recognoscible
- relacions del domini comprensibles i alineades amb el projecte base
- validacions visibles en el codi i verificades amb casos correctes i de fallada
- `README` i documentació tècnica actualitzats
- AI log si la IA ha ajudat a resoldre autenticació, migracions, relacions o validacions

## Riscos habituals
- donar per resolta l'autenticació només perquè hi ha scaffolding o middleware per defecte
- confondre autenticació amb autorització
- crear models i migracions sense relació clara amb el domini triat
- deixar tota la validació barrejada en controladors massa grossos
- confiar que `Eloquent` resol automàticament coherència, permisos o casos límit
- arribar al Repte 4 sense tindre clar quins recursos i errors passaran després a API

## Checklist final
- l'autenticació és funcional i el control d'accés està aplicat amb criteri
- el domini disposa d'un model mínim coherent amb `Laravel`
- les migracions o l'evolució d'esquema i les relacions bàsiques estan definides i provades
- hi ha validacions mínimes recognoscibles i alineades amb el comportament real
- la base resultant és prou estable per adaptar-se als Reptes 2 i 3 i preparar el salt cap a API
