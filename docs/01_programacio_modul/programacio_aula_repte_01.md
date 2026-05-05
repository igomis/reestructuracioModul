# Programació d'aula del Repte 1

## Finalitat del document

Este document baixa `R1` a una seqüència operativa d'aula perquè el professorat puga conduir l'arrancada del backend sense inflar el repte ni confondre infraestructura amb producte.

## Finalitat del repte

- entendre el model client/servidor aplicat al producte del curs
- assumir una base tècnica guiada sobre `Docker`, `PHP` i servidor web
- posar en marxa una base executable mínima i reproduïble
- adaptar-la al projecte propi i completar-la amb base de dades i phpMyAdmin
- deixar un primer punt d'entrada funcional del backend
- documentar i verificar la base creada
- preparar un pas net cap a `R2`

## Duració base

- `12 hores`
- `4` sessions de `3` hores
- cada sessió es correspon amb un microrepte docent concret

## Coordinació explícita entre sessions i microreptes

| Sessió | Duració | Microrepte | Focus principal | Evidència clau |
|---|---:|---|---|---|
| `1` | `3h` | Microrepte `1` | model client/servidor i elecció guiada de stack | fitxa breu d'exploració tècnica i explicació del model |
| `2` | `3h` | Microrepte `2` | base executable mínima en PHP amb Docker, adaptació i completació de l'entorn | projecte arrancant, BBDD i phpMyAdmin incorporats, `README` inicial i decisió/incidència |
| `3` | `3h` | Microrepte `3` | primer punt d'entrada funcional del backend | ruta, vista, endpoint o `healthcheck` funcional |
| `4` | `3h` | Microrepte `4` | documentació tècnica, verificació i checkpoint | README executable, verificació i pas cap a `R2` |

## Seqüència recomanada de sessions

### Sessió 1. Microrepte 1

# Sessió 1 — Model client/servidor i elecció guiada de stack

## Objectiu

Situar el curs, explicar el paper del servidor i acotar la base tècnica del repte.

## Què explica el professorat

- projecte únic del curs
- diferència client/servidor
- què fa el backend
- per què R1 encara no és un repte de framework complet

## Què modela el professorat

- lectura curta del briefing inicial
- mapa bàsic client/servidor
- ús de la fitxa breu d'exploració tècnica inicial
- exemple molt breu de decisió tècnica orientativa

## Què fa l'alumnat

- concreta el producte
- ompli la fitxa breu d'exploració tècnica inicial
- identifica tecnologies de client i servidor
- explora de manera breu possibles stacks o frameworks amb ajuda d'IA si convé
- deixa una primera decisió tècnica visible amb dubtes oberts

## Producte final de la sessió

Fitxa breu d'exploració tècnica inicial, tancada al final de la sessió o entre la sessió 1 i la 2, i usada com a evidència del microrepte 1.

## Evidència esperada

- fitxa breu entregada
- primera decisió tècnica orientativa
- explicació del model client/servidor

## Checkpoint

Cada alumne pot explicar:

- quin paper jugarà el servidor en el seu producte
- quines tecnologies ha identificat
- amb què començaria
- quins dubtes tècnics manté oberts

## Seqüència temporal de la sessió (3 hores)

### 0:00–0:25 — Obertura i marc del curs

- presentació del projecte únic del curs
- sentit de R1 com a repte d'arrencada, comprensió tècnica i acotació
- pregunta central: què haurà de fer el servidor en el teu producte?

### 0:25–0:50 — Model client/servidor

- diferència entre client, servidor i base de dades
- recorregut bàsic petició-resposta
- exemples simples: login, consulta de llista, enviament de formulari
- aclariment: en esta fase importa entendre responsabilitats, no dominar encara un framework

### 0:50–1:10 — Modelatge de la fitxa breu

- presentació de la fitxa breu d'exploració tècnica inicial
- exemple molt curt omplit en directe
- mostra d'una decisió tècnica orientativa provisional

### 1:10–1:55 — Exploració guiada

- l'alumnat concreta el producte
- ompli la fitxa
- identifica tecnologies de client i servidor
- compara 1 o 2 opcions de stack o framework
- pot usar IA per aclarir conceptes o comparar opcions
- deixa una primera decisió orientativa i dubtes oberts

### 1:55–2:20 — Posada en comú i contrast tècnic

- 3 o 4 exemples ràpids d'alumnes
- contrast entre opcions
- aclariments sobre backend, persistència, autenticació i punt de partida tècnic

### 2:20–2:45 — Ajust final de la fitxa

- revisió de la fitxa després del contrast
- millor redacció de la decisió orientativa
- concreció de dubtes tècnics oberts
- preparació de l'entrega

### 2:45–3:00 — Checkpoint final

- comprovació oral breu o revisió ràpida
- entrega de la fitxa al final o entre la sessió 1 i la 2

## Exemple molt breu de decisió tècnica orientativa

> Començaria amb un client web senzill en HTML/CSS/JS i un servidor en PHP perquè en esta fase em permet entendre millor el flux petició-resposta, el tractament de formularis i la lògica del backend sense afegir encara massa abstracció. El servidor haurà de validar dades, gestionar informació i guardar-la en base de dades. Com a dubtes oberts, encara no tinc clar si més avant em convindrà continuar amb PHP directe o passar a un framework per a ordenar millor la part MVC i la persistència.

## Paper de la IA en esta sessió

Ús acceptable:

- aclarir diferències entre tecnologies
- comparar 2 opcions de stack
- reformular dubtes tècnics
- resumir pros i contres

No acceptable:

- pegar una decisió tècnica prefabricada sense entendre-la
- entregar una fitxa generada per IA sense contrast personal

# Sessió 2 — Backend mínim en PHP amb Docker i completació de l’entorn

## Objectiu

Passar de la comprensió inicial del backend a una base executable real del repte, deixant un entorn mínim en PHP amb Docker i servidor web, i completant-lo amb base de dades i phpMyAdmin.

## Què explica el professorat

- què és una base executable mínima
- per què no es dona l’entorn complet tancat
- quines peces hi ha en l’entorn:
    - projecte
    - servidor web
    - PHP
    - Docker
    - base de dades
    - phpMyAdmin
- què vol dir que l’entorn “funciona”
- què s’espera del microrepte 2

## Què modela el professorat

- un backend mínim en PHP amb Docker i servidor web
- una estructura mínima del projecte
- una arrencada bàsica
- una comprovació simple al navegador
- un README mínim
- deixa expressament oberta la completació de l’entorn amb base de dades i phpMyAdmin

## Què fa l’alumnat

- parteix del model mínim mostrat pel professorat
- l’adapta al seu projecte
- decideix elements mínims propis:
    - nom/identitat del projecte
    - estructura mínima
    - port o ajust simple
    - resposta inicial personalitzada
- completa l’entorn afegint:
    - servei de base de dades
    - servei de phpMyAdmin
- prova l’arrancada
- comprova que els serveis funcionen
- escriu un README curt
- registra una incidència, dubte o decisió tècnica

## Producte final de la sessió

- estructura mínima del projecte
- entorn executable bàsic
- serveis de BBDD i phpMyAdmin incorporats
- resposta inicial funcional
- README curt d’arrancada
- nota breu de decisió tècnica o incidència

## Evidència esperada

- `docker-compose.yml` o equivalent adaptat
- serveis mínims definits i arrancables
- comprovació de funcionament
- README executable
- justificació curta d’una decisió tècnica
- incidència detectada o resolta

## Checkpoint

Cada alumne ha de poder explicar:

- quins serveis té el seu entorn
- què fa cada peça
- què ha adaptat respecte del model del professorat
- com comprova que funciona
- quina decisió tècnica ha pres
- quina incidència o dubte ha trobat

## Seqüència temporal de la sessió (3 hores)

### 0:00–0:20 — Marc i modelatge inicial

- recuperació del sentit del microrepte 2
- explicació curta del backend mínim executable
- presentació de les peces de l’entorn
- idea clau: el professorat modela una base mínima, l’alumnat l’adapta i la completa

### 0:20–0:50 — Demostració guiada del professorat

- estructura mínima del projecte
- Docker + PHP + servidor web
- arrencada bàsica
- comprovació simple
- README mínim
- indicació explícita del que queda perquè l’alumnat ho complete

### 0:50–2:10 — Treball de l’alumnat

- adaptació del model al projecte propi
- incorporació de BBDD i phpMyAdmin
- arrencada i comprovació
- registre d’incidències
- redacció del README

### 2:10–2:35 — Posada en comú i desbloqueig

- revisió d’errors habituals
- contrast entre decisions
- aclariment de bloquejos tècnics
- ajust de l’entorn

### 2:35–3:00 — Checkpoint final

- comprovació ràpida de funcionament
- explicació oral breu
- revisió del README
- tancament del microrepte o preparació de continuació

## Paper de la IA en esta sessió

Ús acceptable:

- interpretar errors de configuració
- comparar opcions mínimes d’entorn
- aclarir el paper de cada servei
- suggerir un README curt
- ajudar a entendre un bloqueig concret

No acceptable:

- copiar una configuració completa sense entendre-la
- pegar una solució sencera no validada
- donar per funcional un entorn que no es pot explicar ni reproduir

## Continuació de la seqüència recomanada

### Sessió 3. Microrepte 3

**Primer punt d'entrada funcional del backend**

- Objectiu: deixar una primera resposta funcional del backend que done sentit al producte.
- Què explica el professorat: què diferencia un punt d'entrada útil d'un esquelet buit i quin és el mínim funcional no trivial de `R1`.
- Què modela el professorat: una ruta, vista, endpoint o `healthcheck` servit pel backend i connectat amb el domini del producte.
- Què fa l'alumnat: implementa el primer punt d'entrada funcional i el prova en execució real.
- Evidència esperada: resposta visible del sistema, prova curta del comportament i coherència amb el producte triat.
- Checkpoint: el backend ja fa alguna cosa real i explicable, encara que simple.

### Sessió 4. Microrepte 4

**Documentació tècnica, verificació i checkpoint**

- Objectiu: tancar `R1` amb documentació usable, verificació real i un pas clar cap a `R2`.
- Què explica el professorat: què es comprovarà al checkpoint `R1 -> R2`, què ha de tindre el `README`, què s'ha de poder defendre i què encara no cal resoldre en este repte.
- Què modela el professorat: execució del projecte seguint el `README`, revisió d'evidències i defensa tècnica breu.
- Què fa l'alumnat: polix documentació, registra comprovacions, prepara la demo curta i deixa clar quin flux es protegirà després en `R2`.
- Evidència esperada: `README` executable, justificació tècnica breu, verificació del punt d'entrada funcional i pas justificat cap a `R2`.
- Checkpoint: l'alumnat pot defensar el producte arrancat, el punt d'entrada i la base tècnica sense dependre d'una demo memoritzada.

## Evidències esperades per sessió

- Sessió `1`: fitxa breu d'exploració tècnica inicial, explicació client/servidor i decisió tècnica orientativa.
- Sessió `2`: base executable amb `Docker`, `PHP`, servidor web, BBDD, phpMyAdmin, `README` inicial, decisió tècnica i incidència o dubte registrat.
- Sessió `3`: punt d'entrada funcional del backend en execució real.
- Sessió `4`: documentació, verificació i checkpoint de pas a `R2`.

## Moments de checkpoint

- Checkpoint curt `1`: al final de la sessió `1` o a l'inici de la sessió `2`, per validar que hi ha criteri tècnic i no només intuïció.
- Checkpoint curt `2`: al final de la sessió `2`, per comprovar que el projecte arranca de veritat, que els serveis mínims estan definits i que l'alumnat pot explicar què ha adaptat i completat.
- Checkpoint curt `3`: al final de la sessió `3`, per confirmar que existix un punt d'entrada funcional.
- Checkpoint de pas `R1 -> R2`: al final de la sessió `4`, per decidir si el grup entra a `R2` sobre una base real.

## Preparació del tancament del repte

- demanar una demo curta de l'arrancada del projecte
- revisar que el `README` permeta posar el projecte en marxa
- exigir una explicació clara de la relació client/servidor i del paper de cada component tècnic
- comprovar que el punt d'entrada funcional és reproduïble i no decoratiu
- demanar quina operació del domini serà la primera funcionalitat protegida de `R2`
- comprovar que l'ús de la IA, si ha existit, es pot explicar i verificar

## Criteri pràctic de tancament

`R1` queda preparat quan el professorat pot veure una decisió tècnica guiada, una base executable adaptada i completada, un primer punt d'entrada funcional del backend i una documentació suficient per continuar cap a `R2` sense tornar a començar.
