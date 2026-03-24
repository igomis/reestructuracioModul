# Full de treball del Repte 3

## Objectiu
Professionalitzar el flux principal del producte amb arquitectura més clara, persistència real i una primera prova de regressió.

## Tasca
- tria quina operació real de `R2` és la més important
- separa millor entrada, lògica i persistència, o equivalent segons l'itinerari
- crea o consolida una entitat principal del domini
- deixa una operació persistent de punta a punta
- prova que el flux principal continua viu després del canvi
- actualitza `README` amb com reproduir el repte

## Evidència mínima
- estructura recognoscible i explicable
- una entitat principal persistent
- creació o consulta real del domini amb persistència
- una prova o verificació de regressió mínima
- `README` tècnic actualitzat

## Validació mínima
- mostra on entra la petició, on va la lògica i on persistix
- crea o recupera una dada real del domini
- prova un cas incorrecte o incoherent
- torna a executar el flux principal de `R2`

## Errors habituals
- reorganitzar carpetes sense millorar cap cas d'ús real
- afegir base de dades però continuar depenent d'estat provisional
- barrejar validació, lògica i persistència al mateix punt
- no provar regressions després del canvi
- no saber explicar per què l'estructura nova és millor

## Ampliació si acabes prompte
- afegeix una relació més clara del domini
- reforça una prova de regressió
- millora noms, separació de capes o claredat del model
