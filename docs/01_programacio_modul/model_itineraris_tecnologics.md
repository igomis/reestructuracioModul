# Model d’itineraris tecnològics guiats

## Finalitat

Definir un model reutilitzable per introduir itineraris tecnològics en el mòdul DWES sense trencar la coherència curricular: mateixos reptes, mateixos RA, mateixes evidències i mateix marc d’avaluació.

## Principi general

L’alumnat pot treballar amb diferents frameworks dins d’un marc docent comú i controlat. No es planteja llibertat total de tecnologies: hi ha un nucli comú obligatori i només s’autoritzen itineraris prèviament definits.

## Model adoptat

Model de variació guiada sobre base comuna:

- nucli comú obligatori: reptes `1-5`, `RA1-RA9`, evidències mínimes, instruments d’avaluació, verificació d’autoria i criteris d’ús de la IA
- `R2` com a base comuna en `PHP` per a tot l’alumnat
- capes variables controlades a partir de `R3`: framework, llibreries i patrons d’implementació propis de cada stack autoritzada
- comparabilitat d’avaluació: els criteris de qualitat i defensa tècnica són equivalents, independentment del framework

Itineraris autoritzats:

- `Laravel`
- `Symfony`
- `NestJS`

Via no base general:

- `FastAPI`, només com a opció avançada o excepcional quan hi haja prou autonomia i viabilitat docent

## Moment d’introducció dels itineraris

L’itinerari tecnològic es fixa amb un nucli comú i s’obri principalment a partir de:

- `Repte 3` (migració d’arquitectura i persistència)
- `Repte 4` (publicació i consum d’API)
- `Repte 5` (integració híbrida i manteniment)

Això implica:

- `R1` obri el projecte i deixa la primera peça funcional
- `R2` consolida una base comuna en `PHP`
- el contrast de frameworks no entra com a norma general en `R2`
- el mateix projecte continua després amb itineraris diferents

Això evita fragmentació prematura i manté una base docent compartida en l’arrancada del curs.

## Requisits mínims comuns per a qualsevol itinerari

- compliment dels mateixos objectius de repte i cobertura dels RA previstos
- evidències equivalents i verificables: repositori, proves, documentació tècnica i defensa
- entorn professional mínim compartit: Git/GitHub, debugging, testing, documentació i traçabilitat
- estructura de lliurables homologable entre itineraris
- capacitat de manteniment i evolució del producte en els reptes successius

En tots els casos:

- el repositori és individual
- les evidències són individuals
- la defensa és individual
- el contrast tècnic compartit només complementa l’acreditació

## Organització preferent del contrast

La modalitat preferent és:

- mateix projecte
- mateix encàrrec funcional
- repositoris individuals
- evidències individuals
- defensa individual
- contrast tècnic compartit

El model base és el de parelles de contrast tècnic.

També es poden permetre trios avançats:

- només quan hi haja prou autonomia
- només si hi ha tres stacks diferents realment sostenibles
- només si la verificació individual continua sent clara

## Paper de la IA

La IA s’utilitza com a suport per explorar una stack nova, accelerar prototips i detectar errors, especialment quan l’alumnat entra en un itinerari menys conegut.

Límit docent obligatori:

- la IA no substituïx la validació tècnica
- la IA no substituïx la defensa tècnica
- qualsevol aportació assistida s’ha de poder explicar, provar i modificar

## Criteris de viabilitat docent

- disponibilitat real de materials mínims per l’itinerari autoritzat
- càrrega de seguiment assumible pel professorat en correcció i defensa
- equivalència de dificultat i d’evidències entre itineraris
- possibilitat de feedback tècnic accionable sense duplicar tota la programació
- riscos acotats de dependència excessiva de la IA en stacks noves

En el cas de `FastAPI`, a més:

- no s’ha de presentar com a itinerari base general
- només s’ha d’obrir quan hi haja justificació docent clara
- s’ha de llegir com a via avançada o excepcional

## Proposta d’aplicació progressiva

1. Fase inicial: mantindre `R2` com a base comuna en `PHP`.
2. Fase pilot de contrast: aplicar itineraris guiats des de `R3`.
3. Fase de consolidació: ajustar plantilles de repte i rúbriques amb equivalències per framework.
4. Fase d’estandardització: incorporar el model en projectes tècnics i en la programació `v2`.

## Relació amb projectes tècnics futurs

El model d’itineraris obri una línia per definir projectes tècnics comparables entre stacks (backend, API, integracions i automatització) mantenint evidències comunes.

Es deixa registrada una línia futura específica vinculada a mecanismes de tokenització (autenticació i/o control d’accés), pendent de disseny detallat en una fase posterior.

## Definition of done del model

Este model es considera preparat quan:

- queda documentat el nucli comú obligatori i els límits de variació per stack
- queda fixat explícitament que `R2` és base comuna en `PHP`
- consten explícitament `Laravel`, `Symfony` i `NestJS` com a frameworks base
- `FastAPI` queda identificat com a via avançada o excepcional
- queda fixat que el desplegament principal dels itineraris es farà en Reptes `3`, `4` i `5`
- el paper de la IA queda definit com a assistència verificable, no substitutòria
- el model es pot reutilitzar després en fitxes de repte i projectes tècnics sense redisseny complet
