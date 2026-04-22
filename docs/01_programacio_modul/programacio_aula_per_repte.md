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

- obrir el projecte del curs amb una base clara sobre `PHP`, un entorn executable i un primer punt d'entrada funcional del backend

### Duració base recomanada

- `12` hores
- `4` sessions de `3` hores
- una sessió per cada microrepte docent de `R1`

### Què no és suficient

- triar tecnologia o framework sense demostrar un primer flux executable
- deixar només un esquelet tècnic o una ruta de prova sense valor funcional
- usar el repositori com a contenidor final sense traçabilitat de decisions i proves

### Quin és el mínim funcional no trivial

- repositori inicial usable i base comuna en `PHP` clarament assumida
- entorn executable amb `Docker`, `PHP` i servidor web
- una ruta, vista, `endpoint` o `healthcheck` funcional d'entrada al backend
- `README` executable i verificació bàsica del que ja funciona

### Què diferencia una resolució superficial d'una professional

- superficial: infraestructura arrencada, però encara no hi ha producte recognoscible
- professional: la base tècnica ja arranca, es pot explicar i deixa un primer punt d'entrada funcional, verificable i documentat

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
- model client/servidor, base tècnica inicial i criteris mínims d'arrancada
- què comptarà com a evidència vàlida en este primer repte

### Què ha de modelar en directe

- posada en marxa inicial del repositori amb estructura recognoscible
- exemple curt de `README` inicial i d'una primera decisió tècnica registrada
- arranque mínim d'un backend amb `Docker`, `PHP` i servidor web
- primer punt d'entrada funcional simple del backend

### Què treballa l'alumnat amb autonomia

- selecció de domini i resolució de la base inicial
- arranque de l'entorn tècnic
- primera decisió tècnica del producte
- organització inicial del repositori
- primer punt d'entrada funcional del backend
- documentació i verificació bàsica del que ja funciona

### Materials que s'activen

- fitxa del Repte 1
- enunciat base del projecte
- materials comuns del mòdul
- base comuna del curs com a suport d'arrancada

### Evidències a arreplegar

- repositori usable
- primer `README`
- entorn funcional
- decisió de domini i base comuna assumida
- primera traça tècnica del procés
- punt d'entrada funcional del backend

### Errors habituals a anticipar

- arranque reduït a esquelet buit de framework
- domini triat sense impacte real en el producte
- repositori usat només com a dipòsit final
- ús de la IA sense contrast ni registre

### Checkpoint docent

- el grup només pot donar el repte per superat si té entorn executable, primer `README`, decisió tècnica, punt d'entrada funcional i traçabilitat mínima del procés

## Repte 2. Processament, estat, autenticació i primera funcionalitat de negoci

### Finalitat docent

- construir la primera funcionalitat real del producte a partir d'un flux complet: entrada de dades, processament en servidor, lògica bàsica, estat, autenticació i operació protegida sobre una base comuna en `PHP`

### Duració base recomanada

- `21` hores
- `7` sessions de `3` hores
- una sessió per cada microprojecte docent principal

### Coordinació mínima entre microprojectes

- `MP1`: formulari i validació visible
- `MP2`: processament i guardat funcional
- `MP3`: lògica del flux i regles del projecte
- `MP4`: estat, sessió i/o cookies
- `MP5`: autenticació i funcionalitat protegida
- `MP6`: prova, depuració, documentació mínima i checkpoint tècnic
- `MP7`: refactorització, organització en fitxers i primer objecte de domini

### Què no és suficient

- implementar només formulari, registre, login o logout sense un cas d'ús del domini
- protegir una ruta decorativa o sense valor funcional real
- convertir la persistència en el centre del repte mentre el flux principal continua dèbil
- deixar la prova només com a frase final sense verificació real del recorregut
- convertir la sessió `7` en una reescriptura arquitectònica gran o en una entrada obligatòria a POO completa i BBDD

### Quin és el mínim funcional no trivial

- formulari o entrada equivalent amb validació visible
- tractament correcte en servidor i conservació funcional de la informació
- almenys una regla recognoscible del projecte
- evidència d'estat, sessió i/o cookies quan el flux ho necessita
- una funcionalitat de negoci autenticada del domini
- una prova autoritzada, una prova denegada i un cas d'error o validació visible
- una revisió final del codi amb millora de mantenibilitat justificable, `include` / `require` amb sentit i un objecte mínim de domini

### Què diferencia una resolució superficial d'una professional

- superficial: hi ha auth aparent, però el producte encara no resol res rellevant, no es pot demostrar el flux complet o la sessió `7` es reduïx a canvis cosmètics
- professional: l'autenticació sosté una operació de negoci real, la dada correcta es reutilitza, els errors són visibles, el conjunt es pot provar i la revisió final deixa el codi un poc més clar i mantenible

### Què sap ja l'alumnat

- ja té domini, repositori i base tècnica activats
- sap posar en marxa l'entorn del projecte
- ha iniciat criteris de documentació i traçabilitat

### Què cal recordar breument

- la diferència entre estat temporal i conservació funcional del domini
- que la persistència pot aparéixer, però encara no és el focus principal
- la diferència entre autenticació, autorització i funcionalitat protegida
- que el contrast de frameworks encara no és el centre del repte
- que la sessió `7` millora mantenibilitat, però no substituïx `R3`
- que la sessió `7` ha d'incorporar organització simple en fitxers i un objecte mínim del domini sense convertir el repte en POO completa

### Què ha d'explicar el professorat

- la seqüència real del repte: dades, processament, lògica, estat, auth, prova i revisió final de mantenibilitat
- quins criteris de `RA2`, `RA3` i `RA4` es fan visibles en cada tram
- com es validen entrades, com es documenten errors i quina prova mínima s'exigirà

### Què ha de modelar en directe

- una entrada de dades amb validació visible
- un tram curt de processament en servidor amb resposta generada
- una regla bàsica del domini o un ús d'estat recognoscible
- una comprovació tècnica del cas autoritzat i del cas denegat
- una revisió curta de codi amb comparativa abans/després, extracció a fitxer comú amb `require_once` o equivalent, primer objecte simple del domini i comprovació final del flux

### Què treballa l'alumnat amb autonomia

- construcció del flux funcional del repte
- processament, lògica i conservació funcional de dades
- estat, sessió o mecanisme equivalent
- control d'accés, validacions i primeres proves
- revisió final del codi, organització en fitxers i primer objecte del domini
- actualització de documentació operativa

### Materials que s'activen

- materials del Repte 2
- materials comuns
- base comuna en `PHP`
- programació d'aula específica de `R2`

### Evidències a arreplegar

- flux funcional executable
- validacions i errors mínims controlats
- primera reutilització de la informació correcta
- estat o sessió verificables
- operació real protegida
- proves bàsiques o comprovacions equivalents
- comparativa breu abans/després de la revisió final
- almenys un fitxer comú reutilitzat amb `include` / `require` i una entitat simple del domini
- `README` actualitzat
- `AI log` si aplica

### Errors habituals a anticipar

- validar només al client o només en casos feliços
- tindre auth aparent però sense acció protegida real
- confondre persistència del domini amb estat temporal
- funcionar només en una demostració preparada
- voler convertir la sessió `7` en un salt complet a arquitectura o persistència forta
- no poder explicar què ha generat la IA i què s'ha verificat

### Checkpoint docent

- no s'obri `R3` fins que el flux funcional siga real, reproduïble, mínimament verificat i la sessió `7` haja deixat una primera millora de mantenibilitat explicable

### Regla metodològica del repte

- `R2` manté una base comuna més controlada
- `R2` incorpora una sessió final real de refactorització i millora de mantenibilitat
- la sessió `7` ha d'introduir reutilització en fitxers i un objecte mínim del domini sense convertir-se en un bloc de POO completa
- el contrast de `Laravel`, `Symfony` i `NestJS` entra després
- la prova i la depuració no es deixen només per al final, sinó que s'arrepleguen al llarg dels microprojectes
- la sessió `7` no substituïx el treball d’arquitectura, persistència i frameworks propi de `R3`

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

En este punt, l'itinerari base del projecte pot ser:

- `Laravel`
- `Symfony`
- `NestJS`

`FastAPI` només s'hauria d'obrir si el centre l'està treballant com a via avançada o excepcional.

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

## Organització docent del contrast

- la modalitat base és la de parelles de contrast tècnic
- es manté el mateix projecte i el mateix encàrrec funcional
- el repositori, la traçabilitat i la defensa continuen sent individuals
- els trios avançats només s'obrin amb prou autonomia i tres stacks diferents realment sostenibles

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
