# Versió prepilotatge v1

## Finalitat del document
Congelar una versió base usable del paquet docent abans del pilotatge real, de manera que quede clar què es considera prou madur per entrar en prepilotatge i què passa a una capa separada de millora pendent abans del curs següent.

Este document no torna a definir el model del curs. La seua funció és deixar fixat què entra en la `v1` prepilotatge, quines peces es poden usar ja amb criteri estable i on es talla la línia entre base consolidada i treball pendent.

## Què entra dins de la v1 prepilotatge
La `v1` prepilotatge inclou, com a paquet usable:
- projecte base del curs i enunciat base del producte
- seqüència de treball per reptes `R1-R5`
- materials comuns, materials nuclears per repte i apunts reals
- itineraris `Laravel`, `Express/Nest` i `FastAPI` com a variants homologables
- implantació docent en `2` avaluacions, amb calendari, programació, seqüenciació i curs executable
- sistema d'evidències, rúbriques, checklists i instruments de seguiment
- kits de pilotatge de les setmanes `1-20`
- pla de pilotatge, pla d'execució i peça de seguiment del pilotatge

## Què es considera estable
A efectes de prepilotatge, es considera estable allò que ja no necessita més arquitectura nova per poder-se usar amb sentit:
- el curs es desplega sobre un mateix producte backend i una seqüència comuna de reptes
- el desenvolupament principal es resol dins de les dues primeres avaluacions
- la tercera avaluació queda fora del desenvolupament nuclear del projecte
- l'avaluació es resol amb criteri individual, encara que puguen existir contextos de producte compartit
- Git/GitHub es tracta com a traçabilitat i repàs metodològic, no com a iniciació
- la IA es tracta com a eina guiada i verificable, amb contrast i defensa
- el nivell d'exigència es manté entre itineraris encara que canvie la implementació

## Quines peces estan prou madures per usar-se
Es consideren prou madures per entrar en prepilotatge:
- la visió global del model i el mapa mòdul-reptes
- el projecte base i la seqüència completa del curs en `20` setmanes
- la programació d'aula operativa i el curs executable en `2` avaluacions
- els materials comuns i els paquets nuclears dels Reptes `2`, `3`, `4` i `5`
- els materials de sessió contextualitzats per repte
- els itineraris tecnològics homologats
- la rúbrica base, la defensa tècnica, el sistema d'evidències i els instruments de seguiment
- els kits de pilotatge setmanals i la documentació de pilotatge real

Lectura pràctica:
- el paquet ja es pot revisar, preparar i activar com a sistema complet
- el que queda pendent és afinament i priorització, no construcció del nucli docent

## Què queda fora d'esta versió
Queda fora de la `v1` prepilotatge:
- qualsevol redisseny estructural dels reptes o de la seqüència temporal
- ajustos derivats d'observació real amb alumnat, perquè el pilotatge encara no s'ha executat
- refinaments editorials o de coherència que no bloquegen l'ús del paquet
- decisions fines sobre càrrega real, patrons d'incidència o ordre de checkpoints, que només tenen sentit amb evidència de pilotatge
- canvis reservats per a una futura `v2`

## Definition of done de la v1 prepilotatge
La `v1` prepilotatge es considera congelada quan:
- el paquet es pot descriure com un sistema docent complet i usable, no com una suma de peces en construcció
- queden clarament separades les peces estables de les millores pendents
- el professorat pot preparar el curs sense necessitat d'afegir nova arquitectura documental
- la base del model queda fixada en treball per reptes, projecte base compartit, seqüència en `2` avaluacions, evidències autèntiques i IA verificable
- el que queda pendent passa a backlog i no continua barrejant-se amb la definició de la versió base
