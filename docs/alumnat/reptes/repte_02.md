# Repte 2. Sessions, autenticació i primera funcionalitat

## Què és el repte

És el moment en què el producte deixa de ser només una base i passa a tindre una primera funcionalitat de negoci protegida per autenticació, sessió o estat equivalent.

El repte no es queda en formulari, login i error. El flux ha d’incloure entrada de dades, validació visible, processament, correcció quan hi ha error i conservació funcional de la informació correcta perquè després es puga reutilitzar.

Este repte es resol sobre una **base comuna en `PHP`**. El contrast fort de frameworks encara no és l'objectiu del repte.

La base del repte queda en `7` sessions de `3` hores. La sessió `7` està dedicada a refactorització i millora de mantenibilitat sobre el codi que ja funciona.

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
- revisió final del codi per reduir repetició, millorar noms i deixar el flux més clar

La base de dades pot aparéixer de manera controlada, però en `R2` encara no és el centre del repte. El focus continua sent el flux funcional complet i la seua defensa tècnica.

La sessió `7` no equival a passar tot el projecte a POO ni a obrir una arquitectura gran. És una sessió de neteja i millora de mantenibilitat.

## Evidència mínima

- demostració funcional del flux autenticat
- prova d'un cas permés i un cas denegat
- commits i documentació actualitzada
- verificació de validacions i errors
- justificació breu de la revisió final del codi
- `AI log` si la IA ha participat en una part rellevant

## Errors habituals

- deixar l'autenticació desacoblada del producte
- no protegir cap acció real
- no distingir autenticació de autorització
- no provar errors de credencials o accessos sense permís
- preparar massa coses per a després i no tancar el nucli

## Connexió amb el següent pas

En `R3` esta funcionalitat s'ha de mantindre viva, però ja amb entrada de framework, arquitectura o equivalent i persistència més explicable i segura. És ahí on comença el contrast de `Laravel`, `Symfony` o `NestJS`.

La sessió `7` ha de servir per fer una primera neteja útil, no per consumir abans d’hora tot el treball metodològic propi de `R3`.

## Si vols el detall complet

Consulta [Repte 2. Sessions, autenticació i primera funcionalitat de negoci](../../02_reptes/repte_02_sessions_i_autenticacio.md).
