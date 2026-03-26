# Guia de refactorització a MVC o equivalent

## Finalitat

Convertir el Repte 3 en una migració controlada des d'un backend funcional però acoblat cap a una estructura mantenible, on responsabilitats, flux de dades i punts d'extensió siguen recognoscibles.

Esta guia no demana una reescriptura total ni una arquitectura ornamental. El seu objectiu és separar prou bé el codi perquè el producte puga créixer cap a API, integració i manteniment sense dependre de fitxers monolítics o lògica dispersa.

## Contingut operatiu

### Criteris mínims de separació de responsabilitats

La refactorització ha de deixar, com a mínim, estes responsabilitats diferenciades:

- entrada o capa d'exposició: rep peticions, valida format mínim i delega
- lògica de negoci o cas d'ús: aplica regles del domini i coordina el flux
- persistència o accés a dades: encapsula consultes, operacions de lectura i escriptura
- model o estructura de dades: representa entitats, validacions associades o esquemes
- tractament d'errors i respostes: manté coherència i evita comportaments dispersos

Criteris pràctics:

- un controlador o equivalent no hauria de concentrar tota la lògica de negoci
- la capa de dades no hauria d'estar barrejada amb codi de sessió, resposta o presentació
- una mateixa regla de negoci no hauria d'estar duplicada en diversos punts
- la refactorització ha de preservar funcionalitat existent del Repte 2

### Patrons o capes equivalents segons l'itinerari

L'equivalència docent no exigeix la mateixa estructura exacta, però sí una separació recognoscible:

- **Laravel**
  Patró habitual: `Controller` -> `Service` o cas d'ús -> `Model`/persistència. Quan calga, es pot afegir `Form Request`, repositori o capa de consulta.

- **Express o Nest**
  Patró habitual: ruta/controlador -> servei -> repositori o capa de dades -> model/esquema. En Nest, esta separació sol aparéixer de forma més explícita amb `controller`, `service`, `module` i `dto`.

- **FastAPI**
  Patró habitual: `router` -> servei -> repositori o accés a dades -> `schema`/model. La validació d'entrada pot descansar en esquemes, però la lògica de negoci no hauria de quedar absorbida només al `router`.

El criteri comú és este:

- una entrada rep la petició
- una capa de negoci decidix què s'ha de fer
- una capa de dades executa persistència
- el conjunt és provable i rastrejable

### Evidències esperades

S'espera trobar evidències com:

- commits que mostren migració incremental i no una substitució opaca final
- estructura de carpetes o mòduls amb responsabilitats recognoscibles
- un cas d'ús prioritzat ja migrat completament com a patró
- documentació tècnica actualitzada sobre l'estructura adoptada
- decisions d'arquitectura explicables en defensa tècnica
- AI log si la IA ha ajudat a proposar estructura, patrons o reorganització de capes

### Transició al Repte 4

El Repte 3 hauria de deixar preparat:

- quins casos d'ús passen millor a endpoints o recursos d'API
- on s'ha de concentrar el contracte d'entrada, eixida i errors per publicar-lo al Repte 4
- quines parts de l'arquitectura ja són prou estables per documentar-se com a API pública

## Errors habituals o riscos

- moure fitxers de lloc però no separar responsabilitats reals
- crear massa capes buides només per aparentar arquitectura
- refactoritzar trencant fluxos que ja funcionaven al Repte 2
- deixar consultes o accés a base de dades dins del controlador principal
- barrejar validació, negoci i resposta en un mateix bloc difícil de provar
- acceptar estructures suggerides per IA sense comprovar si realment milloren mantenibilitat

## Checklist final

- existix separació recognoscible entre entrada, negoci i persistència
- el codi del Repte 2 continua funcionant després de la migració
- almenys un cas d'ús clau ja està migrat a l'estructura nova
- les responsabilitats no estan duplicades ni barrejades de manera crítica
- l'arquitectura triada és defensable dins de l'itinerari tecnològic usat
- la base resultant queda preparada per publicar API al Repte 4
