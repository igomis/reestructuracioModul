# Projectes base

## Què és el projecte base
Durant el curs no faràs un projecte diferent en cada repte. Treballaràs sobre un únic producte backend que va creixent de `R1` a `R5`.

Els tres projectes base admesos són compatibles amb `Laravel`, `Express/Nest` i `FastAPI`. L'avaluació continua sent individual i la tokenització, quan apareix, s'entén com a mecanisme funcional útil del backend, no com a tema `web3`.

## 1. Gestor d'inventari amb rols i token d'operació
És una bona opció si t'interessa treballar amb recursos, moviments, autoritzacions i traçabilitat.

Normalment implica:
- recursos o actius amb estat i responsable
- operacions d'entrada, eixida o transferència
- rols que autoritzen o executen moviments
- un token d'operació per confirmar una entrega o transferència real

No és un simple llistat d'objectes. El mínim útil és un flux complet d'operació amb control d'accés i rastre.

## 2. Sistema de reserves amb tokens de confirmació o cancel·lació
És una bona opció si t'interessa treballar amb disponibilitat, franges, conflictes i estats.

Normalment implica:
- recursos o serveis reservables
- reserves en estat pendent, confirmat o cancel·lat
- validació de solapaments o límits temporals
- un token per confirmar o cancel·lar una reserva real

No és suficient guardar cites en una taula. Ha d'haver-hi regles de negoci i control d'estat.

## 3. Gestor d'incidències amb invitació o seguiment extern tokenitzat
És una bona opció si t'interessa treballar amb fluxos de treball, assignació, historial i comunicació amb tercers.

Normalment implica:
- incidències amb prioritat, estat i responsable
- historial de canvis i seguiment
- rols interns per gestionar i tancar
- un token per consulta externa, invitació o aportació limitada d'informació

No és un CRUD de tickets. Ha d'haver-hi un flux real de seguiment i resolució.

## Com triar bé
- tria un projecte que pugues imaginar viu fins a `R5`
- evita el que et semble "més fàcil" si en realitat no et suggerix casos d'ús clars
- pensa si el mateix projecte et permet auth, persistència, API i integració sense forçar-lo
- pensa també en la defensa: has de poder explicar actors, regles i decisions

## Si vols el detall complet
La concreció llarga està en [Projectes base concretats del mòdul](../05_projectes_tecnics/projectes_base_concretats.md).
