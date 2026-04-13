# Repte 2. Sessions, autenticació i primera funcionalitat

## Què és el repte

És el moment en què el producte deixa de ser només una base i passa a tindre una primera funcionalitat de negoci protegida per autenticació, sessió o estat equivalent.

Este repte es resol sobre una **base comuna en `PHP`**. El contrast fort de frameworks encara no és l'objectiu del repte.

## Què no és suficient

- fer només registre, login i logout
- protegir una ruta sense valor real de domini
- no aplicar cap rol, permís o restricció
- validar només el cas feliç

## Mínim funcional no trivial

- tractament correcte de dades d'entrada al servidor
- lògica bàsica recognoscible dins del flux
- registre o alta d'usuari
- login, logout i comprovació de sessió
- almenys una funcionalitat real del domini protegida
- una regla de rol o restricció de negoci
- errors coherents d'autenticació, autorització i validació

## Evidència mínima

- demostració funcional del flux autenticat
- prova d'un cas permés i un cas denegat
- commits i documentació actualitzada
- verificació de validacions i errors
- `AI log` si la IA ha participat en una part rellevant

## Errors habituals

- deixar l'autenticació desacoblada del producte
- no protegir cap acció real
- no distingir autenticació de autorització
- no provar errors de credencials o accessos sense permís
- preparar massa coses per a després i no tancar el nucli

## Connexió amb el següent pas

En `R3` esta funcionalitat s'ha de mantindre viva, però ja amb entrada de framework, arquitectura o equivalent i persistència segura. És ahí on comença el contrast de `Laravel`, `Symfony` o `NestJS`.

## Si vols el detall complet

Consulta [Repte 2. Sessions, autenticació i primera funcionalitat de negoci](../../02_reptes/repte_02_sessions_i_autenticacio.md).
