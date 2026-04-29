# Planificació d'aula del Repte 3

## Finalitat del bloc

Este document baixa `R3` a una seqüència operativa d'aula perquè el professorat puga conduir el pas des de la base comuna de `R2` cap a una arquitectura més mantenible, amb persistència real i verificable, sense convertir el repte en tres cursos paral·lels de framework.

El bloc no redefineix el repte. La seua funció és indicar què convé fer en classe, què ha de modelar el professorat, quines evidències mínimes s'han de recollir i quin criteri permet obrir `R4`.

`R3` treballa sobre el mateix projecte funcional del curs. La diferència és que el cas d'ús prioritari passa a estar millor separat entre presentació, lògica i persistència, i comença el contrast tecnològic amb `Laravel`, `Symfony` o `NestJS` com a itineraris de stack.

## Posició de `R3` dins de la seqüència del curs

`R2` queda tancat com a base comuna en `PHP`: formulari, validació, processament, estat, autenticació i una funcionalitat protegida ja han d'existir com a referència funcional.

`R3` no torna a construir eixe flux des de zero. Agafa una funcionalitat real de `R2`, diagnostica els seus problemes de mantenibilitat i la migra o reconstrueix dins d'una arquitectura més clara.

El canvi important del bloc és este:

- de codi funcional però encara acoblat
- a cas d'ús estructurat, persistent, verificat i explicable

Este pas és imprescindible abans de `R4`, perquè una `API` publicada sobre una base efímera, desordenada o no defensable només amplifica els problemes del projecte.

## Relació amb `RA5` i preparació de `RA6`

`R3` continua tenint com a eix principal `RA5`: aplicar mecanismes per separar presentació, lògica de negoci i organització interna de l'aplicació.

La persistència entra com a suport fort i verificable de `RA6`, però encara amb abast controlat: no es tracta de modelar tota la base de dades del producte, sinó de deixar persistent el recurs o cas d'ús que dona sentit al bloc.

Lectura docent:

- `RA5` marca la qualitat de la separació de responsabilitats.
- `RA6` comença a aparèixer amb accés a dades real, ús segur i comprovació de lectura i escriptura.
- `R4` només s'ha d'obrir si la persistència de `R3` és suficient per exposar després serveis o `API` amb coherència.

## Duració recomanada en sessions de 3 hores

Duració base:

- `12 hores`
- `4` sessions de `3` hores
- una única planificació comuna
- variants de stack segons `Laravel`, `Symfony` o `NestJS`

Distribució recomanada:

| Sessió | Duració | Focus principal | Evidència clau |
|---|---:|---|---|
| `1` | `3h` | diagnosi del codi actual i pla de migració | cas d'ús triat, mapa de responsabilitats i pla curt |
| `2` | `3h` | primera refactorització estructural i separació de responsabilitats | flux reorganitzat amb capes o rols visibles |
| `3` | `3h` | persistència real i verificable sobre el cas d'ús prioritari | lectura i escriptura persistents dins del flux |
| `4` | `3h` | regressió, documentació, defensa breu i tancament de `R3` | proves mínimes, README tècnic i criteri d'entrada a `R4` |

## Seqüència detallada de 4 sessions

### Sessió 1. Diagnosi del codi actual i pla de migració

**Objectiu**

Seleccionar el cas d'ús de `R2` que passarà a `R3`, detectar acoblaments reals i deixar un pla curt de migració viable dins del stack triat.

**Què explica el professorat**

- per què `R3` no és repetir `R2` en un framework
- quina diferència hi ha entre moure fitxers i separar responsabilitats
- com usar `Laravel`, `Symfony` o `NestJS` com a via tècnica sense fragmentar l'objectiu docent
- què significa una persistència suficient per al cas d'ús prioritari

**Què modela el professorat**

- una lectura ràpida d'un flux existent amb mescla de presentació, lògica i accés a dades
- una taula curta de responsabilitats actuals i responsabilitats desitjades
- un pla de migració de 3 o 4 passos, amb risc i evidència esperada

**Què fa l'alumnat**

- tria un cas d'ús real del seu projecte
- identifica què ve de `R2` i què es vol professionalitzar
- marca punts d'acoblament, duplicació o dependència excessiva
- decideix el stack base: `Laravel`, `Symfony` o `NestJS`
- obri issue principal o registre equivalent amb microtasques

**Variants de stack**

- en `Laravel`, localitzar ruta, controlador, servei o acció, vista i model o migració prevista
- en `Symfony`, localitzar ruta, controlador, servei, plantilla o resposta i entitat o repositori previst
- en `NestJS`, localitzar controlador, servei, mòdul, DTO i persistència prevista

**Evidència mínima de sessió**

- cas d'ús triat
- diagnosi breu del punt de partida
- mapa de responsabilitats actuals i futures
- pla curt de migració
- issue principal de `R3` amb tasques inicials

**Checkpoint docent**

El professorat valida que el cas d'ús és real, que ve de `R2` i que el pla no és una reescriptura total ni una reorganització ornamental.

### Sessió 2. Primera refactorització estructural i separació de responsabilitats

**Objectiu**

Fer la primera migració o reconstrucció controlada del cas d'ús, separant qui rep la petició, qui coordina el flux, on queda la lògica i com es prepara la resposta.

**Què explica el professorat**

- com reconèixer les peces equivalents a controlador, servei, vista, cas d'ús, DTO, entitat o repositori segons el stack
- per què la nomenclatura del framework no és suficient si les responsabilitats continuen barrejades
- com fer commits de migració incremental que permeten revisar el canvi

**Què modela el professorat**

- una refactorització curta d'un fragment funcional
- extracció d'una responsabilitat fora del controlador o de la vista
- comprovació immediata que el comportament principal no s'ha trencat

**Què fa l'alumnat**

- crea o ajusta l'estructura base del framework triat
- migra una primera part del cas d'ús
- separa entrada, coordinació, lògica i resposta amb noms comprensibles
- manté un comportament executable encara que el flux no estiga complet
- registra en commits les decisions estructurals principals

**Variants de stack**

- `Laravel`: ruta i controlador prim, validació o request quan pertoque, servei o acció per a lògica i vista o resposta clara
- `Symfony`: controlador prim, servei de domini o aplicació, formulari/DTO si aplica i plantilla o resposta separada
- `NestJS`: mòdul del cas d'ús, controlador, servei, DTO i resposta controlada sense lògica de negoci dins del controlador

**Evidència mínima de sessió**

- estructura del stack recognoscible
- primera part del cas d'ús migrada o reconstruïda
- separació visible de responsabilitats
- demo curta del flux parcial o complet
- commit o sèrie de commits de refactorització

**Checkpoint docent**

El professorat demana a l'alumnat que explique què ha deixat de viure en el fitxer o peça original i on s'ha mogut cada responsabilitat. Si la resposta només és “ara està en el framework”, el checkpoint no està superat.

### Sessió 3. Persistència real i verificable sobre el cas d'ús prioritari

**Objectiu**

Connectar el cas d'ús refactoritzat amb una persistència real, suficient i comprovable, incloent lectura i almenys una operació d'escriptura, actualització o equivalent.

**Què explica el professorat**

- què és persistència verificable i què és només simulació
- com encaixa la capa de dades en cada stack sense contaminar la presentació
- quins errors mínims de dades s'han de controlar
- per què `R3` no exigeix model complet del producte, però sí base persistent real del cas d'ús prioritari

**Què modela el professorat**

- una entitat, model o esquema mínim del recurs central
- una lectura real de dades dins del flux
- una escriptura o actualització verificable
- una comprovació directa de l'estat de les dades abans i després

**Què fa l'alumnat**

- defineix el recurs persistent central del cas d'ús
- configura migració, entitat, model, esquema o repositori segons el stack
- integra lectura de dades en el flux refactoritzat
- implementa una operació de creació, actualització o equivalent
- prova un cas positiu i un error controlat relacionat amb dades

**Variants de stack**

- `Laravel`: migració, model `Eloquent`, relació mínima si és necessària i ús des d'un servei o controlador prim
- `Symfony`: entitat, repositori, migració o schema update controlat i ús des d'un servei
- `NestJS`: DTO, servei, entitat/esquema segons ORM o ODM triat i accés encapsulat en servei o repositori

**Evidència mínima de sessió**

- recurs persistent definit
- lectura real de dades
- escriptura, actualització o operació equivalent verificable
- captura, checklist o registre de prova abans/després
- explicació breu de per què la persistència és suficient per a `R3`

**Checkpoint docent**

El professorat executa o demana executar una lectura i una modificació de dades. El resultat ha de poder comprovar-se fora de la pantalla final de la demo, amb base de dades, consola, eina d'administració, logs o prova reproduïble.

### Sessió 4. Regressió, documentació, defensa breu i tancament de `R3`

**Objectiu**

Demostrar que el cas d'ús continua funcionant després de la migració, documentar l'estat real i decidir si la base està preparada per entrar a `R4`.

**Què explica el professorat**

- com fer una regressió mínima sobre el flux migrat
- quina documentació és útil per a continuar amb `R4`
- com preparar una defensa tècnica curta basada en evidències
- quins deutes tècnics poden quedar oberts i quins bloquegen el pas

**Què modela el professorat**

- una checklist curta de prova: cas positiu, cas negatiu, persistència i error controlat
- una lectura de `README` tècnic coherent amb el codi real
- una defensa de 3 minuts amb decisió, canvi, prova i límit pendent

**Què fa l'alumnat**

- executa regressió mínima del cas d'ús
- registra incidències i correccions
- actualitza `README`, decisions tècniques o `ADR`
- completa `AI log` si ha usat IA
- prepara i fa una defensa breu del canvi
- proposa quin recurs o flux serà base d'`API` en `R4`

**Evidència mínima de sessió**

- checklist de prova amb cas positiu i negatiu
- demo del flux persistent
- documentació tècnica actualitzada
- registre de decisions i deute tècnic
- defensa breu individual o per equip amb preguntes de contrast

**Checkpoint docent**

El professorat contrasta repositori, commits, documentació, proves i defensa. Si algun d'estos elements no correspon amb els altres, `R3` no queda tancat.

## Què modela el professorat

El professorat ha de modelar peces curtes i transferibles, no una implementació completa del repte:

- lectura d'un flux existent i detecció d'acoblaments
- pla de migració incremental
- refactorització curta amb prova immediata
- separació entre controlador, servei, presentació i dades o equivalents
- creació d'un recurs persistent mínim
- comprovació de lectura i escriptura
- regressió mínima amb cas positiu i negatiu
- defensa tècnica breu basada en evidències

La consigna és mostrar el mètode de treball, no donar una plantilla que l'alumnat puga copiar sense entendre-la.

## Què pot deixar-se parcialment a la IA

La IA pot ajudar en tasques de suport:

- detectar possibles acoblaments a partir d'un fragment de codi
- proposar un pla de refactorització per passos
- generar esquelets inicials de controlador, servei, DTO, model o entitat
- suggerir casos de prova
- revisar missatges d'error o documentació tècnica
- comparar avantatges i límits de l'stack triat per al cas concret

Controls obligatoris:

- l'alumnat ha de poder explicar cada peça acceptada
- cap codi generat substitueix la prova real
- les decisions importants han de quedar al repositori o en un registre tècnic
- si hi ha ús d'IA, cal `AI log` o registre equivalent
- el professorat pot demanar un microcanvi en viu sobre una peça generada

No s'ha de deixar a la IA:

- triar el cas d'ús sense criteri del producte
- decidir l'arquitectura final sense contrast amb el codi real
- fabricar proves no executades
- redactar una defensa que l'alumnat no puga sostindre oralment

## Evidències mínimes per sessió

| Sessió | Evidències mínimes |
|---|---|
| `1` | cas d'ús triat, diagnosi, mapa de responsabilitats, pla curt de migració i issue principal |
| `2` | estructura del stack, primera migració, separació de responsabilitats, demo parcial o completa i commits |
| `3` | recurs persistent, lectura real, escriptura o actualització verificable, prova abans/després i justificació de suficiència |
| `4` | regressió mínima, cas positiu i negatiu, documentació actualitzada, deute tècnic i defensa breu |

## Checkpoints docents

- Final de sessió `1`: el cas d'ús ve de `R2`, és funcional i té un pla de migració viable.
- Final de sessió `2`: la separació de responsabilitats és visible i no només nominal.
- Final de sessió `3`: la persistència és real, verificable i integrada en el flux.
- Final de sessió `4`: el cas d'ús és explicable, provat i preparat per servir de base a `R4`.

Preguntes útils de contrast:

- quin comportament de `R2` continua viu?
- quina responsabilitat s'ha mogut i per què?
- on es valida l'entrada i on es tracta l'error?
- on es llig o escriu la dada persistent?
- què passaria si demà calguera exposar este recurs com a `API`?

## Adaptació per alumnat endarrerit

L'objectiu és reduir abast, no rebaixar verificació.

Mesures recomanades:

- limitar `R3` a un únic cas d'ús i un únic recurs persistent
- prioritzar una ruta o acció completa abans que diverses peces parcials
- usar el stack triat amb l'estructura mínima recognoscible
- ajornar relacions complexes, permisos avançats o segones entitats
- exigir igualment lectura i escriptura verificables
- preparar una defensa curta centrada en què funciona, què s'ha separat i què queda pendent

Mínim no negociable:

- cas d'ús real de `R2`
- separació bàsica de responsabilitats
- persistència real
- prova reproduïble
- documentació curta però coherent

## Ampliació per alumnat avançat

L'ampliació ha de aprofundir el mateix bloc, no obrir un producte paral·lel.

Possibles ampliacions:

- migrar un segon cas d'ús relacionat
- afegir una relació de dades simple i útil
- incorporar proves més sistemàtiques
- millorar tractament d'errors i validacions
- introduir patró de repositori, cas d'ús o servei d'aplicació si encaixa amb el stack
- preparar un contracte preliminar d'`API` per a `R4`
- documentar trade-offs entre dos enfocaments del mateix stack

Condició:

- l'ampliació no pot substituir la defensa del cas d'ús principal ni relaxar la verificació de persistència.

## Riscos metodològics i mesures de control

| Risc | Mesura de control |
|---|---|
| convertir `R3` en tres planificacions diferents per framework | mantindre sessions, evidències i checkpoints comuns; tractar els frameworks com a variants de stack |
| repetir `R2` dins d'un framework | exigir diagnosi, comparativa abans/després i justificació de la millora estructural |
| crear capes buides o noms correctes sense responsabilitats reals | preguntes de contrast sobre què fa i què no fa cada peça |
| persistència decorativa o simulada | prova directa de lectura i escriptura amb comprovació abans/després |
| delegació excessiva en IA | `AI log`, microcanvi en viu i defensa oral sobre codi real |
| reescriptura massa gran i pèrdua de control | pla curt de migració, commits incrementals i regressió al final de cada canvi significatiu |
| documentació embellida però falsa | contrast entre `README`, commits, execució i preguntes de defensa |
| pas prematur a `R4` | checkpoint formal d'entrada amb persistència, regressió i explicació tècnica |

## Criteri d’entrada a `R4`

No s'obri `R4` només perquè el calendari avance.

`R4` pot començar quan el professorat pot verificar que:

- el cas d'ús prioritari ve de `R2` i continua funcionant
- la nova estructura separa responsabilitats de manera explicable
- hi ha persistència real del recurs central
- es pot demostrar lectura i escriptura o actualització de dades
- existeix regressió mínima amb cas positiu i cas negatiu
- el `README` o documentació tècnica permet reproduir el flux
- l'alumnat pot defensar què ha canviat, per què i què queda pendent
- el recurs persistent pot convertir-se en base raonable per a una `API`

Si falta persistència verificable, si el codi no és explicable o si la demo depén d'estat temporal no reproduïble, `R3` continua obert i `R4` no hauria de començar.
