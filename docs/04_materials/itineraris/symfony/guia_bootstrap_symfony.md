# Guia de bootstrap Symfony

## Finalitat

Oferir una base operativa perquè l'itinerari `Symfony` es puga arrancar amb criteri tècnic a partir de `R3`, sense convertir l'entrada al framework en un front separat del projecte del curs.

## Quan usar Symfony dins del projecte

Convé usar `Symfony` quan:

- el mateix projecte de `R2` ja està consolidat sobre la base comuna en `PHP`
- cal professionalitzar controladors, serveis, entitats i persistència
- l'equip pot defensar l'ús del framework i no només el seu esquelet

## Mínim exigible

- estructura de projecte reproduïble
- configuració bàsica comprensible
- controladors i serveis recognoscibles
- entitats i persistència alineades amb el domini
- instruccions clares de posada en marxa al `README`

## Errors a evitar

- entrar a `Symfony` abans de tancar el flux real de `R2`
- confiar tota la comprensió a `maker` o a la IA
- dissoldre la lògica del projecte dins del controlador

## Resultat esperat

- el projecte arranca amb passos clars
- la separació de responsabilitats és recognoscible
- la base queda preparada per a persistència, `API` i integració
