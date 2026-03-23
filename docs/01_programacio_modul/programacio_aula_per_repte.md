# Programació d'aula per repte

## Finalitat del document
Baixar el model global d'implantació docent a una lectura operativa per repte, de manera que el professorat sàpia què convé activar, què ha de recordar, què ha de modelar en directe i quines evidències ha d'arreplegar en cada tram real del curs.

## Criteris d'ús
- este document complementa la programació d'aula global i la seqüenciació per sessions
- està pensat per a contextos on el projecte es desenvolupa dins de les dues primeres avaluacions lectives
- Git/GitHub es treballa com a repàs metodològic i criteri de traçabilitat, no com a iniciació des de zero
- cada repte combina explicació docent, modelatge en directe i treball autònom de l'alumnat
- el pas d'un repte al següent depén d'un checkpoint docent amb evidències mínimes

## Repte 1. Kickoff funcional del backend
### Finalitat docent
- obrir el projecte del curs amb un domini clar, un stack viable i una primera peça funcional real del producte

### Què no és suficient
- triar tecnologia o framework sense demostrar un primer flux executable
- deixar només un esquelet tècnic o una ruta de prova sense valor funcional
- usar el repositori com a contenidor final sense traçabilitat de decisions i proves

### Quin és el mínim funcional no trivial
- repositori inicial usable i decisió tecnològica justificada
- landing page o equivalent funcional d'entrada al producte
- formulari mínim per arreplegar una primera dada del domini
- validació bàsica al servidor i primer registre o persistència mínima de la informació

### Què diferencia una resolució superficial d'una professional
- superficial: stack triat, projecte arranca, però encara no hi ha producte recognoscible
- professional: la base tècnica ja produïx una primera interacció funcional, verificable i documentada

### Què sap ja l'alumnat
- té base prèvia de treball amb Git/GitHub
- coneix conceptes generals de desenvolupament web i entorns de projecte
- pot seguir una configuració guiada si l'objectiu està ben acotat

### Què cal recordar breument
- criteris de traçabilitat, `README`, `ADR`, evidències i `AI log`
- dominis admesos i lògica del projecte base
- que el repte no consistix a "instal·lar un framework", sinó a arrancar un producte

### Què ha d'explicar el professorat
- encàrrec del projecte base del curs
- domini, stack i criteris mínims d'arrancada
- què comptarà com a evidència vàlida en este primer repte

### Què ha de modelar en directe
- posada en marxa inicial del repositori amb estructura recognoscible
- exemple curt de `README` inicial i d'una primera decisió tècnica registrada
- arranque mínim d'un backend dins d'un dels itineraris autoritzats

### Què treballa l'alumnat amb autonomia
- selecció de domini i stack
- arranque de l'entorn tècnic
- primera decisió tècnica del producte
- organització inicial del repositori

### Materials que s'activen
- fitxa del Repte 1
- enunciat base del projecte
- materials comuns del mòdul
- itineraris tecnològics com a suport d'arrancada

### Evidències a arreplegar
- repositori usable
- primer `README`
- entorn funcional
- decisió de domini i stack
- primera traça tècnica del procés

### Errors habituals a anticipar
- arranque reduït a esquelet buit de framework
- domini triat sense impacte real en el producte
- repositori usat només com a dipòsit final
- ús de la IA sense contrast ni registre

### Checkpoint docent
- el grup només pot donar el repte per superat si té entorn executable, primer `README`, decisió tècnica i traçabilitat mínima del procés

## Repte 2. Sessions, autenticació i primera funcionalitat de negoci
### Finalitat docent
- construir la primera funcionalitat real del producte i demostrar que el backend ja resol un flux usable, autenticat i amb restriccions de negoci

### Què no és suficient
- implementar només registre, login o logout sense un cas d'ús del domini
- protegir una ruta decorativa o sense valor funcional real
- mostrar auth aparent sense proves d'accés, restriccions i errors

### Quin és el mínim funcional no trivial
- flux complet de registre o alta, login, logout i control d'accés
- almenys una funcionalitat de negoci autenticada del domini
- una regla de rol, permís o restricció recognoscible sobre eixa funcionalitat
- validacions i errors mínims verificats sobre el flux complet

### Què diferencia una resolució superficial d'una professional
- superficial: la sessió funciona, però el producte encara no resol res rellevant
- professional: l'autenticació sosté una operació de negoci real, defensable i comprovada

### Què sap ja l'alumnat
- ja té domini, stack i repositori activat
- sap posar en marxa l'entorn del projecte
- ha iniciat criteris de documentació i traçabilitat

### Què cal recordar breument
- lògica de validació de servidor i tractament mínim d'errors
- diferència entre demo puntual i flux real reproduïble
- necessitat de proves bàsiques i de documentació actualitzada

### Què ha d'explicar el professorat
- què és el mínim funcional exigible en auth o estat equivalent
- com es validen entrades i com es documenten errors
- quines evidències tècniques s'esperen per considerar el repte resolt

### Què ha de modelar en directe
- un flux simple de registre o login
- una validació de servidor amb resposta d'error comprensible
- una comprovació tècnica bàsica del flux implementat

### Què treballa l'alumnat amb autonomia
- construcció del flux funcional del repte
- control d'accés, sessió o estat equivalent
- validacions mínimes i primeres proves
- actualització de documentació operativa

### Materials que s'activen
- materials del Repte 2
- materials comuns
- suport inicial de l'itinerari triat

### Evidències a arreplegar
- flux funcional executable
- validacions i errors mínims controlats
- proves bàsiques o comprovacions equivalents
- `README` actualitzat
- `AI log` si aplica

### Errors habituals a anticipar
- validar només al client o només en casos feliços
- tindre auth aparent però sense accés protegit real
- funcionar només en una demostració preparada
- no poder explicar què ha generat la IA i què s'ha verificat

### Checkpoint docent
- no s'obri `R3` fins que el flux funcional siga real, reproduïble i mínimament verificat

## Repte 3. Arquitectura i persistència
### Finalitat docent
- passar d'un backend funcional a un backend mantenible, amb capes o equivalents i persistència coherent sobre una funcionalitat real ja existent

### Què no és suficient
- reorganitzar carpetes o fitxers sense millorar un cas d'ús real
- afegir persistència només aparent o només pensada per a la demo
- passar a MVC o equivalent sense proves de regressió ni defensa de decisions

### Quin és el mínim funcional no trivial
- almenys un cas d'ús del domini migrat a una estructura més mantenible
- persistència real de l'entitat principal o equivalent
- validacions lligades al model i no només al punt d'entrada
- comprovació que el flux funcional anterior continua viu després de la refactorització

### Què diferencia una resolució superficial d'una professional
- superficial: hi ha capes noves i base de dades, però el flux continua fràgil o opac
- professional: l'arquitectura és explicable, la persistència és coherent i el cas d'ús es pot verificar de punta a punta

### Què sap ja l'alumnat
- ja ha resolt un primer flux funcional del producte
- coneix el domini i els casos d'ús inicials
- manté documentació i traçabilitat mínimes

### Què cal recordar breument
- per què no s'ha d'obrir una `API` sobre estat efímer o arquitectura improvisada
- què és una separació de responsabilitats suficient segons l'itinerari
- com lligar model de dades, validació i persistència

### Què ha d'explicar el professorat
- criteris mínims de capes o equivalent
- model de dades mínim del domini
- relació entre persistència, regressió i mantenibilitat

### Què ha de modelar en directe
- refactorització curta d'una funcionalitat existent cap a una estructura més clara
- creació o lectura d'una entitat del domini amb persistència real
- comprovació bàsica que el canvi no trenca el flux anterior

### Què treballa l'alumnat amb autonomia
- modelat del domini
- pas a persistència funcional
- refactorització del projecte per capes o equivalent
- proves mínimes de regressió i revisió de documentació

### Materials que s'activen
- materials del Repte 3
- materials comuns
- itinerari triat com a suport directe de persistència i arquitectura

### Evidències a arreplegar
- model de dades explicable
- persistència coherent amb el domini
- refactorització recognoscible
- proves mínimes o verificacions equivalents
- documentació actualitzada

### Errors habituals a anticipar
- deixar tota la lògica en controladors o rutes
- persistència parcial o només preparada per a demo
- model de dades desalineat amb el producte real
- voler passar a `API` sense base persistent estable

### Checkpoint docent
- el grup només passa a `R4` si pot demostrar persistència real, arquitectura explicable i absència de dependència forta d'estat temporal

## Repte 4. Publicació i consum d'API
### Finalitat docent
- convertir el backend en un servei publicable, documentat i verificable a partir de funcionalitats reals del producte

### Què no és suficient
- obrir rutes o retornar JSON sense contracte ni valor funcional clar
- documentar una `API` que no coincidix amb el comportament real
- demostrar només el productor o només el consumidor, però no el flux complet

### Quin és el mínim funcional no trivial
- endpoints principals lligats a casos d'ús reals del domini
- contracte d'`API` amb errors, codis d'estat i validacions coherents
- consum verificat des d'un client, col·lecció de proves o servei auxiliar
- documentació operativa alineada amb el comportament real

### Què diferencia una resolució superficial d'una professional
- superficial: hi ha rutes i captures, però no un contracte usable per tercers
- professional: la `API` exposa valor real del producte, es pot consumir i es pot defensar tècnicament

### Què sap ja l'alumnat
- ja treballa amb persistència i arquitectura mínimes
- pot justificar el model de dades i la lògica principal del producte
- té una base de documentació i traçabilitat en marxa

### Què cal recordar breument
- contracte mínim d'`API`
- coherència entre endpoints, codis d'estat, errors i documentació
- necessitat de provar el consum i no només d'exposar rutes

### Què ha d'explicar el professorat
- quins recursos i operacions són realment nuclears
- com documentar una `API` del curs sense burocràcia innecessària
- quines proves mínimes fan falta per validar-la

### Què ha de modelar en directe
- definició curta d'un endpoint amb entrada, eixida i error controlat
- prova d'una operació d'`API`
- exemple mínim de documentació coherent amb el comportament real

### Què treballa l'alumnat amb autonomia
- implementació dels endpoints principals
- documentació del contracte d'`API`
- proves i consum verificat
- alineació de `README` i evidències tècniques

### Materials que s'activen
- materials del Repte 4
- materials comuns
- itineraris reutilitzats en context d'`API`

### Evidències a arreplegar
- endpoints principals funcionals
- documentació d'`API`
- col·lecció de proves o peticions verificades
- traça d'errors i correccions
- `README` actualitzat

### Errors habituals a anticipar
- `API` improvisada i desalineada amb el model del producte
- documentació que no reflectix el comportament real
- codis d'estat i errors incoherents
- absència de proves de consum

### Checkpoint docent
- no s'obri `R5` fins que la `API` estiga publicada, documentada i comprovada amb evidències mínimes

## Repte 5. Integració híbrida, automatització i tancament
### Finalitat docent
- completar el producte del curs amb una integració externa o automatització funcional, no trivial, i preparar la defensa final

### Què no és suficient
- muntar un workflow o una integració ornamental sense valor funcional clar
- demostrar només un efecte visual de l'automatització sense recorregut complet de dades
- arribar a defensa final sense proves de punta a punta ni control bàsic d'errors

### Quin és el mínim funcional no trivial
- un flux híbrid que reuse l'`API` del producte sobre un cas d'ús real
- prova de punta a punta del recorregut complet
- documentació de punts d'entrada, eixida, errors i decisions de manteniment
- defensa tècnica del valor i dels límits de la integració

### Què diferencia una resolució superficial d'una professional
- superficial: hi ha una automatització aparent, però no queda clar per a què servix ni com es manté
- professional: la integració tanca un procés de negoci recognoscible, es pot provar, revisar i defensar

### Què sap ja l'alumnat
- ja disposa d'un backend persistent i d'una `API` usable
- ha construït documentació, proves i traçabilitat en reptes anteriors
- coneix el seu itinerari i el comportament real del producte

### Què cal recordar breument
- què compta com a integració amb valor real i què és només ornament
- necessitat de prova de punta a punta
- paper central de la defensa, l'autoria i el contrast de la IA al tancament

### Què ha d'explicar el professorat
- criteris per triar una integració o workflow acceptable
- com documentar entrada, eixida i control d'errors del flux híbrid
- què s'espera d'una defensa final tècnica en este model

### Què ha de modelar en directe
- esquema d'un flux híbrid mínim amb punts d'entrada i eixida clars
- exemple de verificació d'un recorregut complet
- contrast breu de defensa tècnica sobre una decisió real del projecte

### Què treballa l'alumnat amb autonomia
- implementació de la integració final
- prova del flux complet
- tancament de documentació, `AI log` i narrativa de defensa
- revisió final de repositori i evidències

### Materials que s'activen
- materials del Repte 5
- materials comuns
- reutilització final dels itineraris per al tancament tècnic

### Evidències a arreplegar
- integració o workflow funcional
- prova de punta a punta
- documentació final
- defensa tècnica preparada
- traçabilitat final del procés

### Errors habituals a anticipar
- integració sense valor funcional real
- automatització no provada de punta a punta
- defensa desconnectada del repositori i de les evidències
- ús de la IA sense capacitat d'explicació o contrast final

### Checkpoint docent
- el projecte només queda tancat si el grup pot demostrar integració real, prova completa, repositori coherent i defensa tècnica suficient abans de `FCT`

## Definition of done del document
Este document es considera completat quan:
- dona una lectura docent específica per als reptes `1-5`
- deixa clar què sap ja l'alumnat i què cal recordar en cada repte
- explicita què ha d'explicar i modelar el professorat
- diferencia treball docent i treball autònom de l'alumnat
- identifica materials, evidències, errors habituals i checkpoint docent per repte
