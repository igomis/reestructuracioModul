# Model d’itineraris tecnològics guiats

## Finalitat

Definir un model reutilitzable per introduir itineraris tecnològics en el mòdul DWES sense trencar la coherència curricular: mateixos reptes, mateixos RA, mateixes evidències i mateix marc d’avaluació.

## Principi general

L’alumnat pot treballar amb diferents stacks dins d’un marc docent comú i controlat. No es planteja llibertat total de tecnologies: hi ha un nucli comú obligatori i només s’autoritzen itineraris prèviament definits.

## Model adoptat

Model de variació guiada sobre base comuna:

- nucli comú obligatori: reptes 1-5, RA1-RA9, evidències mínimes, instruments d’avaluació, verificació d’autoria i criteris d’ús de la IA
- capes variables controlades: framework, llibreries i patrons d’implementació propis de cada stack autoritzada
- comparabilitat d’avaluació: els criteris de qualitat i defensa tècnica són equivalents, independentment de la stack

Itineraris autoritzats:

- PHP + Laravel
- Node.js + Express o Nest
- Python + FastAPI

## Moment d’introducció dels itineraris

L’itinerari tecnològic es fixa amb un nucli comú en Repte 1-2 i s’obri principalment a partir de:

- Repte 3 (migració d’arquitectura i persistència)
- Repte 4 (publicació i consum d’API)
- Repte 5 (integració híbrida i manteniment)

Això evita fragmentació prematura i manté una base docent compartida en l’arrancada del curs.

## Requisits mínims comuns per a qualsevol itinerari

- compliment dels mateixos objectius de repte i cobertura dels RA previstos
- evidències equivalents i verificables: repositori, proves, documentació tècnica i defensa
- entorn professional mínim compartit: Git/GitHub, debugging, testing, documentació i traçabilitat
- estructura de lliurables homologable entre itineraris
- capacitat de manteniment i evolució del producte en els reptes successius

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

## Proposta d’aplicació progressiva

1. Fase inicial (model comú): mantindre focus en tancar fitxes de reptes, instruments i materials base.
2. Fase pilot (R3-R5): aplicar itineraris guiats en activitats i evidències seleccionades.
3. Fase de consolidació: ajustar plantilles de repte i rúbriques amb equivalències per stack.
4. Fase d’estandardització: incorporar el model en projectes tècnics i en la programació v2.

## Relació amb projectes tècnics futurs

El model d’itineraris obri una línia per definir projectes tècnics comparables entre stacks (backend, API, integracions i automatització) mantenint evidències comunes.

Es deixa registrada una línia futura específica vinculada a mecanismes de tokenització (autenticació i/o control d’accés), pendent de disseny detallat en una fase posterior.

## Definition of done del model

Este model es considera preparat quan:

- queda documentat el nucli comú obligatori i els límits de variació per stack
- consten explícitament els tres itineraris autoritzats
- queda fixat que el desplegament principal dels itineraris es farà en Reptes 3, 4 i 5
- el paper de la IA queda definit com a assistència verificable, no substitutòria
- el model es pot reutilitzar després en fitxes de repte i projectes tècnics sense redisseny complet
