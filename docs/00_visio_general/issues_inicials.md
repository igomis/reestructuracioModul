# Estat de producció dels materials

## Situació general
El repositori ja no està en fase de bootstrap. La base curricular, el projecte base i el pla de materials prioritaris existixen i la fase real del projecte és ara de consolidació pública dels paquets produïts i de preparació del salt cap als materials per itinerari.

La necessitat actual no és obrir més fronts, sinó assegurar que allò que ja s'ha publicat com a `MG-02` a `MG-06` siga llegible, usable i coherent com a conjunt.

## Paquets consolidats
- `MG-01` queda consolidat com a marc de priorització i seqüència de producció a `docs/04_materials/pla_materials_prioritaris.md`.
- `MG-02` queda consolidat com a base comuna del mòdul amb guies de Git, README/ADR, testing/debugging i ús verificable de la IA.
- `MG-03` queda consolidat com a paquet nuclear del Repte 2 amb materials sobre flux d'usuari, sessions, validació i errors de servidor.
- `MG-04` queda consolidat com a paquet nuclear del Repte 3 amb materials sobre arquitectura per capes o equivalent, persistència i qualitat tècnica.
- `MI-01` queda consolidat com a primer patró d'itinerari reusable a `docs/04_materials/itineraris/laravel/`.
- `MI-02` queda consolidat com a segon patró d'itinerari reusable a `docs/04_materials/itineraris/express_nest/`.

## Paquets en producció
- `MG-05` ja té publicats els materials del Repte 4 a `docs/04_materials/repte_04/`, però encara ha de passar per la mateixa ronda de consolidació pública i homogeneïtzació de lectura aplicada als paquets anteriors.
- `MG-06` ja té publicats els materials del Repte 5 a `docs/04_materials/repte_05/`, però encara forma part del bloc en producció perquè ha d'alinear-se del tot amb la seqüència `R3 -> R4 -> R5`.
- `MI-03` obri el tercer itinerari tecnològic a `docs/04_materials/itineraris/fastapi/` i completa la primera trilogia de stacks autoritzats del mòdul.

## Paquets pendents
- tancar la ronda de consolidació de `MG-02` a `MG-06` abans d'obrir paquets nous
- revisar densitat, llegibilitat i coherència transversal dels materials ja publicats
- deixar preparat el repositori per obrir materials específics d'itinerari sense reescriure la base comuna

## Materials per itinerari pendents
- no queden nous itineraris per obrir; queda pendent consolidar transversalment `MI-01`, `MI-02` i `MI-03`

Criteri d'obertura:
- s'obrin de manera progressiva i un itinerari cada vegada
- `MI-01` queda com a primer patró reusable i base de comparació formal
- `MI-02` confirma la translació del model a ecosistema `Node.js`
- `MI-03` completa ara la translació del model a ecosistema Python amb `FastAPI`
- han de nàixer com a adaptació coherent dels materials existents, no com a línia paral·lela desconnectada

Nota d'itineraris:
- `MI-01` consolidat
- `MI-02` consolidat
- `MI-03` en producció: `docs/04_materials/itineraris/fastapi/`

## Revisió global pendent
- revisar que `MG-02` a `MG-06` compartixen una estructura mínima recognoscible i reutilitzable
- consolidar millor la transició pedagògica i tècnica entre `Repte 2`, `Repte 3`, `Repte 4` i `Repte 5`
- revisar la convivència entre les rutes `docs/04_materials/repte_*` i els directoris antics `docs/04_materials/materials_repte_*` abans d'obrir nous fronts
- mantindre alineats `README`, estat de producció, pla de materials i projecte base
