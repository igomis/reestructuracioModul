# MT08. Migracions, seeders i dades de prova

Micro-presentació docent breu per a `R3S2`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- la base de dades ha de poder reconstruir-se
- les dades de prova no són decoració
- un flux sense dades realistes no es pot defensar bé

## Diapositiva 2. Migracions

- defineixen estructura
- documenten evolució
- permeten entorns repetibles
- eviten bases de dades artesanals
- han de reflectir el model del domini

## Diapositiva 3. Seeders o fixtures

- creen dades mínimes
- permeten provar rols i estats
- fan reproduïble la demo
- eviten dependència de dades manuals
- han de tindre sentit de negoci

## Diapositiva 4. Dades útils

- almenys dos usuaris o rols
- recursos en estats diferents
- un cas correcte
- un cas conflictiu
- un cas denegat

## Diapositiva 5. Evidència del dia

- migracions executades de zero
- dades inicials carregades
- flux provat amb eixes dades
- instrucció en README
- commit verificable

## Diapositiva 6. Tancament

- si només funciona amb la teua base local, encara no és reproduïble
- les dades de prova també conten una història del producte
- pregunta final: pots esborrar i reconstruir la base sense perdre el flux?
