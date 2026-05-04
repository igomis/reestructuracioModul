# Ajust fi de reptes i instruments

## Classificació documental

Este és un **document derivat**. Depén dels documents canònics [curs executable](curs-executable.md), [matriu de coherència curricular](matriu-coherencia-curricular-dwes.md), [avaluació i evidències](03_avaluacio/index.md) i dels `R1-R5`.

No fixa criteri nou. Sintetitza els ajustos de la Fase 4 perquè el professorat puga llegir d'una peça què s'ha ajustat i amb quina intenció docent.

## Lectura global de la seqüència `R1-R5`

La seqüència queda reforçada així:

- `R1` obri el curs i fixa l'entorn, la traçabilitat i la primera decisió tècnica.
- `R2` concentra la construcció nuclear compartida: flux de dades, lògica bàsica, estat, autenticació i primera funcionalitat protegida.
- `R3` consolida l'entrada a framework, persistència mínima real i primer flux **server-rendered** sense exigir una migració total del projecte.
- `R4` convertix una funcionalitat estabilitzada en servei reusable i verificable.
- `R5` deixa de carregar una cobertura nuclear pròpia i passa a operar com a síntesi transversal retallable abans de la defensa.

## Paper didàctic de cada repte

| Repte | Paper didàctic | Sentit docent principal |
|---|---|---|
| `R1` | iniciació / arranque | obrir bé el curs i impedir una entrada improvisada al projecte |
| `R2` | construcció nuclear | assegurar fonaments funcionals reals abans d'obrir el contrast de frameworks |
| `R3` | consolidació | professionalitzar estructura i persistència sense convertir el repte en una migració total descontrolada |
| `R4` | integració | treballar `RA7` amb contracte, consum i verificació real |
| `R5` | síntesi transversal | comprovar interoperabilitat i valor professional sense fer-lo pesar com un nou nucli curricular |

## Ajustos realitzats

- s'ha explicitat la funció didàctica principal en les fitxes canòniques dels cinc reptes
- s'ha afegit en cada repte un checkpoint de control amb sentit pedagògic real
- s'ha deixat clar en cada repte:
  - instrument dominant
  - instrument de comprensió
  - instrument de control de delegació excessiva
  - instrument de recuperació o millora
- `R3` incorpora una seqüència interna més realista i un doble checkpoint (`CP-R3A`, `CP-R3B`)
- `R5` queda definit com a síntesi transversal i amb abast retallable si el calendari es tensiona

## Canvis en evidències

S'han reforçat només evidències amb retorn docent clar:

- commit rellevant comentat
- ADR o justificació tècnica breu
- comparativa entre contracte previst i comportament observat
- comparativa solució inicial / ús assistit per IA / solució final quan té sentit
- registre breu d'errors detectats i corregits
- mini defensa tècnica en checkpoint
- `README` tècnic centrat en decisions

No s'ha afegit burocràcia general. Les evidències noves servixen per a fer més visible l'aprenentatge real i reduir dependència de la impressió subjectiva del docent.

## Canvis en instruments

La lectura resultant és:

- `R1`: domina el checklist d'arrencada
- `R2`: domina la rúbrica del repte sobre flux funcional protegit
- `R3`: domina la rúbrica de reconstrucció en framework, amb checkpoints de control
- `R4`: domina la rúbrica específica de servei web
- `R5`: domina el checklist d'integració híbrida amb defensa breu

La revisió de repositori i la defensa tècnica curta apareixen de manera sostinguda com a instruments de comprensió i de control de delegació excessiva.

## Decisions sobre checkpoints

Els checkpoints deixen de ser només hitos de seguiment. Passen a ser moments de:

- verificació tècnica mínima
- contrast de decisions
- comprovació de comprensió
- traçabilitat de l'ús assistit per IA

Especialment:

- `R2` tanca amb una mini defensa de flux complet
- `R3` es partix en `CP-R3A` i `CP-R3B`
- `R4` obliga a contrastar contracte i resposta real
- `R5` exigix cas positiu, cas d'error i defensa del mapping

## Paper final de `Repte 5`

`R5` queda situat com a **síntesi transversal**.

La decisió no és cosmètica. Vol dir:

- no se li carrega una cobertura nuclear independent del mòdul
- el seu valor principal és professional i integrador
- si el temps es complica, s'ha de retallar abast abans que contaminar `R1-R4`
- el mínim sostingut és una font externa, un cas d'ús híbrid real, un cas positiu, un cas d'error i una defensa breu

Les integracions més riques, múltiples fonts o automatitzacions periòdiques queden com a ampliació avançada.

## Impactes sobre càrrega, cobertura i avaluació

- baixa el risc que `R3` absorbisca massa complexitat sense control
- millora la visibilitat de `RA8` perquè el flux **server-rendered** queda lligat a checkpoints concrets
- es conté millor el desbordament de `RA6` en `R4` i `R5`
- la verificació de l'ús assistit per IA deixa de dependre només de la intuïció docent
- la seqüència global guanya viabilitat d'aula perquè el repte més retallable és ara també el menys nuclear curricularment
