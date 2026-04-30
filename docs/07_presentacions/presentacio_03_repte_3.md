# Presentació 03. Repte 3

Micro-presentació docent breu. Equival aproximadament a `8` diapositives.

## Diapositiva 1. Idea central

- `R3` és reconstruir el projecte en framework
- base operativa real, persistència mínima real i fluxos verificables
- no es demana migrar tota l'aplicació de `R2`

## Diapositiva 2. Què resol el repte

- Docker i projecte arrancable
- rutes, controladors, vistes o respostes i models o equivalents
- BBDD real amb `migrations` i `seeders`
- `2` casos d'ús end-to-end

## Diapositiva 3. Què no és suficient

- moure fitxers al framework
- quedar-se en l'esquelet
- connectar BBDD sense dades reproduïbles
- fer només un flux o un segon flux cosmètic

## Diapositiva 4. Què modela el professorat

- arrencada del framework amb Docker
- migració, seeder o equivalent
- recorregut ruta, controlador, model o servei i resposta
- prova d'un cas positiu i d'un error

## Diapositiva 5. Què construeix l'alumnat

- base en framework operativa
- primer flux migrat de `R2`
- segon flux migrat o ampliació funcional útil
- validació, errors, proves i README

## Diapositiva 6. Evidència mínima

- Docker funcional i `.env` documentat
- BBDD creada amb `migrations`
- dades inicials amb `seeders` o equivalent
- demo dels `2` fluxos
- backlog del que queda per migrar

## Diapositiva 7. Errors habituals

- confondre migrar amb copiar fitxers
- no poder reconstruir la BBDD
- usar dades estàtiques
- no saber quin flux ve de `R2`
- no provar errors

## Diapositiva 8. Connexió amb `R4`

- si `R3` queda sòlid, `R4` pot publicar una `API` real
- si `R3` queda feble, `R4` només exposarà rutes damunt d'una base inestable
- `R4` hereta directament la qualitat de la base en framework
