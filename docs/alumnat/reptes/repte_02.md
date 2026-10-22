# Repte 2. Sessions, autenticació i primera funcionalitat

## Què és el repte

És el moment en què el producte deixa de ser només una base i passa a tindre una primera funcionalitat de negoci protegida per autenticació, sessió o estat equivalent.

El repte no es queda en formulari, login i error. El flux ha d’incloure entrada de dades, validació visible, processament, correcció quan hi ha error i conservació funcional de la informació correcta perquè després es puga reutilitzar.

Este repte es resol sobre una **base comuna en `PHP`**. El contrast fort de frameworks encara no és l'objectiu del repte.

La base del repte queda en `9` sessions de `3` hores. La sessió `7` automatitza el flux HTTP; la sessió `8` crea una primera peça testable amb POO, Composer i prova unitària; la sessió `9` introduïx persistència mínima amb BBDD.

## Què no és suficient

- fer només registre, login i logout
- protegir una ruta sense valor real de domini
- no aplicar cap rol, permís o restricció
- validar només el cas feliç

## Mínim funcional no trivial

- tractament correcte de dades d'entrada al servidor
- visualització d'errors de validació i possibilitat de reintent
- lògica bàsica recognoscible dins del flux
- conservació funcional simple de la informació correcta
- reutilització posterior d'eixa informació dins del projecte
- registre o alta d'usuari
- login, logout i comprovació de sessió
- almenys una funcionalitat real del domini protegida
- una regla de rol o restricció de negoci
- tractament d'imatge o fitxer si el cas d'ús ho demana
- errors coherents d'autenticació, autorització i validació
- `tests/flux-r2.php` o una prova HTTP equivalent que comprove login, accés protegit i logout amb assercions
- primera classe simple carregada amb Composer i provada amb una prova unitària mínima

La base de dades pot aparéixer de manera controlada, però en `R2` encara no és el centre del repte. El focus continua sent el flux funcional complet i la seua defensa tècnica.

La sessió `7` convertix les comprovacions manuals en un recorregut executable que falla davant resultats inesperats. La sessió `8` no equival a passar tot el projecte a POO: crea una sola peça unitària i torna a executar el flux.

## Evidència mínima

- demostració funcional del flux autenticat
- prova d'un cas permés i un cas denegat
- commits i documentació actualitzada
- verificació de validacions i errors
- prova HTTP automatitzada amb denegació inicial, login incorrecte i correcte, operació protegida, logout i denegació final
- `composer.json` o equivalent, classe simple i prova unitària mínima
- `AI log` si la IA ha participat en una part rellevant

## Errors habituals

- deixar l'autenticació desacoblada del producte
- no protegir cap acció real
- no distingir autenticació de autorització
- no provar errors de credencials o accessos sense permís
- preparar massa coses per a després i no tancar el nucli

## Connexió amb el següent pas

En `R3` esta funcionalitat s'ha de mantindre viva, però ja amb entrada de framework, arquitectura o equivalent i persistència més explicable i segura. És ahí on comença el contrast de `Laravel`, `Symfony` o `NestJS`.

La sessió `7` comprova el flux des de fora; la sessió `8` prova una peça interna. Cap de les dos ha de consumir abans d’hora tot el treball metodològic propi de `R3`.

## Si vols el detall complet

Consulta [Repte 2. Sessions, autenticació i primera funcionalitat de negoci](../../02_reptes/repte_02_sessions_i_autenticacio.md).
