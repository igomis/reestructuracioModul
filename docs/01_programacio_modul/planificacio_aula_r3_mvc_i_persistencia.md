# Planificació d'aula del Repte 3

## Finalitat del bloc

Este document baixa `R3` a una seqüència operativa d'aula perquè el professorat puga conduir el pas des de la base comuna de `R2` cap a una arquitectura més mantenible, amb persistència real i verificable, sense convertir el repte en tres cursos paral·lels de framework.

No redefineix el repte. La referència conceptual i avaluable continua sent [repte_03_mvc_i_persistencia.md](../02_reptes/repte_03_mvc_i_persistencia.md). Esta planificació concreta com portar-lo a classe: què convé modelar, què ha de produir l'alumnat, quines evidències mínimes cal exigir i quan es pot considerar que la base està preparada per entrar a `R4`.

El producte continua sent el mateix que ve de `R2`. El canvi de `R3` és que un cas d'ús real passa d'una implementació funcional però encara acoblada a una base més estructurada, persistent, verificable i defensable.

## Posició de `R3` dins del curs

`R3` s'obri al final de l'avaluació 1 i es tanca a l'inici de l'avaluació 2.

En la seqüència de 20 setmanes del repositori, això correspon a:

- `Setmana 9`: entrada a arquitectura i persistència inicial.
- `Setmana 10`: tancament de la primera avaluació amb `R3` obert i encaminat.
- `Setmana 11`: consolidació de persistència i regressió.
- `Setmana 12`: tancament formal de `R3` i validació d'entrada a `R4`.

`R2` queda tancat com a base comuna en `PHP`: formulari, validació, processament, estat, autenticació i una funcionalitat protegida han d'existir com a referència funcional. `R3` no torna a fer eixe flux des de zero; el professionalitza dins de `Laravel`, `Symfony` o `NestJS`.

Els itineraris tecnològics funcionen com a suport de stack:

- mateixa seqüència docent
- mateixes evidències mínimes
- mateixos checkpoints
- diferent nomenclatura tècnica segons el framework

## Relació amb `RA5` i preparació de `RA6`

El nucli de `R3` és `RA5`: separació de presentació, lògica de negoci, coordinació del flux i estructura interna de l'aplicació.

`RA6` s'activa com a suport integrat: la persistència ha de ser real, segura i suficient per al cas d'ús prioritzat, però no cal convertir el repte en un model complet de dades de tot el producte.

Lectura docent:

- `RA5` marca si l'arquitectura és més clara, mantenible i explicable.
- `RA6` marca si l'accés a dades és real, coherent, verificable i integrat en el flux.
- `R4` només té sentit si la base persistent de `R3` pot exposar-se després com a `API` sense improvisació.

## Duració recomanada

El document del repte situa `R3` en una duració orientativa de `6` a `8` sessions.

Opció docent preferent:

- `8` sessions de `3` hores
- `24` hores aproximades
- `4` setmanes de treball en el model de `6` hores setmanals
- inici al final de l'avaluació 1
- tancament a l'inici de l'avaluació 2

Compactació possible:

- `6` sessions si el grup arriba amb `R2` molt sòlid, el cas d'ús és molt acotat i l'stack no introdueix fricció significativa.
- no convé compactar per davall de `6` sessions perquè desapareix la verificació real de persistència, regressió i defensa.

## Justificació de per què es proposen 8 sessions

La proposta de `8` sessions evita compactar artificialment un repte que té tres moviments diferents:

- diagnosticar i decidir què es migra
- reorganitzar el cas d'ús en una arquitectura més mantenible
- consolidar persistència, regressió, documentació i defensa

També encaixa millor amb la seqüència real del curs: dues setmanes finals de l'avaluació 1 per obrir el canvi i dues setmanes inicials de l'avaluació 2 per tancar-lo amb garanties.

La distribució de `8` sessions permet que els microprojectes de `R3` no queden reduïts a una demo:

| Tram | Sessions | Microprojectes principals | Sentit docent |
|---|---:|---|---|
| Obertura i diagnosi | `1-2` | `MP1` | auditar el codi real, triar cas d'ús i planificar la migració |
| Migració arquitectònica | `3-4` | `MP2` | entrar al framework i migrar el primer cas d'ús amb separació visible |
| Consolidació de capes | `5` | `MP3` | ajustar controladors, serveis, presentació o equivalents |
| Persistència aplicada | `6` | `MP4` | integrar lectura i escriptura persistents en el cas d'ús |
| Qualitat i regressió | `7` | `MP5` | validar entrada, errors i continuïtat funcional |
| Tancament i pas a `R4` | `8` | `MP6` | documentar, defensar i decidir entrada a API |

## Seqüència detallada de 8 sessions de 3 hores

### Sessió 1. Diagnosi inicial del codi de `R2`

**Microprojecte vinculat**

- `MP1 — Diagnosi del codi actual i pla de migració`

**Objectiu**

Auditar el cas d'ús candidat de `R2` i detectar problemes concrets de mantenibilitat, acoblament o persistència.

**Què explica el professorat**

- per què `R3` no és repetir `R2` dins d'un framework
- què diferencia una diagnosi real d'una llista genèrica sobre MVC
- com llegir un flux existent buscant responsabilitats barrejades
- quina evidència mínima ha de quedar abans de tocar codi

**Què modela el professorat**

- lectura curta d'un flux existent amb `HTML`, entrada HTTP, lògica i dades barrejades
- identificació d'acoblaments, duplicitats i punts fràgils
- taula simple de responsabilitats actuals

**Què fa l'alumnat**

- selecciona un cas d'ús real heretat de `R2`
- identifica fitxers, rutes, funcions, dades i punts de decisió implicats
- registra què funciona ara i què no és mantenible
- obri issue principal o registre equivalent de `R3`

**Evidència mínima**

- cas d'ús candidat
- diagnosi breu del codi actual
- mapa inicial de responsabilitats o dependències
- primer registre d'incidències tècniques

**Checkpoint docent**

El cas d'ús ha de ser real, funcional i vinculat al projecte. Si la diagnosi podria aplicar-se a qualsevol pràctica genèrica, no és suficient.

### Sessió 2. Selecció definitiva del cas d'ús i pla de migració

**Microprojecte vinculat**

- `MP1 — Diagnosi del codi actual i pla de migració`

**Objectiu**

Tancar el cas d'ús que es professionalitzarà, decidir l'stack i convertir la diagnosi en un pla de migració per iteracions curtes.

**Què explica el professorat**

- com triar un abast viable per a `R3`
- com usar `Laravel`, `Symfony` o `NestJS` com a suport de stack sense canviar l'objectiu docent
- com escriure microtasques revisables
- què ha d'estar preparat per començar a migrar sense perdre control

**Què modela el professorat**

- pla curt de migració amb passos ordenats
- comparació abans/després esperada
- criteri de risc: què es pot ajornar i què bloqueja el repte

**Què fa l'alumnat**

- confirma el cas d'ús prioritari
- tria `Laravel`, `Symfony` o `NestJS`
- defineix quines responsabilitats passaran a controlador, servei, presentació, model, repositori o equivalents
- concreta microtasques i criteris de prova
- deixa preparada la base del framework o el pla d'arrencada si encara no està creada

**Variants de stack**

- `Laravel`: ruta, controlador, request o validació, servei o acció, model/migració i vista o resposta.
- `Symfony`: ruta, controlador, servei, formulari/DTO si aplica, entitat/repositori i plantilla o resposta.
- `NestJS`: mòdul, controlador, servei, DTO, entitat/esquema i capa d'accés a dades.

**Evidència mínima**

- stack triat i justificat
- pla de migració amb passos curts
- issue principal amb microtasques
- definició de prova mínima abans/després

**Checkpoint docent**

El professorat valida que el pla no és una reescriptura total, que no duplica indefinidament `R2` i que deixa clar quin comportament s'ha de conservar.

### Sessió 3. Entrada real al framework i primera migració estructural

**Microprojecte vinculat**

- `MP2 — Separació de capes i migració del primer cas d'ús`

**Objectiu**

Introduir o estabilitzar l'estructura base del framework triat i portar-hi el primer tram executable del cas d'ús.

**Què explica el professorat**

- què és estructura recognoscible del framework i què és arquitectura buida
- com fer un controlador prim o equivalent
- com mantindre commits incrementals durant una migració
- com provar després de cada canvi significatiu

**Què modela el professorat**

- una ruta o entrada HTTP del cas d'ús dins del framework
- un controlador mínim que no absorbeix tota la lògica
- una comprovació immediata del flux parcial

**Què fa l'alumnat**

- crea o ajusta l'estructura base del framework
- migra l'entrada del cas d'ús
- conserva el comportament principal encara que siga en versió parcial
- registra la comparació amb el punt de partida

**Evidència mínima**

- projecte del framework arrancable
- entrada del cas d'ús dins del nou stack
- primer commit de migració estructural
- demo parcial reproduïble

**Checkpoint docent**

No basta que el framework arranque. Ha d'existir una connexió clara entre el cas d'ús de `R2` i el nou recorregut.

### Sessió 4. Separació real de responsabilitats

**Microprojecte vinculat**

- `MP2 — Separació de capes i migració del primer cas d'ús`

**Objectiu**

Separar entrada, coordinació, lògica i resposta de manera visible i funcional.

**Què explica el professorat**

- com detectar si un controlador, servei o vista està assumint massa responsabilitats
- com moure lògica sense trencar el flux
- com comprovar que la separació no és només de noms

**Què modela el professorat**

- extracció d'una regla de negoci o coordinació a servei, cas d'ús o equivalent
- separació de preparació de resposta i lògica
- prova curta del cas positiu després de la refactorització

**Què fa l'alumnat**

- reorganitza el cas d'ús amb rols tècnics clars
- redueix mescles entre presentació, lògica i accés a dades
- documenta què ha canviat respecte de `R2`
- comprova que el comportament principal continua viu

**Evidència mínima**

- cas d'ús migrat o reconstruït en una primera versió funcional
- separació visible de responsabilitats
- comparativa breu abans/després
- commits de migració incremental

**Checkpoint docent**

L'alumnat ha de poder respondre què fa cada peça i què no hauria de fer. Si la lògica continua concentrada en una sola peça, el checkpoint queda pendent.

### Sessió 5. Consolidació de capes o equivalents

**Microprojecte vinculat**

- `MP3 — Controladors, serveis i components de presentació o equivalent`

**Objectiu**

Revisar i consolidar les fronteres internes del mòdul perquè la nova estructura siga defensable i preparada per connectar persistència.

**Què explica el professorat**

- com s'interpreten les capes en cada stack sense imposar la mateixa nomenclatura
- quins símptomes indiquen duplicació o responsabilitats confuses
- com preparar la capa de dades sense fer encara una persistència ornamental

**Què modela el professorat**

- revisió d'un controlador massa gros
- ajust d'un servei o cas d'ús
- separació entre dades que venen del domini i dades preparades per a la resposta

**Què fa l'alumnat**

- revisa controladors, serveis, plantilles, DTO, casos d'ús o equivalents
- ajusta noms, dependències i fronteres
- prepara el punt d'entrada cap a model, entitat, repositori o mecanisme persistent
- deixa una justificació breu de rols tècnics

**Evidència mínima**

- estructura final provisional del mòdul
- justificació dels rols tècnics
- demo del flux complet o quasi complet
- registre d'ajustos realitzats

**Checkpoint docent**

El professorat pot demanar un microcanvi en viu sobre una regla, resposta o validació. La ubicació del canvi ha de ser coherent amb l'arquitectura defensada.

### Sessió 6. Model de dades i persistència segura aplicada

**Microprojecte vinculat**

- `MP4 — Persistència segura aplicada al cas d'ús prioritari`

**Objectiu**

Consolidar una persistència real i suficient sobre el cas d'ús migrat, amb lectura i escriptura o actualització verificables.

**Què explica el professorat**

- què és persistència verificable i què és simulació
- com encaixa l'accés a dades dins de cada stack
- per què no cal modelar-ho tot, però sí el recurs central del cas d'ús
- quins errors de dades s'han de controlar des del principi

**Què modela el professorat**

- model, entitat, migració, esquema o equivalent del recurs central
- lectura real de dades dins del flux
- operació de creació, actualització o equivalent
- comprovació abans/després amb base de dades, consola, logs o prova reproduïble

**Què fa l'alumnat**

- defineix el recurs persistent central
- implementa model, entitat, migració, esquema o repositori segons el stack
- integra lectura de dades en el cas d'ús
- implementa una operació d'escriptura, actualització o equivalent
- prova que la dada persisteix fora de l'estat temporal

**Variants de stack**

- `Laravel`: migració, model `Eloquent`, relació mínima si és necessària i ús des d'un servei o controlador prim.
- `Symfony`: entitat, repositori, migració o actualització d'esquema controlada i ús des d'un servei.
- `NestJS`: DTO, servei, entitat o esquema segons ORM/ODM i accés encapsulat en servei o repositori.

**Evidència mínima**

- recurs persistent definit
- lectura real de dades
- escriptura, actualització o operació equivalent verificable
- prova abans/després
- commit associat a persistència

**Checkpoint docent**

El professorat demana demostrar lectura i modificació de dades. El resultat ha de poder comprovar-se fora de la pantalla final de la demo.

### Sessió 7. Validacions, errors i regressió mínima

**Microprojecte vinculat**

- `MP5 — Validacions, errors i regressió mínima`

**Objectiu**

Assegurar que el cas d'ús refactoritzat i persistent continua funcionant i respon correctament davant dades incorrectes o situacions d'error.

**Què explica el professorat**

- com construir una regressió mínima útil
- què ha d'incloure un cas positiu i un cas negatiu
- com evitar proves fictícies o només narrades
- com registrar incidències i correccions

**Què modela el professorat**

- checklist curta de prova del flux complet
- error provocat i tractat de manera visible
- verificació de persistència després de l'error o de la correcció

**Què fa l'alumnat**

- prova el cas positiu principal
- provoca almenys un error significatiu
- revisa validacions i tractament d'errors
- registra incidències detectades i correccions
- comprova que el flux de `R2` continua viu després de la migració

**Evidència mínima**

- registre de proves mínimes
- cas positiu i cas negatiu
- error visible o controlat
- incidències i correccions
- demo del flux complet verificat

**Checkpoint docent**

El professorat contrasta prova, codi i comportament real. Si la prova no s'executa o no es pot reproduir, no compta com a regressió.

### Sessió 8. Documentació, defensa breu i validació d'entrada a `R4`

**Microprojecte vinculat**

- `MP6 — Documentació tècnica i preparació del Repte 4`

**Objectiu**

Tancar `R3` amb documentació coherent, defensa tècnica breu i decisió explícita sobre si el projecte pot entrar a `R4`.

**Què explica el professorat**

- què ha de quedar al `README` o documentació equivalent
- com explicar decisions arquitectòniques sense fer narrativa fictícia
- com connectar el recurs persistent amb el futur contracte d'`API`
- quins deutes tècnics bloquegen i quins poden quedar registrats

**Què modela el professorat**

- estructura d'una defensa de 3 minuts: punt de partida, canvi, prova, límit i pas a `R4`
- revisió d'un `README` tècnic coherent amb el repositori
- contrast entre commits, proves i documentació

**Què fa l'alumnat**

- actualitza `README`, decisions tècniques o `ADR`
- registra deute tècnic pendent
- completa `AI log` si ha usat IA
- prepara defensa breu
- identifica quin recurs o flux podrà exposar-se en `R4`

**Evidència mínima**

- documentació tècnica actualitzada
- registre de decisions
- deute tècnic classificat
- defensa tècnica breu
- proposta de base per a `R4`

**Checkpoint docent**

El professorat valida entrada a `R4` només si codi, persistència, proves, documentació i defensa són coherents entre si.

## Relació entre sessions i microprojectes / microreptes ja definits al document de `R3`

| Sessió | Microprojecte de `R3` | Motiu de la distribució |
|---|---|---|
| `1` | `MP1` | auditoria inicial del codi i detecció de problemes reals |
| `2` | `MP1` | tancament del cas d'ús, stack i pla de migració |
| `3` | `MP2` | entrada real al framework i primera migració executable |
| `4` | `MP2` | separació de responsabilitats i conservació del comportament |
| `5` | `MP3` | consolidació de controladors, serveis, presentació o equivalents |
| `6` | `MP4` | model de dades i persistència segura aplicada |
| `7` | `MP5` | validacions, errors i regressió mínima |
| `8` | `MP6` | documentació, defensa i preparació de `R4` |

`MP1` i `MP2` ocupen més d'una sessió perquè són els punts amb més risc metodològic: una diagnosi feble porta a una migració superficial, i una entrada precipitada al framework sol generar capes nominals sense millora real.

## Què modela el professorat

El professorat ha de modelar peces curtes i transferibles, no una implementació completa:

- lectura d'un flux existent i detecció d'acoblaments
- mapa de responsabilitats actuals i futures
- pla de migració incremental
- entrada mínima al framework triat
- refactorització curta amb prova immediata
- separació entre controlador, servei, presentació i dades o equivalents
- creació d'un recurs persistent mínim
- comprovació de lectura i escriptura
- regressió mínima amb cas positiu i negatiu
- defensa tècnica breu basada en evidències

La clau és ensenyar el mètode de treball i el criteri de verificació, no donar una plantilla tancada per copiar.

## Què pot deixar-se parcialment a la IA

La IA pot actuar com a suport habitual en:

- detectar possibles acoblaments a partir d'un fragment de codi
- suggerir preguntes d'auditoria del flux
- proposar un pla de refactorització per passos
- generar esquelets inicials de controlador, servei, DTO, model, entitat o repositori
- suggerir casos de prova i errors a provocar
- revisar missatges d'error o documentació tècnica
- comparar convencions de `Laravel`, `Symfony` i `NestJS` per a una mateixa responsabilitat

Controls obligatoris:

- l'alumnat ha de poder explicar cada peça acceptada
- cap codi generat substitueix la prova real
- les decisions importants han de quedar en issue, commit, `README`, `ADR` o registre equivalent
- si hi ha ús d'IA, cal `AI log` o registre equivalent
- el professorat pot demanar un microcanvi en viu sobre una peça generada
- qualsevol proposta de la IA s'ha de contrastar amb el codi real del projecte

No s'ha de delegar en la IA:

- triar el cas d'ús sense criteri del producte
- decidir l'arquitectura final sense contrast docent
- fabricar proves no executades
- justificar una persistència que l'alumnat no pot demostrar
- redactar una defensa que l'alumnat no pot sostindre oralment

## Evidències mínimes per sessió

| Sessió | Evidències mínimes |
|---|---|
| `1` | cas d'ús candidat, diagnosi del codi, mapa inicial de responsabilitats i registre d'incidències |
| `2` | cas d'ús definitiu, stack triat, pla de migració, issue principal i prova mínima abans/després |
| `3` | framework arrancable, entrada del cas d'ús migrada, demo parcial i commits de migració |
| `4` | separació visible de responsabilitats, comparativa abans/després i flux principal encara funcional |
| `5` | estructura del mòdul consolidada, justificació de rols tècnics i demo del flux complet o quasi complet |
| `6` | recurs persistent, lectura real, escriptura o actualització verificable i prova abans/després |
| `7` | registre de proves, cas positiu, cas negatiu, error controlat i incidències corregides |
| `8` | documentació tècnica, registre de decisions, deute tècnic, defensa breu i proposta de base per a `R4` |

## Checkpoints docents

- Final de sessió `1`: el cas d'ús ve de `R2` i la diagnosi és concreta.
- Final de sessió `2`: el pla de migració és viable i no planteja una reescriptura total.
- Final de sessió `3`: el framework arranca i ja conté un tram real del cas d'ús.
- Final de sessió `4`: la separació de responsabilitats és visible i funcional.
- Final de sessió `5`: les capes o equivalents són defensables i no només nominals.
- Final de sessió `6`: la persistència és real, verificable i integrada en el flux.
- Final de sessió `7`: hi ha regressió mínima amb cas positiu i negatiu.
- Final de sessió `8`: `R3` queda explicable, provat, documentat i preparat per a `R4`.

Preguntes útils de contrast:

- quin comportament de `R2` continua viu?
- quin acoblament concret s'ha reduït?
- què fa cada peça i què no hauria de fer?
- on es valida l'entrada i on es tracta l'error?
- on es llig o escriu la dada persistent?
- com es comprova que la persistència no és estat temporal?
- què queda preparat per exposar en una `API`?

## Adaptació per alumnat endarrerit

L'adaptació ha de reduir abast, no verificació.

Mesures recomanades:

- limitar `R3` a un únic cas d'ús i un únic recurs persistent
- no obrir una segona entitat si la primera no és verificable
- usar l'estructura mínima recognoscible de l'stack triat
- prioritzar una ruta o acció completa abans que diverses peces parcials
- ajornar relacions complexes, permisos avançats o proves extenses
- mantindre igualment lectura i escriptura verificables
- preparar una defensa curta centrada en què funciona, què s'ha separat i què queda pendent

Mínim no negociable:

- cas d'ús real de `R2`
- separació bàsica de responsabilitats
- persistència real
- prova reproduïble
- documentació curta però coherent
- explicació oral suficient

## Ampliació per alumnat avançat

L'ampliació ha d'aprofundir el mateix bloc, no obrir un producte paral·lel.

Possibles ampliacions:

- migrar un segon cas d'ús relacionat
- afegir una relació de dades simple i útil
- millorar validacions i tractament d'errors
- incorporar proves més sistemàtiques
- introduir patró de repositori, cas d'ús o servei d'aplicació si encaixa amb el stack
- preparar un contracte preliminar d'`API` per a `R4`
- documentar trade-offs entre dos enfocaments dins del mateix stack
- millorar observabilitat o logging si aporta valor real

Condició:

- cap ampliació pot substituir la defensa del cas d'ús principal ni relaxar la verificació de persistència.

## Riscos metodològics i mesures de control

| Risc | Mesura de control |
|---|---|
| convertir `R3` en tres planificacions diferents per framework | mantindre sessions, evidències i checkpoints comuns; tractar els frameworks com a variants de stack |
| reduir `R3` a una introducció a MVC | exigir cas d'ús real, migració funcional, persistència i regressió |
| repetir `R2` dins d'un framework | exigir diagnosi, comparativa abans/després i justificació de millora estructural |
| crear capes buides o noms correctes sense responsabilitats reals | preguntes sobre què fa i què no fa cada peça; microcanvi en viu |
| persistència decorativa o simulada | prova directa de lectura i escriptura amb comprovació abans/després |
| reescriptura massa gran i pèrdua de control | pla curt de migració, commits incrementals i regressió al final de cada canvi significatiu |
| documentació embellida però falsa | contrast entre `README`, commits, execució i defensa |
| delegació excessiva en IA | `AI log`, defensa oral, prova real i microcanvi sobre codi generat |
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
