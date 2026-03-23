# Apunts reals del Repte 1. Kickoff backend

## Finalitat del document
Convertir el Repte 1 en un apunt de treball real, curt i executable, pensat perquè professorat i alumnat tinguen clara la seqüència mínima per arrancar el producte amb una primera peça funcional visible, verificable i documentada.

Este repte no consistix a triar tecnologia ni a crear un esquelet buit. El que s'espera és posar en marxa una primera entrada real al producte, per exemple una landing page o equivalent, un formulari útil, validació mínima al servidor i una primera arreplegada o registre de dades.

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
- què és el mínim funcional no trivial: landing page o equivalent, formulari, validació i primer registre de dades
- quines evidències mínimes s'han de deixar des del primer dia: `README`, decisió tècnica, traçabilitat i comprovació funcional

## Què s'ha de modelar en directe
- una posada en marxa mínima del repositori i de l'estructura del projecte
- una decisió tècnica inicial breu registrada al `README` o a un `ADR`
- una landing page o equivalent servida pel backend
- un formulari funcional que arreplegue una primera dada útil del domini
- una validació bàsica al servidor i una resposta clara en cas correcte i incorrecte
- un registre mínim de la informació, encara que siga bàsic o provisional

## Què treballa l'alumnat amb autonomia
- triar el domini concret i justificar-lo
- decidir l'stack dins dels itineraris admesos
- preparar repositori, estructura mínima i convencions bàsiques de treball
- implementar la primera peça funcional d'entrada al producte
- validar el flux mínim i deixar evidències clares de funcionament
- actualitzar `README`, `ADR` i `AI log` si hi ha ús d'IA

## Exemple mínim orientatiu
Exemple orientatiu de recorregut mínim:
1. Crear una pàgina inicial del producte amb una explicació breu del servei.
2. Afegir un formulari per arreplegar una primera dada útil del domini.
3. Validar al servidor que els camps obligatoris arriben correctament.
4. Rebutjar la petició si falta informació mínima o si el format és incorrecte.
5. Registrar la dada enviada en fitxer, memòria controlada o persistència bàsica.
6. Deixar constància al `README` de com reproduir el flux.

Exemples de dada inicial útil:
- una sol·licitud d'incidència
- una petició de reserva
- una alta o petició d'un recurs intern

Criteri docent:
- el valor no està en la complexitat del formulari
- el valor està en demostrar que el producte ja té una primera interacció real i verificable

## Errors habituals
- confondre arrancada tècnica amb primera funcionalitat real
- deixar només una ruta de prova o un text estàtic sense flux recognoscible
- validar només al client o no validar res
- guardar dades sense criteri o sense poder reproduir després què s'ha registrat
- tindre `README` massa genèric o incomplet
- usar IA per generar arrencada, formulari o estructura sense entendre què s'ha creat

## Com es verifica que funciona
Per donar el repte per verificat, cal poder demostrar com a mínim:
- que el projecte arranca seguint el `README`
- que existix una landing page o equivalent funcional d'entrada al producte
- que el formulari es pot enviar
- que el servidor valida almenys els camps obligatoris
- que hi ha resposta diferenciada entre cas correcte i incorrecte
- que la informació enviada queda registrada o persistida de manera mínima i comprovable
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
- formulari funcional i validació mínima al servidor
- evidència del primer registre o persistència de dades
- traçabilitat mínima del procés amb commits i, si aplica, issues
- `AI log` si s'ha utilitzat IA per a configuració, esquelets, validació o documentació

## Checklist final del repte
- [ ] existix repositori usable i estructura inicial coherent
- [ ] la decisió tecnològica està justificada de manera breu i defensable
- [ ] existix landing page o equivalent funcional d'entrada al producte
- [ ] existix formulari útil per arreplegar una primera dada del domini
- [ ] el servidor valida almenys els camps obligatoris
- [ ] la dada enviada queda registrada o persistida de manera mínima i verificable
- [ ] el `README` explica com arrancar i provar el repte
- [ ] hi ha traçabilitat mínima del procés de treball
- [ ] l'ús de la IA, si existix, està registrat i contrastat
- [ ] queda clar que "triar tecnologia" o "crear esquelet" no és suficient per donar el repte per superat

## Connexió amb el Repte 2
El Repte 1 només té sentit si deixa preparada l'entrada al primer flux funcional autenticat del producte. En concret, hauria de deixar identificat:
- quina dada inicial del domini evolucionarà a funcionalitat de negoci real
- quin actor o usuari tindrà sentit en el pas a autenticació
- quina part del flux inicial es mantindrà i quina s'haurà d'enfortir amb control d'accés, validació i estat

Lectura de transició:
- si `R1` només ha deixat infraestructura, `R2` començarà massa tard
- si `R1` ja ha deixat una entrada funcional del producte, `R2` podrà convertir-la en un flux autenticat i amb regla de negoci
