# Revisió editorial final del paquet docent

## Finalitat del document

Deixar constància de la ronda final de revisió editorial del paquet docent, indicant quins criteris s'han usat, quins documents s'han revisat, quines incoherències s'han detectat i quins ajustos s'han aplicat per millorar llegibilitat, coherència i navegació del repositori.

## Criteris de revisió editorial

- unificar terminologia clau en els documents de portada i en les peces centrals del model
- mantindre una estructura pública similar en els documents estratègics del paquet
- evitar redundàncies i canvis cosmètics sense impacte real d'ús
- facilitar navegació i lectura ràpida per a professorat que arriba al repositori des de la capa de desplegament
- mantindre el nucli del model: treball per reptes, projecte base, `2` avaluacions lectives, evidències autèntiques i IA verificable

## Terminologia a unificar

- usar `paquet docent exportable i reutilitzable` com a formulació preferent
- substituir l'anglicisme `reusable` per `reutilitzable`
- usar `Git/GitHub` quan es parla de metodologia de treball i traçabilitat
- mantindre `curs executable` com a nom de la peça docent principal d'ús real
- mantindre `instruments de seguiment docent` com a nom del paquet de control i revisió periòdica
- mantindre `2 avaluacions lectives` com a formulació de referència del model temporal

## Estructura mínima comuna dels documents clau

Per als documents centrals de la fase final del paquet docent es fixa esta estructura mínima comuna:

- `Finalitat del document`
- context o criteris d'ús
- cos operatiu principal
- punts crítics, riscos o decisions docents
- `Definition of done`

Lectura editorial:

- no tots els documents han de tindre exactament la mateixa llargària
- sí han de permetre una lectura ràpida, una lectura operativa i una localització clara del tancament del document

## Documents revisats

- `README.md`
- `docs/00_visio_general/issues_inicials.md`
- `docs/00_visio_general/paquet_docent_exportable.md`
- `docs/00_visio_general/revisio_editorial_final.md`
- `docs/01_programacio_modul/calendaritzacio_per_avaluacions.md`
- `docs/01_programacio_modul/seqüenciacio_sessions_2_avaluacions.md`
- `docs/01_programacio_modul/curs_executable_dwes_2_avaluacions.md`
- `docs/03_avaluacio/instruments_seguiment_docent.md`
- `docs/06_plantilles/plantilla_paquet_modul_reptes_ia.md`

## Incoherències detectades

- alternança entre `reusable` i `reutilitzable`
- alternança entre `Git i GitHub` i `Git/GitHub` en documents de primera línia
- `README.md` encara llegia la fase següent com a pas previ a l'exportació, quan el paquet exportable ja estava creat
- l'estat de producció encara no reflectia la revisió editorial final com a fase explícita
- la nova capa de revisió i presentació final encara no tenia una peça pròpia que la documentara

## Canvis aplicats

- normalització de `reusable` a `reutilitzable` en documents clau
- normalització de `Git/GitHub` com a formulació preferent quan es parla de traçabilitat i metodologia
- actualització del `README` perquè el focus actual passe de construcció del paquet a revisió editorial final i preparació compartible
- actualització de `issues_inicials.md` perquè `ID-09` quede consolidat i `ID-10` entre en producció
- incorporació d'esta peça de revisió editorial final per deixar rastre explícit de la consolidació de presentació
- millora de navegació al `README` afegint la revisió editorial final com a document visible de la fase actual

## Aspectes pendents o opcionals

- preparar una versió encara més compartible del paquet, pensada per lliurament extern o circulació entre centres
- crear, si realment fa falta, una portada resum o índex curt de paquet docent
- revisar més avant si convé una versió PDF o de lliurament institucional del paquet
- fer una última passada de consolidació sobre `MG-05` i `MG-06`, que continuen oberts a nivell de materials

## Definition of done de la revisió final

La revisió editorial final es considera completada quan:

- els documents clau de la fase final compartixen terminologia coherent
- el `README` i l'estat de producció reflectixen l'estat real del paquet docent
- les incoherències detectades queden registrades i resoltes si afectaven navegació o lectura
- el paquet exportable queda presentat com a conjunt reutilitzable i compartible
- el següent pas del repositori ja és de presentació externa o lliurament, no de reconstrucció interna del model
