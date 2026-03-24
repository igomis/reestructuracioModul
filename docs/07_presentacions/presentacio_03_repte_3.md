# Presentació 03. Repte 3

Micro-presentació docent breu. Equival aproximadament a `8` diapositives.

## Diapositiva 1. Idea central
- `R3` és el pas de “funciona” a “es pot mantindre”
- el repte professionalitza el producte
- arquitectura i persistència només tenen valor sobre un cas d'ús real

## Diapositiva 2. Què resol el repte
- separació de responsabilitats
- persistència segura i coherent
- validacions i errors més robustos
- primera base real per publicar `API`

## Diapositiva 3. Què no és suficient
- moure fitxers i carpetes
- capes decoratives
- connectar BD sense flux persistent complet
- reescriure el projecte i perdre el que ja funcionava

## Diapositiva 4. Què modela el professorat
- una refactorització curta i explicable
- una entitat persistent amb cas d'ús complet
- una comprovació de regressió
- una decisió tècnica sobre capes o equivalent

## Diapositiva 5. Què construeix l'alumnat
- estructura MVC o equivalent aplicada de veritat
- cas d'ús real refactoritzat
- model persistent del domini
- proves mínimes i documentació actualitzada

## Diapositiva 6. Evidència mínima
- commits de migració incremental
- cas d'ús verificat amb persistència real
- proves o comprovacions registrades
- `README` i decisions tècniques al dia

## Diapositiva 7. Errors habituals
- fer neteja cosmètica i dir-li arquitectura
- no provar regressions
- persistència aparent però fràgil
- crear massa capes sense necessitat

## Diapositiva 8. Connexió amb `R4`
- si `R3` queda sòlid, `R4` pot publicar una `API` real
- si `R3` queda feble, `R4` només exposarà rutes damunt d'una base inestable
- `R4` hereta directament la qualitat d'este repte
