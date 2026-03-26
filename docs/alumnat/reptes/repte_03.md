# Repte 3. MVC i persistència

## Què és el repte

És el pas de "funciona" a "es pot mantindre". Has d'ordenar el producte, separar responsabilitats i consolidar persistència sobre un cas d'ús real.

## Què no és suficient

- moure fitxers sense millorar el comportament real
- fer una arquitectura decorativa
- connectar una base de dades sense un flux complet persistent
- reescriure de zero i perdre la funcionalitat anterior

## Mínim funcional no trivial

- estructura MVC o equivalent aplicada de veritat
- model de dades persistent i explicable
- almenys un cas d'ús real refactoritzat de punta a punta
- validacions i errors coherents
- proves mínimes executades

## Evidència mínima

- commits de migració incremental
- cas d'ús verificat amb persistència real
- proves o comprovacions registrades
- `README` i decisions tècniques actualitzades
- demostració que la funcionalitat principal continua viva

## Errors habituals

- fer una neteja cosmètica i dir-li refactorització
- no conservar el flux del repte anterior
- persistència aparent però no robusta
- no provar regressions
- crear massa capes innecessàries

## Connexió amb el següent pas

Si `R3` queda ben tancat, `R4` pot publicar una API real del producte. Si no, l'API quedarà penjada sobre una base dèbil.

## Si vols el detall complet

Consulta [Repte 3. Migració a MVC i persistència segura](../../02_reptes/repte_03_mvc_i_persistencia.md).
