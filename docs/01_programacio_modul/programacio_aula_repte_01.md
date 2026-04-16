# Programació d'aula del Repte 1

## Finalitat del document

Este document baixa `R1` a una seqüència curta i operativa d'aula perquè el professorat puga conduir l'arrancada del backend sense improvisar i sense confondre arrencada tècnica amb producte real.

## Finalitat del repte

- obrir el projecte del curs amb un producte recognoscible
- assumir la base comuna en `PHP` com a punt de partida compartit
- posar en marxa un entorn executable de veritat
- deixar un primer punt d'entrada funcional del producte
- validar una primera entrada de dades amb resposta recognoscible
- preparar un pas net cap a `R2`

## Duració orientativa

- `4` setmanes o `6-8` sessions d'entre `50` i `120` minuts
- si el centre treballa amb menys hores, es poden fusionar les sessions `1-2` i `5-6`
- si el grup arriba just, no s'obri un segon flux: es tanca només el primer

## Seqüència recomanada de sessions

### Sessió 1. Obrir el curs i el producte

- Objectiu: situar el curs en clau de producte únic, reptes i treball verificable.
- Què explica el professorat: model client/servidor, projecte únic del curs, evidències, paper del `README` i ús acceptable de la IA.
- Què modela el professorat: lectura curta del briefing inicial, estructura mínima d'un repositori usable i exemple molt breu de `README`.
- Què fa l'alumnat: tria projecte base, obri repositori i deixa per escrit què vol posar en marxa.
- Evidència esperada: repositori creat, `README` inicial i decisió provisional de projecte.
- Checkpoint: cada alumne pot explicar quin producte comença i què haurà de fer el servidor dins d'eixe producte.

### Sessió 2. Entorn executable i decisió tècnica

- Objectiu: passar del plantejament general a una base tècnica real que arranca.
- Què explica el professorat: per què `R1` encara no és un repte de framework complet, què vol dir base comuna en `PHP` i què es considera entorn executable.
- Què modela el professorat: arrencada local del projecte, punt d'entrada mínim i actualització del `README` amb instruccions d'ús.
- Què fa l'alumnat: prepara entorn, confirma base comuna i deixa una decisió tècnica curta i defensable.
- Evidència esperada: projecte arrancant localment, estructura recognoscible i instruccions d'arrancada.
- Checkpoint: el projecte es pot posar en marxa davant del professorat sense explicacions improvisades.

### Sessió 3. Primera entrada funcional del producte

- Objectiu: deixar una pantalla inicial o equivalent que ja tinga sentit dins del domini.
- Què explica el professorat: què diferencia una pantalla útil d'una maqueta i quin és el mínim funcional no trivial del repte.
- Què modela el professorat: una ruta o punt d'entrada real servit pel backend i una pantalla inicial coherent amb el producte.
- Què fa l'alumnat: implementa la primera peça funcional visible i la connecta amb el cas d'ús d'entrada.
- Evidència esperada: pantalla inicial funcional, flux d'entrada recognoscible i coherència amb el producte triat.
- Checkpoint: el que es veu en pantalla ja deixa entendre què podrà fer el producte.

### Sessió 4. Recepció de dades i validació mínima

- Objectiu: fer que el servidor reba una primera dada real i no només mostre una interfície.
- Què explica el professorat: entrada, tractament, validació mínima i diferència entre cas correcte i cas incorrecte.
- Què modela el professorat: recepció d'una dada simple, comprovació d'un camp obligatori i resposta bàsica en els dos casos.
- Què fa l'alumnat: implementa un formulari o entrada equivalent, tracta la dada i mostra almenys un error visible.
- Evidència esperada: cas correcte i incorrecte reproduïbles.
- Checkpoint: el backend ja no sols renderitza, sinó que tracta dades amb criteri bàsic.

### Sessió 5. Primer registre o persistència bàsica

- Objectiu: deixar rastre útil de la primera dada correcta del domini.
- Què explica el professorat: què és un registre funcional suficient en `R1` i per què encara no cal obrir persistència avançada ni arquitectura pesada.
- Què modela el professorat: guardat molt simple de la dada principal i lectura del rastre deixat.
- Què fa l'alumnat: guarda o registra la dada correcta de manera mínima i actualitza el `README` amb com provar-ho.
- Evidència esperada: dada correcta registrada o persistida de manera bàsica.
- Checkpoint: el producte ja deixa un rastre útil que podrà aprofitar-se després.

### Sessió 6. Tancament del repte i pas net a `R2`

- Objectiu: revisar que `R1` queda prou sòlid per obrir autenticació o estat sense base falsa.
- Què explica el professorat: què es comprovarà al checkpoint `R1 -> R2`, què no convé obrir encara i què s'ha de poder defendre.
- Què modela el professorat: demostració curta del flux complet i lectura final del `README` i de la traçabilitat mínima.
- Què fa l'alumnat: prepara demo curta, corregeix punts febles i deixa clar quin flux serà protegit a `R2`.
- Evidència esperada: repositori usable, `README` clar, flux correcte i incorrecte, registre bàsic i pas justificat cap a `R2`.
- Checkpoint: l'alumnat pot defensar el flux complet sense dependre d'una demo memoritzada.

## Evidències esperades per trams

- Tram d'arrancada: repositori, `README`, projecte base triat i entorn executable.
- Tram funcional: primera entrada del producte, recepció de dades i validació mínima.
- Tram de tancament: cas correcte, cas incorrecte, registre o persistència bàsica i explicació del pas a `R2`.

## Moments de checkpoint

- Checkpoint curt `1`: al final de la sessió `2`, per validar que hi ha projecte i entorn, no només intenció.
- Checkpoint curt `2`: al final de la sessió `4`, per comprovar que el backend ja tracta dades i mostra errors.
- Checkpoint de pas `R1 -> R2`: al final de la sessió `6`, per decidir si el grup pot entrar en auth o estat sobre una base funcional real.

## Preparació del tancament del repte

- demanar una demo curta del flux principal sense ajuda del professorat
- revisar que el `README` permeta arrancar el projecte i provar-lo
- exigir una explicació clara de què es valida i de què es registra
- demanar quina operació del domini serà la primera funcionalitat protegida de `R2`
- comprovar que l'ús de la IA, si ha existit, es pot explicar i verificar

## Criteri pràctic de tancament

`R1` queda preparat quan el professorat pot veure una primera entrada real al producte, una dada tractada pel servidor, un error visible, un rastre bàsic de la informació correcta i una traçabilitat mínima que permeta continuar cap a `R2` sense tornar a començar.
