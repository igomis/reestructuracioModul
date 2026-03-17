# Guia de Git i flux de treball

## Finalitat
Establir un flux mínim de treball amb Git que siga reutilitzable en tots els reptes del mòdul i que deixe evidències autèntiques del procés real de desenvolupament.

## Contingut mínim operatiu
- treballar cada repte o microtasca amb una referència clara a issue, objectiu o tasca de treball
- fer commits curts i coherents, cadascun amb un canvi verificable
- mantindre `master` com a referència estable i evitar canvis llargs sense traçabilitat
- descriure en el commit què s'ha canviat i amb quin propòsit
- fer `push` només quan el canvi es puga executar, revisar o defensar
- usar el repositori com a rastre de decisions, correccions i evolució del producte

Flux mínim recomanat:
1. llegir l'encàrrec del repte o de la microtasca
2. preparar el canvi amb abast curt i concret
3. implementar i verificar localment
4. fer commit amb missatge clar
5. fer `push` i deixar el canvi visible al repositori

## Checklist o punts clau
- hi ha una relació clara entre el que es treballa i una issue, repte o microtasca
- els commits mostren evolució real i no una pujada única al final
- els missatges de commit expliquen el canvi amb criteri professional
- el codi o document pujat correspon a un estat revisable
- el repositori permet reconstruir què s'ha fet i en quin ordre

## Errors habituals o riscos
- fer un únic commit gran al final i perdre la traçabilitat del treball
- treballar directament sense cap relació amb issue, repte o objectiu concret
- pujar canvis sense comprovar que el resultat és coherent o executable
- usar Git només com a còpia de seguretat i no com a registre professional d'evolució
