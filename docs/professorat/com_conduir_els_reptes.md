# Com conduir els reptes

## Seqüència docent `R1-R5`

La seqüència no és una llista de tecnologies. Cada repte resol un pas real del producte i deixa preparada l'entrada al següent.

## `R1`. Arrancada funcional del producte

### Què resol

Obrir el projecte amb domini triat, repositori usable, `README` mínim i una primera interacció funcional del producte.

### Què modela el professorat

- criteri de kickoff funcional, no d'esquelet buit
- primer flux d'entrada amb validació i registre mínim
- traçabilitat inicial de repositori, `README` i decisions tècniques

### Què no és suficient

- triar stack sense cas d'ús visible
- tindre només rutes de prova o plantilla estàtica
- infraestructura sense dada validada o registrada

### Pas a `R2`

Només convé passar a `R2` si ja hi ha una acció real del producte sobre la qual puga tindre sentit protegir accés o estat.

## `R2`. Primera funcionalitat de negoci protegida

### Què resol

Convertir auth o estat equivalent en infraestructura al servei d'una operació de negoci real.

### Què modela el professorat

- alta, login o estat equivalent amb sentit de producte
- primera operació protegida
- cas correcte, cas denegat i error mínim controlat

### Què no és suficient

- formularis d'auth sense cap acció del domini
- ruta protegida decorativa
- funcionalitat aparent sense prova reproduïble

### Pas a `R3`

`R3` només té sentit si `R2` deixa un flux real que mereix ser refactoritzat i persistit.

## `R3`. Arquitectura i persistència del flux principal

### Què resol

Fer més mantenible i persistent una funcionalitat que ja està viva.

### Què modela el professorat

- refactorització curta amb millora recognoscible
- primera entitat persistent
- comprovació de regressió sobre el flux principal

### Què no és suficient

- reorganitzar carpetes sense millorar el producte
- afegir base de dades sense integrar-la al cas d'ús
- parlar d'arquitectura sense prova del flux després del canvi

### Pas a `R4`

`R4` s'obri quan la persistència és prou estable i l'arquitectura és explicable sense improvisació.

## `R4`. Publicació i consum d'`API`

### Què resol

Convertir una part rellevant del producte en `API` usable, provada i documentada.

### Què modela el professorat

- contracte mínim d'`API`
- endpoint nuclear amb cas correcte i cas d'error
- prova reproduïble i consum mínim

### Què no és suficient

- obrir endpoints sense cas d'ús publicat
- retornar JSON sense coherència de contracte
- documentació que no coincidix amb el comportament real

### Pas a `R5`

Només convé obrir `R5` si l'`API` ja és consumible i queda una base sòlida per a una integració útil.

## `R5`. Integració híbrida i tancament defensable

### Què resol

Tancar el producte amb una integració o automatització que aporte valor real i preparar la defensa individual.

### Què modela el professorat

- decisió d'integració a partir d'una necessitat del producte
- workflow curt de punta a punta
- prova completa, incidència mínima i defensa tècnica

### Què no és suficient

- fer servir `n8n` o una eina externa sense necessitat funcional
- workflow decoratiu o només aparent
- arribar a defensa sense prova completa ni traçabilitat

### Connexió de tancament

`R5` no obri un bloc nou. Tanca el producte, la documentació i la defensa dins de les dues primeres avaluacions.

## Regla de pas entre reptes

- no s'avança només per calendari
- cada repte ha de deixar una evidència mínima reproduïble
- el professorat modela fluxos curts i verificables, no solucions enormes
- el punt crític no és la quantitat de codi, sinó si el producte es pot explicar, provar i defensar
