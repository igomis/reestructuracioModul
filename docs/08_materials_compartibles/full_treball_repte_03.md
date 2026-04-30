# Full de treball del Repte 3

## Objectiu

Reconstruir el projecte en un framework amb base operativa real, persistència mínima real i primers fluxos funcionals verificables.

## Tasca

- tria l'stack de framework i deixa el projecte arrancant amb Docker
- configura `.env`, rutes mínimes i estructura base
- defineix quins `2` casos d'ús faràs en `R3`
- assegura que almenys `1` cas d'ús ve de `R2`
- crea BBDD real amb `migrations`
- carrega dades inicials amb `seeders` o equivalent
- implementa el primer flux end-to-end migrat de `R2`
- implementa un segon flux migrat o una ampliació funcional útil
- afegeix validació, errors bàsics i proves mínimes
- actualitza `README` amb arrencada, dades i ús
- deixa un mapa del que quedaria per migrar

## Evidència mínima

- Docker i framework arrancables
- `.env.example` o instruccions equivalents
- BBDD creada amb `migrations`
- dades inicials reproduïbles amb `seeders` o equivalent
- `2` casos d'ús funcionals de punta a punta
- prova que almenys `1` flux ve de `R2`
- validació i errors mínims
- proves o verificacions registrades
- `README` tècnic actualitzat

## Validació mínima

- arranca el projecte des de zero
- executa migracions i seeders
- mostra els dos fluxos funcionant
- provoca un error controlat
- explica el recorregut ruta, controlador, model o servei i resposta
- explica què queda fora de la migració total

## Errors habituals

- migrar només fitxers
- quedar-se en l'esquelet del framework
- fer només un cas d'ús
- carregar dades a mà
- usar BBDD sense `migrations` o `seeders`
- fer el segon flux com a canvi visual
- no provar errors

## Ampliació si acabes prompte

- afegeix una relació simple del domini
- reforça cobertura de proves
- millora tractament d'errors
- prepara un esborrany de recurs o endpoint per a `R4`
