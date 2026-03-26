# Checkpoint `R3 -> R4`

## Per a què servix

Esta comprovació curta servix per decidir si el producte ja està prou professionalitzat per publicar una part real com a `API`.

## Hauries de poder ensenyar

- una arquitectura recognoscible
- una entitat principal persistent
- un cas d'ús real que funciona de punta a punta
- una prova o verificació de regressió mínima
- una idea clara de quin recurs o operació passarà a `API`

## Com es verifica en `2-3` minuts

- mostra on entra la petició, on va la lògica i on persistix
- crea o recupera una dada real del domini
- repetix el flux principal després del canvi
- explica quin endpoint o recurs publicaràs i per què

## Senyals d'alerta

- hi ha canvi d'estructura però no millora funcional recognoscible
- la persistència és parcial o només per a demo
- no es pot provar el flux sense improvisació
- el grup no sap què publicarà en `R4`

## Acció correctiva ràpida

- tornar a una sola operació central
- tancar persistència real d'una entitat principal
- deixar una prova mínima de regressió
- no obrir `API` fins que el backend siga prou estable
