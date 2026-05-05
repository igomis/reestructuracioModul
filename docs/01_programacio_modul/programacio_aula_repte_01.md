# Programació d'aula del Repte 1

## Finalitat del document

Este document baixa `R1` a una seqüència operativa d'aula perquè el professorat puga conduir l'arrancada del backend sense inflar el repte ni confondre infraestructura amb producte.

## Finalitat del repte

- entendre el model client/servidor aplicat al producte del curs
- distingir els models d'execució de codi en client web i servidor
- assumir una base tècnica guiada sobre `Docker`, `PHP` i servidor web
- posar en marxa una base executable mínima i reproduïble
- adaptar-la al projecte propi i completar-la amb base de dades i phpMyAdmin
- deixar un primer punt d'entrada funcional del backend
- documentar i verificar la base creada
- preparar un pas net cap a `R2`

## Relació entre microreptes i sessions

El Repte 1 manté `4` microreptes com a unitats de progrés:

- `Microrepte 1`: model client/servidor, model d'execució client vs servidor i decisió tècnica inicial
- `Microrepte 2`: entorn executable
- `Microrepte 3`: primer punt d'entrada funcional
- `Microrepte 4`: documentació, verificació i checkpoint

Estos microreptes no equivalen necessàriament a `4` sessions. En esta programació d'aula, els `4` passos lògics del repte es compacten en `2` sessions principals de treball i una tercera sessió opcional de defensa o checkpoint formal.

## Duració base

- `6 hores` de treball principal
- `2` sessions de `3` hores
- `1` sessió opcional de `3` hores si cal defensa, checkpoint formal o revisió forta d'evidències

## Coordinació explícita entre sessions i microreptes

| Sessió | Duració | Microreptes implicats | Focus principal | Evidència clau |
|---|---:|---|---|---|
| `1` | `3h` | `MP1` + inici de `MP2` | model client/servidor, model d'execució, decisió inicial i arrencada de l'entorn | fitxa inicial, explicació client vs servidor, decisió tècnica i base mínima començada |
| `2` | `3h` | tancament de `MP2` + `MP3` + `MP4` | entorn complet, primera funcionalitat mínima i documentació del repte | entorn arrancable, punt d'entrada funcional, README i documentació en repositori |
| `3` | opcional | checkpoint formal | defensa, execució real i revisió de traçabilitat | defensa tècnica o acta de checkpoint |

## Sessió 1 — Model client/servidor, decisió inicial i arrencada de l’entorn

### Objectiu

Treballar el `Microrepte 1` i iniciar el `Microrepte 2`, deixant clara la base conceptual del backend, distingint els models d’execució de codi en client i servidor, i començant el muntatge de l’entorn executable.

### Què explica el professorat

- model client/servidor
- què s'executa al client web i què s'executa al servidor
- paper del backend i del servidor web
- per què el Repte 1 encara no és un repte de framework complet
- què és una base tècnica inicial útil
- què és un entorn executable mínim

### Què modela el professorat

- lectura curta del briefing inicial
- esquema client/servidor
- fitxa breu d’exploració tècnica inicial
- exemple breu de decisió tècnica orientativa
- demostració inicial d’un entorn mínim amb PHP + Docker + servidor web

### Què fa l’alumnat

- concreta el producte
- ompli la fitxa inicial
- identifica tecnologies de client i servidor
- diferencia quina part del producte s'executarà al client i quina al servidor
- deixa una primera decisió tècnica visible
- inicia l’entorn executable
- comença a adaptar el model mostrat pel professorat al seu projecte

### Producte final de la sessió

- fitxa tècnica inicial
- primera decisió orientativa
- base mínima de projecte
- inici d’entorn executable

### Evidència esperada

- fitxa entregada
- explicació breu del model d'execució client vs servidor aplicada al producte propi
- decisió tècnica inicial
- estructura mínima del projecte
- primeres proves d’arrancada de l’entorn

### Seqüència temporal de la sessió (3 hores)

- `0:00–0:20` marc del repte i model client/servidor
- `0:20–0:45` fitxa d’exploració i decisió inicial
- `0:45–1:15` modelatge inicial de l’entorn executable
- `1:15–2:30` treball de l’alumnat sobre el seu projecte
- `2:30–3:00` posada en comú, ajustos i checkpoint curt

### Checkpoint

Cada alumne ha de poder explicar:

- quin paper jugarà el backend en el seu producte
- quina part del seu producte s'executa al client i quina al servidor
- amb quina base tècnica començarà
- què ha arribat a muntar de l’entorn
- quins dubtes manté oberts

## Sessió 2 — Tancament de l’entorn, primera funcionalitat mínima i documentació del repte

### Objectiu

Tancar el `Microrepte 2` i resoldre el `Microrepte 3` i el `Microrepte 4` en una mateixa sessió: entorn complet, primera funcionalitat mínima, documentació i preparació del checkpoint.

### Què explica el professorat

- criteri de “funciona de veritat”
- què diferencia un esquelet buit d’una primera funcionalitat mínima
- què s’espera del README i de la documentació del repte
- quines evidències fan falta per al checkpoint

### Què modela el professorat

- tancament de l’entorn mínim
- incorporació de BBDD i phpMyAdmin si no havien quedat tancats
- exemple molt curt d’un primer punt d’entrada funcional
- exemple de README executable i documentació mínima útil
- organització d’un directori de documentació dins del repositori
- exemple d’una pàgina o índex que enllace la documentació

### Què fa l’alumnat

- acaba l’entorn executable
- incorpora BBDD i phpMyAdmin si cal
- crea una primera pàgina o punt d’entrada funcional del backend
- documenta com s’arranca i com es comprova
- crea un directori de documentació al repositori
- penja les fitxes o documents del repte dins del repositori
- crea un índex o pàgina que enllace eixa documentació
- prepara el checkpoint final del Repte 1

### Producte final de la sessió

- entorn executable complet
- primer punt d’entrada funcional
- README executable
- directori de documentació dins del repositori
- fitxes del repte penjades i enllaçades
- repte preparat per al checkpoint

### Evidència esperada

- `docker-compose.yml` o equivalent funcional
- entorn que arranca
- primera funcionalitat mínima del backend
- README clar
- documentació del repte organitzada en repositori
- enllaç o pàgina índex de documentació
- justificació tècnica curta
- traçabilitat mínima amb commits i, si toca, AI log

### Seqüència temporal de la sessió (3 hores)

- `0:00–0:20` repàs i tancament del que faltava de l’entorn
- `0:20–0:50` modelatge del primer punt d’entrada funcional i de la documentació mínima
- `0:50–2:10` treball de l’alumnat: entorn + primera funcionalitat + documentació
- `2:10–2:35` revisió d’errors habituals i desbloqueig
- `2:35–3:00` checkpoint final del Repte 1 o preparació de defensa

### Checkpoint

Cada alumne ha de poder explicar:

- com s’arranca el projecte
- què fa cada peça important de l’entorn
- quina és la primera funcionalitat mínima real
- on està la documentació del repte
- què ha decidit i què queda encara pendent

## Sessió 3 opcional — Defensa / checkpoint formal

Esta sessió només s’activa si el professorat considera necessari separar del treball tècnic una revisió formal de tancament. Pot servir per a:

- defensa tècnica
- execució real seguint README
- revisió de traçabilitat
- contrast de comprensió o microcanvis en viu

No substituïx el treball de les sessions `1` i `2`; només dona temps específic per acreditar millor el que ja hauria d’estar preparat.

## Evidències globals del Repte 1

- fitxa breu d’exploració tècnica inicial
- explicació del model d'execució client vs servidor aplicat al producte
- decisió tècnica inicial
- repositori usable
- historial de commits significatiu
- entorn executable amb `Docker`, `PHP`, servidor web, BBDD i phpMyAdmin
- README executable
- primer punt d’entrada funcional del backend
- directori de documentació dins del repositori
- fitxes o documents del repte penjats al repositori
- índex o pàgina visible que enllaça la documentació
- justificació tècnica breu
- AI log quan hi haja ús rellevant d’IA
- defensa tècnica breu o checkpoint quan corresponga

## Criteri pràctic de tancament

`R1` queda preparat quan el professorat pot veure una decisió tècnica guiada, una base executable adaptada i completada, un primer punt d'entrada funcional del backend i una documentació dins del repositori suficient per revisar el procés i continuar cap a `R2` sense tornar a començar.
