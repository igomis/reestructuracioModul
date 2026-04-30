# Planificació d'aula del Repte 3

## Finalitat del bloc

Este document baixa `R3` a una seqüència operativa d'aula perquè el professorat puga conduir la reconstrucció del projecte en framework amb base operativa real, persistència mínima real i primers fluxos funcionals verificables.

No redefineix el repte. La referència conceptual i avaluable continua sent [repte_03_mvc_i_persistencia.md](../02_reptes/repte_03_mvc_i_persistencia.md). Esta planificació concreta com portar-lo a classe: què convé modelar, què ha de produir l'alumnat, quines evidències mínimes cal exigir i quan es pot considerar que la base està preparada per entrar a `R4`.

`R3` no demana migrar tota l'aplicació heretada de `R2`. Demana construir una nova base real en framework i portar-hi almenys `2` casos d'ús end-to-end, amb almenys `1` flux heretat de `R2`. El segon pot ser també migrat o una ampliació funcional xicoteta si fa visible el valor del framework.

## Posició de `R3` dins del curs

`R3` s'obri al final de l'avaluació 1 i es tanca a l'inici de l'avaluació 2.

En la seqüència de `20` setmanes del repositori, això correspon a:

- `Setmana 9`: arrencada del projecte en framework, Docker i rutes mínimes.
- `Setmana 10`: model de dades, BBDD real, `migrations` i `seeders`.
- `Setmana 11`: primer cas d'ús complet migrat de `R2`.
- `Setmana 12`: segon cas d'ús o ampliació funcional, estabilització i tancament tècnic.

`R2` queda tancat com a base comuna en `PHP`: formulari, validació, processament, estat, autenticació i una funcionalitat protegida han d'existir com a referència funcional. `R3` no torna a fer eixe flux de la mateixa manera ni el migra tot: reconstrueix una base real en `Laravel`, `Symfony` o `NestJS` i selecciona fluxos troncals verificables.

Els itineraris tecnològics funcionen com a suport de stack:

- mateixa seqüència docent
- mateixes evidències mínimes
- mateixos checkpoints
- diferent nomenclatura tècnica segons el framework

## Relació amb `RA5` i preparació de `RA6`

El nucli de `R3` és `RA5`: usar el framework per separar entrada HTTP, coordinació, lògica, presentació o resposta i responsabilitats internes.

`RA6` s'activa com a suport fort i parcial: la persistència ha de ser real, segura i suficient per als fluxos prioritzats, però no cal convertir el repte en el model complet de dades de tot el producte.

Lectura docent:

- `RA5` marca si l'arquitectura del framework és clara, mantenible i explicable.
- `RA6` marca si l'accés a dades és real, coherent, verificable i integrat en fluxos funcionals.
- `R4` només té sentit si `R3` deixa una base persistent que es pot exposar després com a `API` sense improvisació.

## Duració recomanada

El document del repte situa `R3` en una duració orientativa de `6` a `8` sessions.

Opció docent preferent:

- `8` sessions de `3` hores
- `24` hores aproximades
- `4` setmanes de treball en el model de `6` hores setmanals
- inici al final de l'avaluació 1
- tancament a l'inici de l'avaluació 2

Compactació possible:

- `6` sessions si el grup arriba amb `R2` molt sòlid i l'stack no introdueix fricció significativa.
- no convé compactar per davall de `6` sessions perquè desapareix la verificació real de Docker, BBDD, `migrations`, `seeders`, dos fluxos i proves.

Si cal reduir abast, es redueix la mida dels fluxos, no els mínims: Docker, projecte arrancable, BBDD real, `migrations`, `seeders`, `2` casos d'ús, validació, errors, proves i README.

## Correspondència entre microprojectes i sessions

| Microprojecte | Sessions | Producte parcial esperat | Evidència mínima | Checkpoint docent |
|---|---|---|---|---|
| `MP1` Arrencada del nou projecte | `1` | stack triat, Docker, projecte base, `.env` i rutes mínimes | projecte arrancable, ruta inicial, issue de `R3` i declaració dels `2` fluxos | no és només esquelet: arranca i té abast funcional definit |
| `MP2` Model de dades i persistència mínima | `2-3` | BBDD real amb esquema inicial i dades de prova | `migrations`, `seeders`, connexió i lectura real | la BBDD es pot reconstruir sense càrrega manual |
| `MP3` Primer cas d'ús complet | `3-4` | primer flux end-to-end migrat de `R2` | ruta, controlador, model/servei, vista/resposta, BBDD i validació mínima | el flux ve de `R2` i funciona amb dades reals |
| `MP4` Segon cas d'ús o ampliació funcional | `5-6` | segon flux end-to-end o ampliació útil | recorregut funcional, BBDD, validació/error i demo | no és canvi cosmètic ni duplicació buida |
| `MP5` Qualitat i estabilització | `6-7` | validació, errors, proves i neteja d'estructura | proves mínimes, cas positiu/negatiu, revisió de responsabilitats | els dos fluxos continuen funcionant després de la neteja |
| `MP6` Tancament tècnic | `8` | README, decisions, demo i backlog de migració | instruccions d'arrencada, fluxos documentats i mapa del que queda | només s'obri `R4` si la base és reproduïble i defensable |

El solapament entre microprojectes és intencionat. `MP2` pot començar mentre encara es tanca `MP1`, i `MP5` pot actuar sobre `MP3` i `MP4` a mesura que apareixen errors. El criteri és mantindre un producte executable en tot moment.

## Seqüència detallada de 8 sessions de 3 hores

### Sessió 1. Arrencada del nou projecte

**Microprojecte principal**

- `MP1 — Arrencada del nou projecte`

**Objectiu**

Triar l'stack, preparar Docker, crear el projecte base del framework i verificar una primera ruta mínima.

**Què explica el professorat**

- per què `R3` no és migrar tota l'aplicació de `R2`
- què vol dir base real en framework
- quins mínims tècnics no es poden ajornar: Docker, `.env`, rutes i arrencada
- com declarar un abast de `2` casos d'ús sense obrir una reescriptura total

**Què modela el professorat**

- arrencada d'un projecte base en el framework triat
- configuració mínima de Docker i `.env`
- ruta o `healthcheck`
- issue principal de `R3` amb microtasques

**Tasques**

- triar `Laravel`, `Symfony`, `NestJS` o via excepcional autoritzada
- crear o estabilitzar el projecte base
- preparar Docker i configuració mínima
- crear una ruta inicial
- declarar els `2` casos d'ús de `R3`
- indicar quin cas d'ús ve de `R2`

**Evidència mínima**

- projecte arrancable amb Docker
- `.env.example` o instruccions equivalents
- ruta inicial funcional
- issue principal amb els `2` fluxos

**Checkpoint docent**

L'aplicació ha d'arrancar. Si només hi ha instal·lació parcial o carpetes del framework sense execució, no es passa a la sessió següent.

### Sessió 2. Model de dades inicial

**Microprojecte principal**

- `MP2 — Model de dades i persistència mínima`

**Objectiu**

Definir l'esquema mínim de dades i crear la primera migració vinculada als fluxos de `R3`.

**Què explica el professorat**

- diferència entre persistència real i dades de demo incrustades
- relació entre cas d'ús, entitat, migració i model o equivalent
- què és una dada mínima suficient per provar un flux

**Què modela el professorat**

- una migració simple
- un model, entitat o esquema
- configuració de connexió a BBDD
- comprovació de taula creada

**Tasques**

- definir les entitats o taules mínimes
- crear `migrations`
- configurar connexió de BBDD
- executar migracions
- registrar decisions de model de dades

**Evidència mínima**

- BBDD creada per `migrations`
- esquema inicial coherent amb els fluxos
- comprovació de connexió i estructura

**Checkpoint docent**

La BBDD ha de poder crear-se de zero. Si l'esquema només existeix manualment en una eina gràfica o local, no és suficient.

### Sessió 3. Seeders i primera lectura real

**Microprojecte principal**

- `MP2 — Model de dades i persistència mínima`

**Microprojecte secundari**

- inici de `MP3 — Primer cas d'ús complet`

**Objectiu**

Carregar dades inicials reproduïbles i preparar la primera lectura real des del framework.

**Què explica el professorat**

- per què els seeders eviten demos irreproduïbles
- com comprovar dades sense dependre de l'estat local d'una màquina
- com una lectura simple prepara el primer flux

**Què modela el professorat**

- seeder, fixture o script equivalent
- reset de BBDD i recàrrega de dades
- lectura bàsica des d'un controlador, servei o consola del framework

**Tasques**

- crear seeders o equivalent
- carregar dades de demostració
- verificar lectura real
- documentar com reiniciar BBDD i dades

**Evidència mínima**

- dades inicials reproduïbles
- lectura real des de l'aplicació o eina del framework
- instruccions de reset de BBDD

**Checkpoint docent**

Les dades han de poder aparéixer després d'un reset. Si cal inserir-les a mà, el repte encara no té persistència reproduïble.

### Sessió 4. Primer cas d'ús complet migrat de `R2`

**Microprojecte principal**

- `MP3 — Primer cas d'ús complet`

**Objectiu**

Portar al framework un cas d'ús real heretat de `R2` amb recorregut complet.

**Què explica el professorat**

- recorregut d'una petició pel framework
- rols de ruta, controlador, model o servei i vista o resposta
- criteri de validació mínima i error controlat

**Què modela el professorat**

- una ruta connectada amb un controlador
- lectura de BBDD dins del flux
- resposta amb plantilla, vista o JSON segons l'stack
- validació o error mínim

**Tasques**

- implementar ruta del primer cas d'ús
- crear o ajustar controlador i servei o equivalent
- llegir dades reals
- retornar vista, plantilla o resposta
- afegir validació mínima si escau
- registrar prova del cas positiu

**Evidència mínima**

- primer flux end-to-end funcionant
- traça que el flux ve de `R2`
- BBDD implicada en el flux
- validació o error mínim

**Checkpoint docent**

El cas d'ús ha de ser funcional de punta a punta. Una pantalla que només mostra dades estàtiques no tanca `MP3`.

### Sessió 5. Segon flux o ampliació funcional

**Microprojecte principal**

- `MP4 — Segon cas d'ús o ampliació funcional`

**Objectiu**

Construir un segon recorregut end-to-end que demostre que la base del framework pot créixer.

**Què explica el professorat**

- diferència entre ampliació funcional i canvi cosmètic
- com reutilitzar estructura sense duplicar codi sense criteri
- com escollir un segon flux viable

**Què modela el professorat**

- una operació xicoteta però real: alta, edició, canvi d'estat, detall o filtratge
- validació i error associats
- ús d'una relació simple si el domini ho demana

**Tasques**

- decidir si el segon flux és migrat o ampliació
- implementar ruta i controlador o equivalents
- connectar-lo amb BBDD
- afegir validació o error mínim
- verificar demo end-to-end

**Evidència mínima**

- segon flux executable
- justificació del seu valor
- prova o verificació mínima

**Checkpoint docent**

No compta com a segon flux una pàgina estàtica, una còpia del primer canviant noms o una millora només visual.

### Sessió 6. Validació, errors i primera bateria de proves

**Microprojecte principal**

- `MP5 — Qualitat i estabilització`

**Objectiu**

Fer que els dos fluxos tinguen validació, errors bàsics i proves mínimes o verificacions reproduïbles.

**Què explica el professorat**

- quins errors mínims cal controlar en un flux amb BBDD
- diferència entre provar manualment una vegada i deixar verificació reproduïble
- com registrar cas positiu i cas negatiu

**Què modela el professorat**

- prova funcional o verificació guiada
- provocació d'un error
- revisió de resposta del sistema

**Tasques**

- afegir o completar validacions
- tractar errors bàsics
- preparar proves mínimes o checklist executable
- verificar cas positiu i cas negatiu dels fluxos

**Evidència mínima**

- proves o verificacions registrades
- errors controlats visibles
- dos fluxos encara funcionant

**Checkpoint docent**

No es considera qualitat mínima si només hi ha una demo feliç sense cap entrada incorrecta o situació d'error.

### Sessió 7. Estabilització d'estructura

**Microprojecte principal**

- `MP5 — Qualitat i estabilització`

**Microprojecte secundari**

- inici de `MP6 — Tancament tècnic`

**Objectiu**

Revisar responsabilitats, netejar duplicacions i assegurar que migracions, seeders i fluxos continuen funcionant.

**Què explica el professorat**

- com detectar controladors massa carregats
- què vol dir responsabilitat clara segons cada framework
- per què una neteja no ha de trencar la reproducció de dades

**Què modela el professorat**

- refactorització mínima d'un controlador o servei
- reexecució de migracions i seeders
- prova ràpida dels dos fluxos després de la neteja

**Tasques**

- revisar rutes, controladors, serveis i models o equivalents
- eliminar duplicacions evidents
- comprovar migracions i seeders
- repetir proves dels dos fluxos
- començar README tècnic

**Evidència mínima**

- estructura revisada
- migracions i seeders encara funcionant
- proves repetides després de la neteja

**Checkpoint docent**

La neteja només és vàlida si el sistema continua arrancant i els dos fluxos continuen vius.

### Sessió 8. Tancament tècnic i pas a `R4`

**Microprojecte principal**

- `MP6 — Tancament tècnic`

**Objectiu**

Tancar `R3` amb documentació executable, demostració curta, decisions tècniques i mapa del que queda per migrar.

**Què explica el professorat**

- com escriure un README que una altra persona puga seguir
- com distingir el que s'ha migrat del que queda pendent
- com decidir quins recursos poden passar a `R4`

**Què modela el professorat**

- estructura curta de README
- backlog de migració
- demo de tancament amb arrencada, BBDD, seeders i dos fluxos

**Tasques**

- actualitzar README
- documentar arrencada, `.env`, migracions i seeders
- descriure els `2` casos d'ús
- registrar decisions tècniques
- deixar backlog o mapa del que queda per migrar de `R2`
- identificar possible nucli d'`API` per a `R4`

**Evidència mínima**

- README tècnic actualitzat
- demo final
- backlog de migració
- base candidata per a `R4`

**Checkpoint docent**

Només s'obri `R4` si el projecte arranca, la BBDD es reconstrueix, les dades es carreguen i els dos fluxos funcionen amb proves mínimes.

## Checkpoints de control del repte

| Moment | Pregunta docent | Evidència exigible |
|---|---|---|
| Després de `MP1` | El projecte en framework arranca de veritat? | Docker, `.env`, ruta mínima i issue amb `2` fluxos |
| Després de `MP2` | La persistència es pot reconstruir de zero? | `migrations`, `seeders`, BBDD i lectura real |
| Després de `MP3` | Hi ha un flux de `R2` migrat i funcional? | ruta, controlador, dades reals, vista/resposta i validació |
| Després de `MP4` | Hi ha un segon flux real? | segon recorregut end-to-end, no cosmètic |
| Després de `MP5` | El projecte aguanta errors i proves mínimes? | cas positiu, cas negatiu, errors i neteja |
| Després de `MP6` | Una altra persona podria arrancar i entendre el projecte? | README, demo, decisions i backlog |

## Adaptacions de ritme

### Alumnat endarrerit

- limitar el domini a una entitat central i una relació opcional
- triar dos fluxos molt xicotets però reals
- prioritzar arrencada, BBDD, migracions, seeders i proves mínimes
- ajornar millores visuals, funcionalitats secundàries i relacions complexes
- no eliminar el segon flux: reduir-lo al mínim funcional

### Alumnat avançat

- afegir més cobertura de proves
- millorar gestió d'errors
- incorporar una relació simple entre entitats
- preparar un contracte preliminar d'`API`
- documentar decisions amb més precisió
- migrar un tercer flux només si els mínims de `R3` ja estan tancats

## Errors habituals a tallar prompte

- convertir `R3` en una comparativa teòrica de frameworks
- fer només instal·lació i captures
- migrar fitxers de `R2` sense adaptar-los al framework
- no usar `migrations` o `seeders`
- simular dades en arrays quan ja toca BBDD
- implementar només un flux
- no poder explicar quin flux ve de `R2`
- fer el segon flux com a canvi visual
- no provar errors
- escriure un README que no permet arrancar el projecte

## Condició d'entrada a `R4`

L'equip pot passar a `R4` quan pot demostrar:

- aplicació en framework operativa
- Docker funcional
- BBDD creada per `migrations`
- dades inicials amb `seeders` o equivalent
- `2` casos d'ús end-to-end
- almenys `1` flux heretat de `R2`
- validació i errors mínims
- proves mínimes o verificacions reproduïbles
- documentació tècnica curta
- backlog o mapa del que queda per migrar

Si falta algun d'estos punts, `R4` s'ha d'ajustar o ajornar, perquè publicar una `API` sobre una base no reproduïble convertiria el problema en més difícil de verificar.
