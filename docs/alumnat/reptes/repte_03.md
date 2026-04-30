# Repte 3. Framework, persistència real i dos fluxos funcionals

## Què és el repte

És el pas de "funciona en una base inicial" a "té una base real en framework". Has de reconstruir el projecte amb un framework, una BBDD real i primers fluxos verificables.

Ací és on entra el contrast de frameworks del curs. El mateix problema de `R2` continua ara amb `Laravel`, `Symfony` o `NestJS`.

No has de migrar tota l'aplicació de `R2`. Sí has de construir una base nova en framework i portar-hi almenys `2` casos d'ús end-to-end. Com a mínim `1` ha de vindre de `R2`; l'altre pot ser migrat o una ampliació funcional xicoteta i útil.

## Què no és suficient

- moure fitxers sense adaptar-los al framework
- fer només una arquitectura decorativa
- quedar-te en l'esquelet del framework
- connectar una BBDD sense `migrations` ni dades reproduïbles
- fer només un flux funcional
- afegir una pantalla nova que siga només cosmètica

## Mínim funcional no trivial

- Docker funcional
- projecte en framework arrancable
- configuració mínima i `.env`
- rutes, controladors i vistes, plantilles o respostes
- models, entitats, esquemes o capa equivalent de dades
- BBDD real creada amb `migrations`
- dades inicials amb `seeders` o equivalent
- `2` casos d'ús de punta a punta
- validacions i errors mínims
- proves mínimes executades
- README curt d'arrencada i ús

## Evidència mínima

- commits significatius del procés
- demo dels `2` casos d'ús
- prova que almenys `1` flux ve de `R2`
- execució de `migrations` i `seeders`
- proves o comprovacions registrades
- `README` i decisions tècniques actualitzades
- mapa del que quedaria per migrar després

## Errors habituals

- dir "migració" a copiar fitxers
- no saber explicar el recorregut ruta, controlador, model o servei i resposta
- usar dades estàtiques quan ja toca BBDD
- carregar dades a mà i no poder reconstruir l'entorn
- fer el segon flux massa gran o només visual
- no provar errors

## Connexió amb el següent pas

Si `R3` queda ben tancat, `R4` pot publicar una API real sobre una base estable. Si no, l'API quedarà penjada sobre un projecte que no es pot arrancar, provar o explicar bé.

## Si vols el detall complet

Consulta [Repte 3. Reconstrucció en framework, persistència real i primers fluxos funcionals](../../02_reptes/repte_03_mvc_i_persistencia.md).
