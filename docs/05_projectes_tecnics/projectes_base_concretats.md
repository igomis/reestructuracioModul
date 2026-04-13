# Projectes base concretats del mòdul

## Finalitat del document

Baixar l'[enunciat base del projecte del curs](enunciat_projecte_base.md) a tres encàrrecs docents quasi tancats, usables i comparables, de manera que el projecte base deixe de ser només un domini general i passe a ser una proposta operativa ja defensable en aula.

Este document no substituïx l'enunciat base. El concreta. La seua funció és fixar tres projectes compatibles amb `Laravel`, `Symfony` i `NestJS`, sostenibles dins de la seqüència en `2` avaluacions i prou densos per generar evidències autèntiques i defensa individual.

La tokenització s'entén ací en sentit funcional útil per al backend: tokens d'operació, confirmació, cancel·lació, invitació o seguiment. No es planteja com a línia `web3` obligatòria ni com a ornament tècnic.

## Criteris per seleccionar projecte

- el projecte ha de permetre construir un únic producte evolutiu durant `R1-R5`, no un conjunt d'exercicis desconnectats
- ha de tindre actors recognoscibles, rols clars i una primera funcionalitat de negoci usable des del primer tram del curs
- ha de permetre model de dades no trivial, persistència, API, validacions de negoci, proves i manteniment real
- ha d'admetre una tokenització funcional útil del domini sense convertir-se en un projecte especialitzat en criptografia
- ha de ser compatible amb acreditació individual: cada alumne ha de poder implementar, explicar, provar i defensar la seua solució
- ha de ser comparable entre itineraris: canvia l'stack, no el nivell d'exigència ni el tipus d'evidència
- ha de cabre en un recorregut docent realista d'unes `20` setmanes i unes `120` hores lectives dins de les dues primeres avaluacions
- ha d'evitar lectures trivials del producte: no val un CRUD sense regles, sense fluxs o sense rastre verificable

Seqüència metodològica associada:

- `R2` és base comuna en `PHP`
- `R3-R5` obrin el contrast de frameworks
- la cooperació docent es formula com a contrast tècnic compartit amb implementació individual

## 1. Gestor d'inventari amb rols i token d'operació

### Context professional

Una organització necessita gestionar material intern, equips i moviments entre espais o responsables. No vol un simple llistat d'objectes, sinó un backend que controle qui pot demanar, autoritzar, entregar, rebre i deixar rastre d'una operació d'inventari.

El token d'operació representa una autorització funcional per executar una entrega, una retirada o una transferència concreta. Pot usar-se com a codi curt, enllaç segur o valor d'un sol ús associat a una operació real.

### Actors

- administrador del sistema
- responsable d'inventari o magatzem
- usuari intern que sol·licita material o demana un moviment
- persona receptora o validadora de l'operació

### Casos d'ús obligatoris

- donar d'alta, editar i desactivar recursos o actius
- classificar recursos per tipus, estat, ubicació i responsable
- registrar entrades, eixides o transferències
- crear una sol·licitud de moviment o d'entrega
- aprovar o rebutjar una operació segons rol
- generar un token d'operació per a una entrega o transferència autoritzada
- validar el token i tancar l'operació deixant rastre d'execució
- consultar l'estat actual i l'historial d'un recurs

### Mínim funcional no trivial

El producte mínim no trivial ha d'incloure usuaris amb rols, recursos inventariables, operacions de moviment, historial i un flux complet de sol·licitud -> autorització -> generació de token -> execució -> tancament.

No és suficient una aplicació que només cree recursos i els llista. Ha d'existir almenys una operació d'inventari amb control d'accés, validació, persistència i token funcional consumible.

### Restriccions i validacions mínimes

- cada recurs ha de tindre identificador intern únic
- no es poden executar eixides o transferències sobre recursos inactius o inexistents
- només els rols autoritzats poden aprovar operacions i generar tokens
- el token d'operació ha d'estar lligat a una única operació, amb caducitat i consum únic
- una operació tancada no es pot tornar a confirmar
- el sistema ha de registrar qui crea, qui autoritza i qui executa l'operació
- si hi ha quantitats o stock, no es poden deixar valors negatius ni moviments incoherents

### Relació amb `R1-R5`

- `R1`: arrencada del repositori, primera pàgina o formulari útil i primera captura d'una sol·licitud o alta de recurs
- `R2`: autenticació, rols i primera funcionalitat autenticada de sol·licitud o aprovació
- `R3`: persistència del model d'inventari, operacions i historial, amb proves mínimes
- `R4`: API per consultar recursos, crear operacions, validar tokens i documentar contractes
- `R5`: integració amb notificacions, lector de codis, webhook o automatització de tancament i manteniment

### Evidències autèntiques esperades

- issues o tasques que separen alta de recurs, model de rols, operacions i tokenització
- README amb posada en marxa i flux de prova complet
- migracions o model persistent de recursos, moviments, usuaris i tokens
- proves sobre autorització, consum del token i consistència d'operacions
- documentació d'API sobre consultes, creació d'operació i validació del token
- registres de prova o captures del flux complet d'entrega o transferència
- AI log o rastre equivalent quan s'haja usat IA

### Punts de defensa individual

- justificar per què el model separa recursos, operacions, historial i tokens
- explicar el cicle de vida del token i com s'eviten reutilitzacions o confirmacions dobles
- defensar les decisions de rol i autorització
- mostrar com es manté la consistència de les operacions davant errors o intents duplicats
- relacionar clarament el que s'ha implementat en cada repte amb el producte final

### Extensió opcional de tokenització útil

Es pot ampliar el projecte amb tokens d'operació signats, codi `QR`, revocació manual, reutilització prohibida per finestra temporal o traçabilitat multi-pas d'una operació complexa.

## 2. Sistema de reserves amb tokens de confirmació o cancel·lació

### Context professional

Una organització gestiona reserves d'espais, recursos o cites de servei. Necessita controlar disponibilitat, conflictes, confirmacions i cancel·lacions sense convertir el sistema en un simple calendari passiu.

Els tokens de confirmació o cancel·lació servixen per validar una reserva provisional, confirmar-la des d'un enllaç segur o cancel·lar-la sense obligar sempre a una sessió autenticada completa, sempre dins d'un flux de negoci real.

### Actors

- administrador del sistema
- gestor del servei o responsable de disponibilitat
- usuari autenticat que fa o gestiona reserves
- persona usuària externa o destinatària d'un token de confirmació/cancel·lació

### Casos d'ús obligatoris

- definir recursos reservables, franges i regles bàsiques de disponibilitat
- consultar disponibilitat abans de reservar
- crear una reserva en estat provisional o pendent
- confirmar una reserva mitjançant token o acció autenticada
- cancel·lar una reserva mitjançant token o acció autenticada
- evitar conflictes de franges, duplicitats o capacitat superada
- llistar reserves per usuari, recurs, data i estat
- registrar l'historial de canvis rellevants d'una reserva

### Mínim funcional no trivial

El mínim funcional no trivial ha d'incloure recursos reservables, franges o blocs temporals, usuaris, reserves amb estat i almenys un flux complet de reserva provisional -> confirmació o cancel·lació -> actualització d'estat.

No és suficient un formulari que cree cites en una taula. Ha d'haver-hi validació temporal, control d'estats, autenticació o tokens funcionals i tractament de conflictes reals.

### Restriccions i validacions mínimes

- no es poden crear reserves solapades per al mateix recurs i franja incompatible
- el sistema ha de validar dates, duració mínima o màxima i disponibilitat real
- un token de confirmació o cancel·lació ha d'estar associat a una reserva concreta, amb caducitat i ús controlat
- una reserva cancel·lada no es pot confirmar després sense nou procés
- només els rols autoritzats poden forçar reserves, reobrir-les o anul·lar restriccions
- el sistema ha de reflectir clarament els estats mínims: pendent, confirmada, cancel·lada i, si cal, expirada

### Relació amb `R1-R5`

- `R1`: primera entrada funcional del producte amb consulta bàsica de disponibilitat o petició inicial de reserva
- `R2`: autenticació, model d'usuari i primera reserva autenticada o provisional
- `R3`: persistència de recursos, franges i reserves, amb regles anti-conflicte i proves
- `R4`: API de disponibilitat, creació de reserves i confirmació/cancel·lació tokenitzada
- `R5`: integració amb notificacions, calendari extern, recordatoris o automatitzacions de venciment

### Evidències autèntiques esperades

- backlog o issues separades per disponibilitat, reserves, estats i tokens
- README amb dades de prova i exemples de conflictes temporals
- model persistent de recursos, franges, reserves, usuaris i tokens
- proves sobre solapament, expiració, confirmació i cancel·lació
- contractes API clars per disponibilitat, reserva i operacions tokenitzades
- evidència d'un flux de negoci complet amb reserva pendent i canvi d'estat verificable
- registre d'ús d'IA quan s'haja emprat com a suport

### Punts de defensa individual

- explicar com es resolen els conflictes de reserva i per què eixa estratègia és defensable
- justificar l'estat provisional i el paper del token dins del flux
- mostrar com es valida la disponibilitat i què passa davant concurrència o duplicitat
- defensar les restriccions temporals i els criteris de cancel·lació
- demostrar que l'API i el model persistent reflectixen el comportament real del sistema

### Extensió opcional de tokenització útil

Es pot ampliar amb tokens de reprogramació, check-in, recordatori, ampliació de termini o confirmació multiactor quan una reserva requerix més d'una validació.

## 3. Gestor d'incidències amb invitació o seguiment extern tokenitzat

### Context professional

Un servei tècnic, departament intern o equip de suport necessita gestionar incidències amb classificació, assignació, historial i comunicació amb tercers. El problema no és només registrar tickets, sinó coordinar treball, seguiment i resposta.

La tokenització permet obrir seguiment extern o invitacions controlades: per exemple, una persona externa pot consultar l'estat, aportar informació o confirmar resolució amb un token específic sense necessitar un compte complet.

### Actors

- administrador del sistema
- agent o tècnic de suport
- usuari autenticat que obri incidències
- persona externa convidada o autoritzada amb token de seguiment

### Casos d'ús obligatoris

- crear incidències amb descripció, categoria, prioritat i context mínim
- assignar o reasignar incidències a un responsable
- canviar estat amb historial traçable
- afegir comentaris interns o visibles segons rol
- generar un token d'invitació o seguiment extern per a una incidència concreta
- permetre consulta externa limitada o aportació d'informació via token
- tancar o reobrir incidències segons criteri de negoci
- consultar llistats per estat, prioritat, responsable o origen

### Mínim funcional no trivial

El mínim funcional no trivial ha d'incloure incidències, usuaris, assignacions, historial i un flux complet de creació -> classificació -> seguiment -> tancament, amb participació externa o consulta externa controlada per token.

No és suficient un CRUD de tickets. Ha d'haver-hi estats, prioritats, traçabilitat, control d'accés i un ús real del token per obrir o limitar un canal extern de seguiment.

### Restriccions i validacions mínimes

- una incidència no es pot tancar sense estat coherent, responsable o evidència mínima definida pel sistema
- només determinats rols poden assignar, prioritzar o tancar incidències
- el token extern ha d'estar limitat a una incidència concreta, amb permisos explícits i caducitat
- l'accés extern via token no ha de permetre operacions internes no autoritzades
- els canvis d'estat han de quedar traçats amb autor, moment i motiu mínim
- s'ha de validar que la informació mínima per obrir una incidència siga suficient per treballar-la

### Relació amb `R1-R5`

- `R1`: primera entrada funcional amb formulari de registre d'incidència o contacte inicial del servei
- `R2`: autenticació, model de rols i primera incidència autenticada o assignable
- `R3`: persistència del model d'incidències, estat, comentaris i historial, amb proves mínimes
- `R4`: API de consulta, creació, assignació i seguiment extern tokenitzat
- `R5`: integració amb notificacions, webhook, automatització de derivació o tancament assistit

### Evidències autèntiques esperades

- issues separades per creació, classificació, assignació, estat i seguiment extern
- README amb dades de prova i itinerari d'ús intern i extern
- model persistent d'incidències, comentaris, historial, usuaris i tokens
- proves sobre permisos, transicions d'estat i límits del token extern
- documentació d'API dels endpoints interns i del canal extern tokenitzat
- registre del flux complet des de l'obertura fins al tancament o resposta externa
- AI log quan la IA haja participat en decisions, proves o revisió

### Punts de defensa individual

- justificar el model d'estats i per què no és un simple llistat de tickets
- explicar com es limita el canal extern i quins permisos es donen via token
- defensar la separació entre comentaris interns i visibles externament, si existix
- mostrar la traçabilitat d'assignació, resolució i reobertura
- connectar clarament el treball dels reptes amb un flux professional recognoscible

### Extensió opcional de tokenització útil

Es pot ampliar amb tokens de satisfacció, confirmació de resolució, invitació temporal a proveïdors externs o reobertura controlada d'una incidència resolta.

## Criteris per decidir quin projecte oferir o assignar

- oferix **gestor d'inventari** quan vulgues prioritzar traçabilitat, rols, consistència d'operacions i una tokenització funcional molt acotada i fàcil de defensar
- oferix **sistema de reserves** quan vulgues reforçar validacions temporals, conflictes de negoci i tractament d'estats vinculats a disponibilitat
- oferix **gestor d'incidències** quan vulgues prioritzar flux de treball, assignació, historial i comunicació amb tercers o seguiment extern
- si el grup és heterogeni, convé oferir com a màxim `2` opcions reals i no obrir un catàleg massa ampli
- si l'objectiu principal és comparabilitat forta entre alumnes, convé assignar un únic projecte base o una única parella de variants amb els mateixos casos d'ús obligatoris
- si l'objectiu principal és diversificar contextos sense perdre comparabilitat, es pot repartir projecte segons perfil, però mantenint la mateixa exigència en auth, persistència, API, proves, integració i defensa
- en tots els casos, l'assignació ha de pensar-se per a avaluació individual: mateix marc docent, repositoris separats o responsabilitat clarament traçable, i defensa tècnica personal

## Definition of done del document

Este document es considera completat quan:

- concreta operativament els dominis admesos de l'enunciat base en tres projectes ja usables
- definix criteris clars de selecció i d'assignació docent
- descriu per a cada projecte context, actors, casos d'ús, mínim funcional, validacions, relació amb `R1-R5`, evidències i defensa
- manté compatibilitat real amb `Laravel`, `Symfony` i `NestJS`
- manté el criteri de treball per reptes, entorn professional realista i acreditació individual
- tracta la tokenització com a mecanisme funcional útil del backend i no com a exigència aliena al mòdul
- deixa el paquet docent més tancat, més executable i més defensable que la llista prèvia de dominis generals
