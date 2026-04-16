# Programació d'aula del Repte 1

## Finalitat del document

Este document baixa `R1` a una seqüència operativa d'aula perquè el professorat puga conduir l'arrancada del backend sense inflar el repte ni confondre infraestructura amb producte.

## Finalitat del repte

- entendre el model client/servidor aplicat al producte del curs
- assumir una base tècnica guiada sobre `Docker`, `PHP` i servidor web
- posar en marxa un entorn executable i reproduïble
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
| `1` | `3h` | Microrepte `1` | model client/servidor i elecció guiada de stack | decisió tècnica inicial i explicació del model |
| `2` | `3h` | Microrepte `2` | entorn executable amb Docker, PHP i servidor web | projecte arrancant i `README` inicial |
| `3` | `3h` | Microrepte `3` | primer punt d'entrada funcional del backend | ruta, vista, endpoint o `healthcheck` funcional |
| `4` | `3h` | Microrepte `4` | documentació tècnica, verificació i checkpoint | README executable, verificació i pas cap a `R2` |

## Seqüència recomanada de sessions

### Sessió 1. Microrepte 1

**Model client/servidor i elecció guiada de stack**

- Objectiu: situar el curs, explicar el paper del servidor i acotar la base tècnica del repte.
- Què explica el professorat: projecte únic del curs, diferència client/servidor, què fa el backend i per què `R1` encara no és un repte de framework complet.
- Què modela el professorat: lectura curta del briefing inicial, mapa bàsic client/servidor i exemple molt breu de decisió tècnica registrada.
- Què fa l'alumnat: concreta el producte, justifica el stack base dins del marc docent i deixa una primera decisió tècnica visible.
- Evidència esperada: comparativa o justificació breu, producte triat i primera nota tècnica o `ADR` curt.
- Checkpoint: cada alumne pot explicar quin paper jugarà el servidor en el seu producte i per què la base triada és assumible.

### Sessió 2. Microrepte 2

**Entorn executable amb Docker, PHP i servidor web**

- Objectiu: convertir la decisió tècnica en un entorn real que arranca.
- Què explica el professorat: què posa en marxa `Docker`, quin paper té `PHP`, quin paper té el servidor web i què compta com a entorn executable.
- Què modela el professorat: arrencada local del projecte, comprovació d'un contenidor o servei, punt d'entrada mínim i actualització del `README` amb instruccions reals.
- Què fa l'alumnat: prepara el repositori, configura l'entorn, comprova que el projecte arranca i deixa documentats els passos d'arrancada.
- Evidència esperada: projecte arrancant, estructura recognoscible, `README` inicial i traçabilitat mínima amb issues o commits.
- Checkpoint: una altra persona pot seguir el `README` i entendre què s'ha d'aixecar.

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

- Sessió `1`: explicació client/servidor i decisió tècnica inicial.
- Sessió `2`: entorn executable amb `Docker`, `PHP`, servidor web i `README` inicial.
- Sessió `3`: punt d'entrada funcional del backend en execució real.
- Sessió `4`: documentació, verificació i checkpoint de pas a `R2`.

## Moments de checkpoint

- Checkpoint curt `1`: al final de la sessió `1`, per validar que hi ha criteri tècnic i no només intuïció.
- Checkpoint curt `2`: al final de la sessió `2`, per comprovar que el projecte arranca de veritat.
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

`R1` queda preparat quan el professorat pot veure una decisió tècnica guiada, un entorn executable, un primer punt d'entrada funcional del backend i una documentació suficient per continuar cap a `R2` sense tornar a començar.
