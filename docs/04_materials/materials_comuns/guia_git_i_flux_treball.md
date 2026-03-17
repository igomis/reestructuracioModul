# Guia de Git i flux de treball

Esta guia no parteix d'una alfabetització inicial en Git o GitHub. S'assumix que l'alumnat ja coneix els conceptes bàsics i que el document servix per normalitzar la forma de treballar, repassar criteris clau i usar el repositori com a evidència professional del procés.

## Finalitat
Establir un flux mínim de treball amb Git que siga reutilitzable en tots els reptes del mòdul i que deixe evidències autèntiques del procés real de desenvolupament.

Esta guia no planteja Git com una formalitat administrativa, sinó com una peça central de treball professional: ha de permetre seguir l'evolució del producte, entendre decisions, revisar incidències i comprovar que el que es defensa en un repte realment s'ha construït al repositori.

## Contingut operatiu
- treballar cada repte o microtasca amb una referència clara a issue, objectiu o tasca de treball
- dividir el treball en canvis curts i verificables, no en una única pujada final
- fer commits coherents: un objectiu clar, un canvi clar i un estat revisable
- descriure en el commit què s'ha canviat i amb quin propòsit
- mantindre `master` com a referència estable i evitar períodes llargs sense traçabilitat
- fer `push` només quan el canvi es puga executar, revisar o defensar
- usar el repositori com a rastre de decisions, correccions, regressions i evolució del producte

Flux mínim recomanat:
1. llegir l'encàrrec del repte o de la microtasca
2. identificar quina part del treball generarà evidència real al repositori
3. preparar el canvi amb abast curt i concret
4. implementar i verificar localment
5. fer commit amb missatge clar
6. fer `push` i deixar el canvi visible al repositori

Artefactes mínims que s'espera trobar:
- seqüència de commits amb evolució real del treball
- relació recognoscible entre issue, repte i canvi aplicat
- estat del repositori prou net perquè el professorat o l'equip puguen revisar el procés
- historial que permeta distingir implementació, correcció, documentació i ajustos finals

Criteri pràctic de missatges:
- usar una primera paraula que situe el tipus de canvi quan aporte claredat: `docs`, `fix`, `feat`, `test`
- evitar missatges genèrics com `canvis`, `proves`, `última versió`
- si el canvi respon a una incidència o una part concreta del repte, deixar-ho recognoscible al missatge

## Errors habituals o riscos
- fer un únic commit gran al final i perdre la traçabilitat del treball
- treballar directament sense cap relació amb issue, repte o objectiu concret
- pujar canvis sense comprovar que el resultat és coherent o executable
- usar Git només com a còpia de seguretat i no com a registre professional d'evolució
- reescriure o compactar tant l'historial que ja no es puga entendre com s'ha arribat al resultat final
- presentar un repositori aparentment net però sense evidència real de proves, correccions o iteracions

## Checklist final
- hi ha una relació clara entre el que es treballa i una issue, repte o microtasca
- els commits mostren evolució real i no una pujada única al final
- els missatges de commit expliquen el canvi amb criteri professional
- el codi o document pujat correspon a un estat revisable
- el repositori permet reconstruir què s'ha fet i en quin ordre
- el `push` no es fa només per còpia de seguretat, sinó per deixar evidència visible i contrastable
- les correccions importants també deixen rastre i no desapareixen dins d'un commit massa gran
