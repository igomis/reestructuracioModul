# Apunts reals del Repte 1. Kickoff backend

## Finalitat del document

Convertir el Repte 1 en un apunt de treball real, curt i executable, pensat perquè professorat i alumnat tinguen clara la seqüència mínima per arrancar el producte amb una primera peça funcional visible, verificable i documentada.

Este repte no consistix a triar tecnologia ni a crear un esquelet buit. El que s'espera és posar en marxa una base tècnica curta i defensable: model client/servidor comprensible, entorn executable amb `Docker`, `PHP` i servidor web, primer punt d'entrada funcional del backend i documentació tècnica usable.

## Calibratge d'aula

- `12` hores de base
- `4` sessions de `3` hores
- `1` microrepte docent per sessió

## Què sap ja l'alumnat

- té base prèvia de treball amb Git/GitHub
- coneix conceptes generals de desenvolupament web i estructura de projecte
- pot seguir una guia de posada en marxa si l'objectiu funcional està ben acotat
- ja entén que el curs treballa amb evidències, `README`, `ADR`, traçabilitat i `AI log`

## Què s'ha de recordar breument

- Git/GitHub es tracta com a metodologia de treball i criteri de traçabilitat, no com a iniciació
- el domini triat ha de permetre construir un producte recognoscible i evolutiu
- un projecte no compta com a iniciat si només arranca tècnicament però encara no resol cap interacció real
- la IA es pot usar com a suport, però totes les propostes s'han de verificar i poder defensar

## Què ha d'explicar el professorat

- quin és l'encàrrec real del Repte 1: deixar una base funcional del producte, no només infraestructura
- quins dominis admesos encaixen amb el projecte base del curs
- què és el mínim funcional no trivial: una resposta real del backend sobre una base que arranca i es pot explicar
- quines evidències mínimes s'han de deixar des del primer dia: `README`, decisió tècnica, traçabilitat i comprovació funcional

## Què s'ha de modelar en directe

- una posada en marxa mínima del repositori i de l'estructura del projecte
- una decisió tècnica inicial breu registrada al `README` o a un `ADR`
- una arrencada real amb `Docker`, `PHP` i servidor web
- una ruta, vista, `endpoint` o `healthcheck` simple servit pel backend
- una revisió del `README` perquè una altra persona puga repetir la prova

## Què treballa l'alumnat amb autonomia

- triar el domini concret i justificar-lo
- decidir el marc tècnic dins de la base guiada del curs
- preparar repositori, estructura mínima i convencions bàsiques de treball
- implementar la primera peça funcional d'entrada al producte
- verificar l'arrencada i deixar evidències clares de funcionament
- actualitzar `README`, `ADR` i `AI log` si hi ha ús d'IA

## Exemple mínim orientatiu

Exemple orientatiu de recorregut mínim:

1. Explicar amb un dibuix curt o una nota tècnica on està el client i on està el servidor.
2. Fixar una decisió tècnica inicial coherent amb la base del curs.
3. Preparar l'entorn amb `Docker`, `PHP` i servidor web.
4. Arrancar el projecte i demostrar que la base és executable.
5. Implementar una ruta, vista, `endpoint` o `healthcheck` simple però funcional.
6. Deixar constància al `README` de com reproduir l'arrencada i la prova funcional.

Criteri docent:

- el valor no està en la quantitat de fitxers o contenidors
- el valor està en demostrar que el backend arranca, respon i es pot explicar

## Errors habituals

- confondre arrancada tècnica amb primera funcionalitat real
- deixar només una ruta de prova o un text estàtic sense flux recognoscible
- no saber què fa cada component de l'entorn
- tindre un `README` que no permet repetir l'arrencada
- tindre `README` massa genèric o incomplet
- usar IA per generar arrencada, configuració o estructura sense entendre què s'ha creat

## Com es verifica que funciona

Per donar el repte per verificat, cal poder demostrar com a mínim:

- que el projecte arranca seguint el `README`
- que existix un punt d'entrada funcional del backend
- que es pot explicar el paper de `Docker`, `PHP` i del servidor web
- que la resposta del sistema és real i reproduïble
- que el repositori mostra traçabilitat recognoscible del treball

Formats de verificació acceptables:

- demostració tècnica en aula o revisió docent
- registre manual clar al `README`
- prova reproduïble del flux descrit pas a pas
- captura o log només com a suport, mai com a substitut d'una reproducció real

## Evidències que s'han d'entregar

- repositori amb estructura inicial usable
- `README` de posada en marxa i comprovació del Repte 1
- justificació breu del domini i de la decisió tècnica inicial
- entorn executable amb `Docker`, `PHP` i servidor web
- evidència del primer punt d'entrada funcional del backend
- traçabilitat mínima del procés amb commits i, si aplica, issues
- `AI log` si s'ha utilitzat IA per a configuració, esquelets o documentació

## Checklist final del repte

- [ ] existix repositori usable i estructura inicial coherent
- [ ] la decisió tecnològica està justificada de manera breu i defensable
- [ ] el projecte arranca amb `Docker`, `PHP` i servidor web
- [ ] existix ruta, vista, `endpoint` o `healthcheck` funcional d'entrada al backend
- [ ] el `README` explica com arrancar i provar el repte
- [ ] hi ha traçabilitat mínima del procés de treball
- [ ] l'ús de la IA, si existix, està registrat i contrastat
- [ ] queda clar que "triar tecnologia" o "crear esquelet" no és suficient per donar el repte per superat

## Connexió amb el Repte 2

El Repte 1 només té sentit si deixa preparada l'entrada al primer flux funcional autenticat del producte. En concret, hauria de deixar identificat:

- quin punt d'entrada del backend evolucionarà a funcionalitat de negoci real
- quin actor o usuari tindrà sentit en el pas a autenticació
- quina part de la base tècnica es mantindrà i quina s'haurà d'enfortir amb control d'accés i estat

Lectura de transició:

- si `R1` només ha deixat infraestructura, `R2` començarà massa tard
- si `R1` ja ha deixat una entrada funcional del backend i una base executable, `R2` podrà convertir-la en un flux autenticat i amb regla de negoci
