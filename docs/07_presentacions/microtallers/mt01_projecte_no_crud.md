# MT01. Projecte no CRUD

Micro-presentació docent breu per a `R1S1`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- un projecte backend no és una taula amb botons
- ha de tindre actors, regles i fluxos
- el domini ha de sobreviure fins a `R5`

## Diapositiva 2. Senyals d'un CRUD pobre

- només alta, edició, llistat i esborrat
- no hi ha estats ni decisions
- no hi ha rols reals
- no hi ha cap error interessant
- no es veu per què cal auth, API o integració

## Diapositiva 3. Senyals d'un projecte viable

- hi ha una operació de negoci recognoscible
- hi ha restriccions i casos denegats
- hi ha dades que canvien d'estat
- hi ha traçabilitat
- hi ha una integració futura plausible

## Diapositiva 4. Preguntes de selecció

- qui usa el sistema?
- què pot fer cada actor?
- què no hauria de poder fer?
- quina decisió pren el backend?
- quin flux podràs defensar en `R5`?

## Diapositiva 5. Evidència del dia

- descripció curta del domini
- actors principals
- primer flux funcional
- dues regles de negoci
- un error o restricció
- primeres issues o tasques

## Diapositiva 6. Tancament

- si el projecte no té conflictes, estats o restriccions, cal replantejar-lo
- el repte no premia idees grans, premia productes defensables
- pregunta final: què farà el teu backend que no siga només guardar files?
