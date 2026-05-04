# Fase 3 de matriu de coherència

## Estructura de la matriu creada

S'ha creat `docs/matriu-coherencia-curricular-dwes.md` com a **document canònic** amb:

- classificació documental i finalitat
- criteri de lectura
- matriu principal `RA -> reptes/projecte -> evidències -> instruments -> verificació -> IA -> límits`
- taula de cobertura per repte i projecte base
- lectura sintètica del paper de l'ús assistit per IA
- tancament amb cobertura global, buits detectats i decisions de Fase 4

## Correspondències principals RA ↔ reptes

- `RA1` -> `Repte 1`
- `RA2`, `RA3`, `RA4` -> `Repte 2`
- `RA5`, `RA6`, `RA8` -> `Repte 3`
- `RA7` -> `Repte 4`
- `Repte 5` -> tancament transversal amb focus principal en `RA7`, projecció aplicada de `RA8` i suport eventual de `RA6`

Cobertures de suport:

- `RA6` reapareix com a suport en `Repte 4` i eventualment en `Repte 5`
- `RA7` es reactiva en `Repte 5` quan el servei propi participa en la integració
- `RA8` només reapareix en `Repte 5` si la integració impacta en fluxos dinàmics o respostes del backend
- el projecte base i la defensa tècnica travessen tota la seqüència

## Evidències principals per repte

- `Repte 1`: comparativa tècnica, ADR, Docker, README, arrencada i primera peça funcional
- `Repte 2`: formularis, codi embegut, lògica, estat, autenticació, proves, documentació i checkpoint
- `Repte 3`: framework, migrations, seeders, model de dades, dos fluxos end-to-end, almenys un flux server-rendered, proves i README
- `Repte 4`: contracte d'API, endpoints, consum real, autenticació d'API, documentació i proves
- `Repte 5`: connector extern, mapping, transformació, integració híbrida, proves, documentació i defensa tècnica

## Instruments d'avaluació vinculats

- rúbrica base de reptes
- rúbrica de defensa tècnica
- checklist de revisió de repositori
- checklists específics per repte
- observació docent i prova guiada
- revisió de repositori
- defensa tècnica

## Punts forts detectats

- la seqüència `R1-R5` mostra una distribució curricular llegible
- cada repte ja tenia prou densitat d'evidències i instruments per construir una matriu real
- l'ús assistit per IA queda integrat com a suport regulat i no com a buit metodològic
- el projecte base ajuda a evitar una lectura fragmentada dels `RA`

## Buits detectats

- `RA8` queda molt concentrat en `R3`
- `RA6` pot menjar-se el focus de `RA7` en `R4` o el caràcter transversal de `R5` si no es controla
- la verificació real de l'ús assistit per IA continua depenent molt de l'execució docent dels checkpoints

## Ajustos mínims fets en documents existents

- s'ha creat `docs/matriu-coherencia-curricular-dwes.md`
- s'ha afegit la matriu curricular als documents canònics d'avaluació
- s'ha afegit la matriu a la navegació principal
- s'ha reforçat `Repte 3` perquè la cobertura de `RA8` quede més visible a la Fase 3

## Correcció curricular aplicada

- s'ha eliminat el resultat d'aprenentatge inexistent que s'havia atribuït a `Repte 5`; la matriu queda ajustada a `RA1-RA8`
- s'ha reubicat curricularment `Repte 5` com a tancament transversal, no com a `RA` autònom
- s'ha justificat `Repte 5` sobretot des de `RA7`, amb projecció aplicada de `RA8` i suport eventual de `RA6`

## Impacte sobre el paper de Repte 5 dins del mòdul

`Repte 5` deixa de llegir-se com una peça nuclear independent i passa a actuar com a comprovació final d'interoperabilitat, integració i criteri tècnic sobre el backend ja construït. Això el fa més rigorós curricularment i evita inventar cobertura que la programació real del mòdul no té.
