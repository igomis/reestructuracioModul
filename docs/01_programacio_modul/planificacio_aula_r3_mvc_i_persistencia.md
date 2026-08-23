# R3. Planificació d'aula — MVC i persistència

## Finalitat del bloc

Este document baixa `R3` a una seqüència operativa d'aula perquè el professorat puga conduir la reconstrucció del projecte en framework amb base operativa real, persistència mínima real i primers fluxos funcionals verificables.

No redefineix el repte. La referència conceptual i avaluable continua sent [repte_03_mvc_i_persistencia.md](../02_reptes/repte_03_mvc_i_persistencia.md). Esta planificació concreta com portar-lo a classe: què convé modelar, què ha de produir l'alumnat, quines evidències mínimes cal exigir i quan es pot considerar que la base està preparada per entrar a `R4`.

`R3` no demana migrar tota l'aplicació heretada de `R2`. Demana construir una nova base real en framework i portar-hi almenys `2` casos d'ús end-to-end, amb almenys `1` flux heretat de `R2`. El segon pot ser també migrat o una ampliació funcional xicoteta si fa visible el valor del framework.

## Posició de `R3` dins del curs

`R3` s'obri al final de l'avaluació 1 i es tanca a l'inici de l'avaluació 2.

En la seqüència de `20` setmanes del repositori, això correspon a:

- `Setmana 9`: arrencada del projecte en framework, Docker i rutes mínimes.
- `Setmana 10`: model de dades, BBDD real, migracions o equivalent, càrrega inicial reproduïble i taller de portabilitat entre frameworks.
- `Setmana 11`: primer cas d'ús complet migrat de `R2`.
- `Setmana 12`: segon cas d'ús o ampliació funcional, estabilització i tancament tècnic.

`R2` queda tancat com a base comuna en `PHP`: formulari, validació, processament, estat, autenticació i una funcionalitat protegida han d'existir com a referència funcional. `R3` no torna a fer eixe flux de la mateixa manera ni el migra tot: reconstrueix una base real en `Laravel`, `Symfony` o `NestJS` i selecciona fluxos troncals verificables.

Els itineraris tecnològics funcionen com a suport de stack:

- mateixa seqüència docent
- mateixes evidències mínimes
- mateixos checkpoints
- diferent nomenclatura tècnica segons el framework

## Relació amb `RA5`, `RA6` i `RA8`

El nucli de `R3` és `RA5`: usar el framework per separar entrada HTTP, coordinació, lògica, presentació o resposta i responsabilitats internes.

`RA6` s'activa com a suport fort i parcial: la persistència ha de ser real, segura i suficient per als fluxos prioritzats, però no cal convertir el repte en el model complet de dades de tot el producte.

`RA8` queda integrat de manera explícita perquè almenys un flux de `R3` ha de generar una resposta `HTML` en servidor amb vista o plantilla, dades reals i una interacció processada pel framework.

Lectura docent:

- `RA5` marca si l'arquitectura del framework és clara, mantenible i explicable.
- `RA6` marca si l'accés a dades és real, coherent, verificable i integrat en fluxos funcionals.
- `RA8` marca si el framework s'usa també per generar pàgines dinàmiques, no només com a estructura interna o futura `API`.
- `R4` només té sentit si `R3` deixa una base persistent que es pot exposar després com a `API` sense improvisació.

## Duració recomanada

El document del repte situa `R3` en una duració orientativa de `10` sessions obligatòries si es compta la transició, el taller de portabilitat i la microdefensa.

Opció docent preferent:

- `10` sessions de `3` hores, incloent `R3S0`, el taller `R3S2B` i la microdefensa `R3SX`
- `30` hores aproximades
- `4` setmanes de treball en el model de `6` hores setmanals
- inici al final de l'avaluació 1
- tancament a l'inici de l'avaluació 2

Compactació possible:

- no convé compactar eliminant `R3S2B`, perquè és la sessió que assegura portabilitat i comprensió real entre stacks.
- si cal ajustar ritme, es reduïx l'abast dels fluxos o es concentra la microdefensa, però no s'elimina el contrast de frameworks.

Si cal reduir abast, es redueix la mida dels fluxos, no els mínims: Docker, projecte arrancable, BBDD real, migracions o equivalent, dades inicials reproduïbles, `2` casos d'ús, autenticació/autorització mínima, validació, errors, proves i README.

## Correspondència entre microprojectes i sessions

| Microprojecte | Sessions | RA avaluat | CA avaluats | RA de context | Producte parcial esperat | Evidència mínima | Checkpoint docent |
|---|---|---|---|---|---|---|---|
| `R3M1` Arrencada del nou projecte | `1` | `RA5` | `RA5.a`, `RA5.b`, `RA5.c`, `RA5.d`, `RA5.e` | `RA8.c` | stack triat, Docker, projecte base, `.env` i rutes mínimes | projecte arrancable, ruta o vista inicial, issue de `R3` i declaració dels `2` fluxos | no és només esquelet: arranca i té abast funcional definit |
| `R3M2` Model de dades i persistència mínima | `2-3` | `RA6` | `RA6.a`, `RA6.b`, `RA6.c`, `RA6.d`, `RA6.e` | `RA5.f` | BBDD real amb esquema inicial i dades de prova | migracions o equivalent, càrrega inicial, connexió i lectura real | la BBDD es pot reconstruir sense càrrega manual |
| `R3M3` Primer cas d'ús complet | `3-4` | `RA8` | `RA8.d`, `RA8.e`, `RA8.g` | `RA5.e`, `RA5.f`, `RA5.g`, `RA6.c`, `RA6.d`, `RA6.f` | primer flux end-to-end migrat de `R2` | ruta, controlador, model/servei, vista o plantilla, BBDD, resposta `HTML` si és el flux server-rendered i validació mínima | el flux ve de `R2` i funciona amb dades reals |
| `R3M4` Segon cas d'ús o ampliació funcional | `5-6` | `RA8` | `RA8.f`, `RA8.g` | `RA5.e`, `RA5.f`, `RA5.g`, `RA5.h`, `RA6.c`, `RA6.d`, `RA6.f` | segon flux end-to-end o ampliació útil | recorregut funcional, BBDD, validació/error, canvi dinàmic de resposta i demo | no és canvi cosmètic ni duplicació buida |
| `R3M5` Autenticació, autorització i middleware | `6` | `RA5` | `RA5.f`, `RA5.g`, `RA5.h` | `RA6.f`, `RA8.g` | acció significativa protegida | login, middleware/guard/voter/policy o equivalent, cas autoritzat i denegat | la protecció està en servidor i no només en la vista |
| `R3M6` Qualitat i estabilització | `7-8` | `RA5` | `RA5.g`, `RA5.h` | `RA6.f`, `RA6.g` | validació, errors, proves i neteja d'estructura | proves mínimes, cas positiu/negatiu, revisió de responsabilitats i protecció intacta | els fluxos continuen funcionant després de la neteja |
| `R3M7` Tancament tècnic | `9` | `RA5` | `RA5.f`, `RA5.g` | `RA6.g` | README, decisions, demo i backlog de migració | instruccions d'arrencada, fluxos documentats, acció protegida i mapa del que queda | només s'obri `R4` si la base és reproduïble i defensable |

El solapament entre microprojectes és intencionat. `R3M2` pot començar mentre encara es tanca `R3M1`, `R3M5` aprofita els fluxos ja construïts per protegir una acció real, i `R3M6` pot actuar sobre `R3M3-R3M5` a mesura que apareixen errors. El criteri és mantindre un producte executable en tot moment.

## Seqüència detallada de 10 sessions de 3 hores

### Sessió 1. Arrencada del nou projecte

**Microprojecte principal**

- `R3M1 — Arrencada del nou projecte`

**Objectiu**

Triar l'stack, comparar-lo amb una alternativa, preparar Docker, crear el projecte base del framework i verificar una primera ruta mínima.

**Què explica el professorat**

- per què `R3` no és migrar tota l'aplicació de `R2`
- què vol dir base real en framework
- per què separar ruta, controlador, vista o resposta i model millora la base de `R2`
- com comparar dos frameworks sense convertir-ho en teoria abstracta
- quins mínims tècnics no es poden ajornar: Docker, `.env`, rutes i arrencada
- com declarar un abast de `2` casos d'ús sense obrir una reescriptura total

**Què modela el professorat**

- arrencada d'un projecte base en el framework triat
- comparació curta entre el framework triat i una alternativa
- esquema abans/després de responsabilitats entre `R2` i la nova base
- configuració mínima de Docker i `.env`
- ruta o `healthcheck`
- issue principal de `R3` amb microtasques

**Tasques**

- triar `Laravel`, `Symfony`, `NestJS` o via excepcional autoritzada
- comparar l'stack triat amb almenys una altra opció viable
- justificar els avantatges de separar responsabilitats respecte a `R2`
- crear o estabilitzar el projecte base
- preparar Docker i configuració mínima
- crear una ruta inicial
- declarar els `2` casos d'ús de `R3`
- indicar quin cas d'ús ve de `R2`
- indicar quin cas d'ús quedarà renderitzat en servidor amb vista o plantilla

**Evidència mínima**

- projecte arrancable amb Docker
- nota comparativa de stack
- esquema abans/després de responsabilitats
- `.env.example` o instruccions equivalents
- ruta inicial funcional o vista mínima generada pel framework
- issue principal amb els `2` fluxos

**Checkpoint docent**

L'aplicació ha d'arrancar i la tria del framework ha d'estar justificada amb avantatges concrets de separació de responsabilitats. Si només hi ha instal·lació parcial o carpetes del framework sense execució, no es passa a la sessió següent.

### Sessió 2. Model de dades inicial

**Microprojecte principal**

- `R3M2 — Model de dades i persistència mínima`

**Objectiu**

Definir l'esquema mínim de dades i crear la primera migració vinculada als fluxos de `R3`.

**Què explica el professorat**

- diferència entre persistència real i dades de demo incrustades
- relació entre cas d'ús, entitat, migració i model o equivalent
- què és una dada mínima suficient per provar un flux
- què significa recuperar i tractar un conjunt de dades perquè alimente un flux real

**Què modela el professorat**

- una migració simple
- un model, entitat o esquema
- configuració de connexió a BBDD
- consulta que retorna un conjunt de dades
- comprovació de taula creada

**Tasques**

- definir les entitats o taules mínimes
- crear migracions o mecanisme equivalent
- configurar connexió de BBDD
- executar migracions
- preparar una consulta o recuperació de conjunt de dades per a un llistat, detall, filtre o resposta
- registrar decisions de model de dades

**Evidència mínima**

- BBDD creada per migracions o mecanisme equivalent
- esquema inicial coherent amb els fluxos
- primera recuperació de conjunt de dades prevista per alimentar un flux
- comprovació de connexió i estructura

**Checkpoint docent**

La BBDD ha de poder crear-se de zero. Si l'esquema només existeix manualment en una eina gràfica o local, no és suficient.

### Sessió 3. Dades inicials i primera lectura real

**Microprojecte principal**

- `R3M2 — Model de dades i persistència mínima`

**Microprojecte secundari**

- inici de `R3M3 — Primer cas d'ús complet`

**Objectiu**

Carregar dades inicials reproduïbles i preparar la primera lectura real de conjunt de dades des del framework.

**Què explica el professorat**

- per què una càrrega inicial reproduïble evita demos irreproduïbles
- com comprovar dades sense dependre de l'estat local d'una màquina
- com un conjunt de dades recuperat prepara el primer flux

**Què modela el professorat**

- fixture, seeder o script equivalent
- reset de BBDD i recàrrega de dades
- lectura d'un conjunt de dades des d'un controlador, servei o consola del framework i ús en una vista, llistat o resposta

**Tasques**

- crear fixtures/seeders o script equivalent
- carregar dades de demostració
- verificar lectura real d'un conjunt de dades
- usar eixe conjunt de dades en un llistat, detall, filtre o resposta equivalent
- documentar com reiniciar BBDD i dades

**Evidència mínima**

- dades inicials reproduïbles
- lectura real d'un conjunt de dades i ús dins d'un flux
- instruccions de reset de BBDD

**Checkpoint docent**

Les dades han de poder aparéixer després d'un reset i alimentar un flux real. Si cal inserir-les a mà, el repte encara no té persistència reproduïble.

### Sessió 3B. Taller de portabilitat entre frameworks

**Sessió formativa sense microrepte propi**

- reforç de `R3M1` i `R3M2`
- preparació de `R3M3`

**Objectiu**

Comprovar que l'alumnat entén les equivalències entre `Laravel`, `Symfony` i `NestJS` abans de construir el primer flux complet.

**Tasques**

- completar una taula d'equivalències del seu stack respecte a un altre;
- localitzar en el repositori ruta, controlador, capa de dades, model, migració o equivalent, càrrega inicial, vista/resposta i prova;
- explicar com es reconstrueix la BBDD i com es carreguen dades inicials;
- preparar una mini defensa del recorregut petició -> resposta;
- registrar una microtasca de correcció.

**Evidència mínima**

- taula d'equivalències;
- auditoria curta del projecte;
- microtasca registrada abans d'entrar a `R3M3`.

### Sessió 4. Primer cas d'ús complet migrat de `R2`

**Microprojecte principal**

- `R3M3 — Primer cas d'ús complet`

**Objectiu**

Portar al framework un cas d'ús real heretat de `R2` amb recorregut complet.

**Què explica el professorat**

- recorregut d'una petició pel framework
- rols de ruta, controlador, model o servei i vista o resposta
- què aporta una vista o plantilla server-rendered dins de `R3`
- criteri de validació mínima i error controlat

**Què modela el professorat**

- una ruta connectada amb un controlador
- lectura de BBDD dins del flux
- resposta amb plantilla o vista quan este siga el flux server-rendered
- validació o error mínim

**Tasques**

- implementar ruta del primer cas d'ús
- crear o ajustar controlador i servei o equivalent
- llegir dades reals
- passar dades del controlador a una vista o plantilla, o justificar si aquest no és el flux server-rendered
- retornar resposta `HTML` generada pel framework en almenys un cas d'ús de `R3`
- afegir validació mínima si escau
- registrar prova del cas positiu

**Evidència mínima**

- primer flux end-to-end funcionant
- traça que el flux ve de `R2`
- BBDD implicada en el flux
- vista o plantilla amb dades reals si aquest és el flux server-rendered
- validació o error mínim

**Checkpoint docent**

El cas d'ús ha de ser funcional de punta a punta. Una pantalla que només mostra dades estàtiques no tanca `R3M3`.

### Sessió 5. Segon flux o ampliació funcional

**Microprojecte principal**

- `R3M4 — Segon cas d'ús o ampliació funcional`

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
- fer que el contingut generat canvie segons dades, paràmetres, estat, filtre o formulari
- afegir validació o error mínim
- verificar demo end-to-end

**Evidència mínima**

- segon flux executable
- justificació del seu valor
- canvi dinàmic visible en la resposta generada
- prova o verificació mínima

**Checkpoint docent**

No compta com a segon flux una pàgina estàtica, una còpia del primer canviant noms o una millora només visual.

### Sessió 6. Autenticació, autorització i middleware

**Microprojecte principal**

- `R3M5 — Autenticació, autorització i middleware`

**Objectiu**

Protegir una acció significativa amb autenticació del framework, autorització mínima i cas denegat verificable.

**Què explica el professorat**

- diferència entre autenticació i autorització
- per què ocultar una vista no protegeix el servidor
- equivalències entre middleware, guard, voter i policy

**Què modela el professorat**

- login i logout o invalidació
- ruta protegida
- cas autoritzat i cas denegat

**Tasques**

- preparar usuari demo
- protegir una acció real
- aplicar middleware, guard, voter, policy o equivalent
- documentar regla d'autorització
- verificar cas sense autenticar, autoritzat i denegat

**Evidència mínima**

- acció protegida en servidor
- cas autoritzat i cas denegat
- instruccions de prova

**Checkpoint docent**

No es considera protecció si només s'oculta un botó o enllaç però la ruta continua accessible.

### Sessió 7. Validació, errors i primera bateria de proves

**Microprojecte principal**

- `R3M6 — Qualitat i estabilització`

**Objectiu**

Fer que els fluxos principals tinguen validació, errors bàsics i proves mínimes o verificacions reproduïbles.

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
- verificar que l'acció protegida continua funcionant

**Evidència mínima**

- proves o verificacions registrades
- errors controlats visibles
- fluxos encara funcionant
- protecció d'accessos intacta

**Checkpoint docent**

No es considera qualitat mínima si només hi ha una demo feliç sense cap entrada incorrecta o situació d'error.

### Sessió 8. Estabilització d'estructura

**Microprojecte principal**

- `R3M6 — Qualitat i estabilització`

**Microprojecte secundari**

- inici de `R3M7 — Tancament tècnic`

**Objectiu**

Revisar responsabilitats, netejar duplicacions i assegurar que migracions o equivalent, càrrega inicial i fluxos continuen funcionant.

**Què explica el professorat**

- com detectar controladors massa carregats
- què vol dir responsabilitat clara segons cada framework
- per què una neteja no ha de trencar la reproducció de dades

**Què modela el professorat**

- refactorització mínima d'un controlador o servei
- reexecució de migracions o equivalent i càrrega inicial
- prova ràpida dels dos fluxos després de la neteja

**Tasques**

- revisar rutes, controladors, serveis i models o equivalents
- eliminar duplicacions evidents
- comprovar migracions o equivalent i càrrega inicial
- repetir proves dels dos fluxos
- començar README tècnic

**Evidència mínima**

- estructura revisada
- migracions o equivalent i càrrega inicial encara funcionant
- proves repetides després de la neteja

**Checkpoint docent**

La neteja només és vàlida si el sistema continua arrancant i els dos fluxos continuen vius.

### Sessió 9. Tancament tècnic i pas a `R4`

**Microprojecte principal**

- `R3M7 — Tancament tècnic`

**Objectiu**

Tancar `R3` amb documentació executable, demostració curta, decisions tècniques i mapa del que queda per migrar.

**Què explica el professorat**

- com escriure un README que una altra persona puga seguir
- com distingir el que s'ha migrat del que queda pendent
- com decidir quins recursos poden passar a `R4`

**Què modela el professorat**

- estructura curta de README
- backlog de migració
- demo de tancament amb arrencada, BBDD, càrrega inicial i dos fluxos

**Tasques**

- actualitzar README
- documentar arrencada, `.env`, migracions o equivalent i càrrega inicial
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
| Després de `R3M1` | El projecte en framework arranca de veritat? | Docker, `.env`, ruta mínima i issue amb `2` fluxos |
| Després de `R3M2` | La persistència es pot reconstruir de zero? | migracions o equivalent, càrrega inicial, BBDD i lectura real |
| Després de `R3M3` | Hi ha un flux de `R2` migrat i funcional? | ruta, controlador, dades reals, vista/resposta i validació |
| Després de `R3M4` | Hi ha un segon flux real? | segon recorregut end-to-end, no cosmètic |
| Després de `R3M5` | Hi ha una acció protegida real? | login, logout, cas autoritzat, cas denegat i middleware/guard/voter/policy o equivalent |
| Després de `R3M6` | El projecte aguanta errors i proves mínimes? | cas positiu, cas negatiu, errors, acció protegida i neteja |
| Després de `R3M7` | Una altra persona podria arrancar i entendre el projecte? | README, demo, decisions i backlog |

## Adaptacions de ritme

### Alumnat endarrerit

- limitar el domini a una entitat central i una relació opcional
- triar dos fluxos molt xicotets però reals
- prioritzar arrencada, BBDD, migracions o equivalent, càrrega inicial i proves mínimes
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
- no usar migracions o equivalent ni càrrega inicial reproduïble
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
- BBDD creada per migracions o equivalent
- dades inicials amb fixtures/seeders o script equivalent
- `2` casos d'ús end-to-end
- almenys `1` flux heretat de `R2`
- almenys `1` flux server-rendered amb vista o plantilla i resposta `HTML` generada en servidor
- validació i errors mínims
- proves mínimes o verificacions reproduïbles
- documentació tècnica curta
- backlog o mapa del que queda per migrar

Si falta algun d'estos punts, `R4` s'ha d'ajustar o ajornar, perquè publicar una `API` sobre una base no reproduïble convertiria el problema en més difícil de verificar.
