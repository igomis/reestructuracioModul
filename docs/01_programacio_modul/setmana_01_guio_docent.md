# Guió docent complet de la setmana 1

## Finalitat de la setmana

Esta setmana ha de situar el curs, fer comprensible què significa programar en entorn servidor i deixar el producte realment arrancat. No es tracta només de preparar la base comuna en `PHP` i instal·lar dependències, però tampoc d'exigir ja el tractament complet d'un flux funcional de formulari en servidor.

El tancament correcte de la setmana 1 és este:

- el curs queda explicat en clau de treball per reptes i producte únic
- l'alumnat entén la lògica bàsica client/servidor i petició/resposta
- el projecte base queda triat i la base comuna en `PHP` queda assumida com a punt de partida
- el projecte arranca localment amb estructura recognoscible
- existix una pantalla inicial funcional, visible i coherent amb el producte
- la traçabilitat inicial i l'ús acceptable de la IA queden activats en clau individual

## Límit didàctic de la setmana

La pantalla inicial pot incloure un formulari o un altre element d'entrada del domini, però el seu tractament complet en servidor no és encara exigible en setmana 1. El que sí és exigible és que la peça estiga integrada en el producte, siga visible, arranque des del backend i tinga sentit dins del cas d'ús triat.

La recepció completa de la dada, la validació en servidor, el cas incorrecte i la persistència poden quedar per a les setmanes següents dins de `R1`.

## Què ha d'explicar el professorat

- què és el curs i com es treballa per reptes: un únic producte backend que creix de `R1` a `R5`, no una col·lecció de pràctiques aïllades
- que l'avaluació és individual encara que puguen existir parelles de contrast tècnic o moments puntuals de coordinació
- què és programar en entorn servidor: codi que viu al backend, rep peticions, aplica lògica i retorna una resposta útil
- diferència client/servidor: què passa al navegador o client i què passa al servidor
- lògica de petició/resposta: ruta, entrada, processament bàsic i resposta visible
- arquitectura mínima o estructura inicial d'un backend: punt d'entrada, configuració, rutes, controladors o handlers, vista o resposta, serveis o capes mínimes i espai per a persistència posterior
- què necessita un projecte per arrancar bé: repositori usable, projecte base recognoscible, base comuna en `PHP`, entorn preparat, instruccions d'arrancada, estructura mínima i primer rastre de decisions
- què és un mínim funcional no trivial en setmana 1: una peça real del producte servida pel backend i explicable, no un esquelet buit
- què compta com a evidència: `README`, justificacions curtes, commits o rastre equivalent, prova d'arrancada i peça visible del producte
- què és traçabilitat individual: cada alumne ha de poder mostrar què ha decidit, què ha fet i què ha verificat
- quin és l'ús acceptable de la IA: ajuda guiada, verificable, citada o registrada quan toca, i sempre sota comprensió i defensa pròpia
- que Git/GitHub es reprén com a metodologia de treball i autoria, no com a iniciació des de zero

## Conceptes mínims que l'alumnat ha d'entendre

- el curs es resol construint un únic producte backend per reptes
- la setmana 1 no tanca encara tot `R1`, però sí l'arrancada real del producte
- programar en entorn servidor no és només fer una pantalla: és fer que el backend servisca una resposta útil
- client i servidor tenen rols diferents i han de poder explicar-se amb un exemple del propi projecte
- tota funcionalitat visible ha d'estar connectada amb un cas d'ús real del domini
- projecte base i base comuna en `PHP` no són una capa ornamental: condicionen l'estructura i el tipus d'arrancada abans del pas a frameworks
- un `README` inicial i la traçabilitat individual formen part de la feina, no són un afegit final
- la IA només és acceptable si el seu ús queda guiat, verificable i defensable

## Què modela el professorat en directe

- lectura curta del briefing del curs i del criteri de no trivialitat del producte
- tria d'un projecte base i lectura explícita de la base comuna en `PHP` com a punt d'arrancada
- preparació d'entorn i arrencada local del projecte de referència
- recorregut comentat per l'estructura mínima del backend perquè es veja on entren rutes, controladors o handlers, configuració i resposta
- creació o adaptació de la ruta inicial del producte perquè el backend servisca una primera pantalla recognoscible
- construcció d'una pantalla inicial funcional alineada amb el domini triat
- incorporació, si convé, d'un formulari o element d'entrada visible dins d'eixa pantalla, deixant clar que el tractament complet al servidor vindrà després
- actualització del `README` inicial amb objectiu del producte, com arranca, decisions preses i següent pas
- primera traçabilitat individual modelada: nota breu de decisió, commit o registre equivalent i anotació d'ús d'IA si s'ha utilitzat

## Què fa l'alumnat

- tria el projecte base del curs sobre el qual treballarà
- assumix la base comuna en `PHP` amb què arrancarà el backend
- deixa una justificació curta de les dos decisions
- prepara l'entorn local i comprova que el projecte arranca
- posa en marxa l'estructura mínima de treball del projecte
- construeix una pantalla inicial funcional servida pel backend
- integra en eixa pantalla, si és coherent amb el producte, un formulari o altre element d'entrada visible del domini
- assumix que el tractament complet del formulari en servidor no és encara exigible en esta setmana
- redacta un `README` inicial amb context, arrencada, decisió de projecte base, base comuna assumida i estat actual
- deixa la primera traçabilitat individual: decisió registrada, primer rastre de treball i ús verificable de la IA si l'ha emprada

## Evidència mínima de la setmana 1

- projecte base triat i justificat
- base comuna en `PHP` assumida i arrencada justificada
- entorn preparat i projecte arrancant localment
- estructura inicial del backend recognoscible
- pantalla inicial funcional i servida pel projecte
- formulari o element d'entrada visible si forma part natural de la pantalla inicial
- `README` inicial usable per entendre què és el producte i com arranca
- primera traçabilitat individual visible

Criteri important:

- si hi ha formulari, no cal exigir encara recepció completa, validació completa en servidor ni persistència
- sí cal exigir que la peça siga funcional, visible i coherent amb el producte que s'està començant

## Què no és suficient

- només preparar la base tècnica i parar ahí
- només instal·lar dependències
- només crear repositori
- una pantalla purament decorativa sense cap relació clara amb el producte
- un `hello world`
- un projecte que arranca però que no permet entendre quin producte es construirà
- un `README` buit o una decisió tècnica sense justificació mínima

## Errors habituals a anticipar

- convertir la setmana en un debat massa llarg de frameworks i retardar l'arrancada real
- confondre l'esquelet del framework amb un producte ja iniciat
- no explicar bé la diferència client/servidor i deixar la pantalla inicial com a maqueta estàtica
- voler tancar massa prompte el formulari complet en servidor i bloquejar l'arrancada
- deixar el `README` per al final o tractar-lo com a tràmit
- no deixar rastre individual perquè es pressuposa cooperació tècnica
- usar IA per generar peces que després no es poden entendre ni verificar
- dedicar temps a reexplicar Git/GitHub des de zero en lloc d'exigir-ne un ús operatiu

## Checkpoint de final de setmana

Al tancament de la setmana 1, cada alumne ha de poder mostrar i explicar:

- quin projecte base ha triat i per què
- com ha arrancat la base comuna en `PHP` i per què és coherent amb el producte
- què vol dir, en el seu cas, programar en entorn servidor
- on es veu la diferència client/servidor en el seu projecte
- com arranca el projecte i què retorna o renderitza la ruta inicial
- quina pantalla inicial funcional té ja el producte
- quina traçabilitat individual ha deixat
- com ha usat la IA, si l'ha usada, i com ho ha verificat
- quin és el següent pas funcional que quedarà per a setmana 2

## Materials que s'activen

- [guia_sessio_a_sessio_20_setmanes.md](guia_sessio_a_sessio_20_setmanes.md)
- [kit_pilotatge_setmanes_01_04.md](kit_pilotatge_setmanes_01_04.md)
- [preparacio_docent_directa_curs_que_ve.md](preparacio_docent_directa_curs_que_ve.md)
- [briefing_inicial_curs.md](../08_materials_compartibles/briefing_inicial_curs.md)
- [full_treball_repte_01.md](../08_materials_compartibles/full_treball_repte_01.md)
- [guio_ús_ia_per_a_lalumnat.md](../08_materials_compartibles/guio_ús_ia_per_a_lalumnat.md)
- [projectes_base_concretats.md](../05_projectes_tecnics/projectes_base_concretats.md)

## Definition of done del document

Este document es considera completat quan:

- baixa la setmana 1 a un nivell operatiu prou concret per conduir l'inici del curs sense improvisació
- deixa clar què s'ha d'explicar, què s'ha de modelar i què ha de fer l'alumnat
- explicita el tall entre arrencada funcional del producte i tractament complet del formulari en servidor
- fixa evidències mínimes, criteris d'insuficiència, errors previsibles i checkpoint final
- manté coherència amb la guia de `20` setmanes, el kit `1-4`, la preparació docent directa, el briefing inicial i el full de treball de `R1`
- manté visibles l'avaluació individual, la traçabilitat i l'ús guiats i verificables de la IA
