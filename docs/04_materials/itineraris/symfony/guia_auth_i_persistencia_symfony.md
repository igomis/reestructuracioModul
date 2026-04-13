# Guia d'auth i persistència en Symfony

## Finalitat

Traduir els mínims de `R3` i `R4` a l'itinerari `Symfony`, de manera que autenticació, persistència, validació i estructura de serveis queden resoltes amb una base defensable.

## Focus del curs

- preservar el flux real construït en `R2`
- separar entrada HTTP, negoci i persistència
- validar dades abans d'arribar a la capa de domini
- preparar el projecte per publicar `API` i continuar fins a `R5`

## Peces clau

- controladors curts
- serveis o casos d'ús recognoscibles
- entitats i repositoris coherents
- seguretat i autenticació explicables
- migracions i proves mínimes

## Errors a evitar

- fer servir autenticació sense connectar-la a una operació real del domini
- tindre persistència aparent però sense model clar
- obrir `API` sense haver estabilitzat abans la base de dades i la lògica

## Resultat esperat

- auth alineada amb el flux del projecte
- persistència coherent amb el model
- validació i errors tractats amb criteri
- base preparada per al contracte d'`API`
