# Guió docent complet de la setmana 2

## Finalitat de la setmana

Esta setmana ha de convertir l'arrancada del producte en una primera pràctica real del comportament bàsic del backend. El focus no està en incorporar ja un framework pesat, sinó en entendre i programar què fa el servidor quan rep dades, les tracta, aplica una validació mínima i retorna una resposta coherent.

El tancament correcte de la setmana 2 és este:

- l'alumnat defineix un primer flux real del seu projecte
- el flux s'implementa sobre la base comuna en `PHP`
- el servidor rep una entrada recognoscible, la tracta i retorna una resposta
- es distingixen com a mínim un cas correcte i un cas incorrecte
- hi ha validació mínima de dades, encara que siga simple
- el `README` i la traçabilitat individual deixen rastre del que realment s'ha construït

## Límit didàctic de la setmana

Encara no és setmana de framework complet. Tampoc és moment d'obrir itineraris diferents: ara interessa consolidar els `RA` previs sobre la base comuna en `PHP`, entendre el cicle bàsic d'una aplicació en entorn servidor i programar-lo de manera explícita abans de passar al contrast de frameworks.

## Què ha d'explicar el professorat

- el cicle bàsic d'una aplicació en entorn servidor: entrada, tractament, validació mínima i resposta
- què vol dir programar este comportament en un llenguatge real i no només dibuixar una interfície o descriure un flux
- com entra la dada al servidor i com es transforma en una decisió o en una resposta útil del producte
- què és una dada d'entrada mínima i quina validació té sentit exigir en este moment
- diferència entre resposta correcta i resposta d'error, encara que les dos siguen simples
- quina és l'estructura mínima del codi abans del framework: punt d'entrada, funció o handler, comprovació de dades i resposta
- per què encara no entra un framework pesat: primer cal entendre el comportament, després encapsular-lo en estructures més grans
- que Laravel no és l'entrada adequada en esta setmana perquè ocultaria massa decisions que encara s'han de veure amb claredat
- que el contrast de frameworks no entra encara: primer cal dominar el flux bàsic sobre `PHP`
- què compta com a primer flux real del projecte: una operació concreta del domini que rep alguna dada i retorna una eixida coherent
- com es manté l'avaluació individual encara que hi haja context compartit de producte
- què ha de quedar registrat al `README`, a la traçabilitat i en l'ús verificable de la IA

## Conceptes mínims que l'alumnat ha d'entendre

- un backend no queda obert perquè tinga una pantalla, sinó perquè tracta una entrada real i respon amb sentit
- programar en servidor és decidir què passa amb la dada quan arriba
- qualsevol flux mínim ha de distingir almenys un cas correcte i un cas incorrecte
- validar no és només comprovar que el programa no caiga: és decidir què és acceptable i què no
- una resposta d'error també forma part del comportament correcte del backend
- encara no és setmana de framework complet ni d'entrar en Laravel
- usar la base comuna en `PHP` obliga a veure el flux amb més claredat i ajuda a consolidar els `RA` previs
- el `README`, la traçabilitat i l'ús d'IA continuen sent part del treball, no annexos

## Què modela el professorat en directe

- definició d'un primer flux real del domini triat, acotat a una sola entrada i una sola resposta principal
- implementació del flux sobre `PHP`, sense dependre d'un framework complet
- recepció d'una dada simple del client o de la petició
- tractament mínim d'eixa dada perquè el servidor faça alguna operació recognoscible
- validació mínima d'un camp o condició obligatòria
- resposta correcta quan la dada compleix el criteri
- resposta d'error quan la dada no el compleix
- recorregut pel codi per mostrar on està l'entrada, on està el tractament, on està la validació i on està la resposta
- actualització del `README` amb descripció del flux implementat i com provar-lo
- registre de traçabilitat individual i d'ús d'IA, si s'ha utilitzat suport extern

## Què fa l'alumnat

- defineix el primer flux real del seu projecte
- implementa este flux sobre la base comuna en `PHP`
- distingix explícitament el cas correcte i el cas incorrecte
- valida mínimament les dades d'entrada
- fa que el servidor retorne una resposta coherent en els dos casos
- evita convertir la setmana en una migració prematura a un framework pesat
- manté el focus en el flux bàsic en `PHP`, sense obrir encara itineraris ni frameworks
- actualitza el `README` amb el flux implementat, com arrancar-lo i com provar el cas correcte i l'error
- deixa evidència individual del treball realitzat i del seu ús verificable de la IA si n'ha fet ús

## Evidència mínima de la setmana 2

- primer flux real del projecte definit i explicable
- implementació funcional sobre la base comuna en `PHP`
- entrada de dades realment tractada pel servidor
- validació mínima visible i defensable
- cas correcte reproduïble
- cas incorrecte o error reproduïble
- resposta coherent en els dos casos
- `README` actualitzat amb arrencada, flux i prova mínima
- evidència individual recognoscible

## Què no és suficient

- tindre només una pantalla o formulari dibuixat
- no tractar cap dada real
- no distingir cas correcte i error
- mostrar respostes falses o decoratives
- limitar-se a descriure el flux sense programar-lo
- voler anticipar un framework i no saber explicar encara què passa amb la dada en `PHP`
- usar IA sense poder explicar el flux, la validació i la resposta

## Errors habituals a anticipar

- voler entrar massa prompte en Laravel o en una arquitectura massa pesada
- confondre progrés tècnic amb quantitat de llibreries o estructura afegida
- rebre la dada però no tractar-la realment
- tractar només el cas feliç i oblidar la resposta d'error
- validar de manera massa decorativa o no validar res
- retornar una resposta que no es correspon amb la dada rebuda
- perdre el focus del projecte i acabar fent un exercici genèric sense relació amb el domini
- actualitzar el codi però no el `README`
- usar IA com a generador opac i no com a ajuda guiada i verificable

## Checkpoint de final de setmana

Al tancament de la setmana 2, cada alumne ha de poder mostrar i explicar:

- quin és el primer flux real que ha triat per al seu projecte
- quina dada entra al servidor
- on es veu el tractament d'eixa dada en el codi
- quina validació mínima s'ha aplicat
- com es distingix el cas correcte del cas incorrecte
- quina resposta retorna el servidor en cada cas
- per què encara no ha entrat en un framework complet
- com ha deixat traçabilitat individual i com ha usat la IA, si l'ha usada

## Materials que s'activen

- [setmana_01_guio_docent.md](setmana_01_guio_docent.md)
- [guia_sessio_a_sessio_20_setmanes.md](guia_sessio_a_sessio_20_setmanes.md)
- [kit_pilotatge_setmanes_01_04.md](kit_pilotatge_setmanes_01_04.md)
- [preparacio_docent_directa_curs_que_ve.md](preparacio_docent_directa_curs_que_ve.md)
- [briefing_inicial_curs.md](../08_materials_compartibles/briefing_inicial_curs.md)
- [full_treball_repte_01.md](../08_materials_compartibles/full_treball_repte_01.md)
- [guio_ús_ia_per_a_lalumnat.md](../08_materials_compartibles/guio_ús_ia_per_a_lalumnat.md)
- [formularis_i_validacio.md](../alumnat/consulta_tecnica/formularis_i_validacio.md)

## Definition of done del document

Este document es considera completat quan:

- baixa la setmana 2 a un nivell operatiu usable en aula
- deixa explícit que el focus és el comportament bàsic del backend en llenguatge real, encara sense framework pesat
- concreta què ha d'explicar el professorat, què ha de modelar i què ha de fer l'alumnat
- fixa evidències mínimes, criteris d'insuficiència, errors previsibles i checkpoint final
- manté coherència amb la setmana 1, amb la seqüència de `20` setmanes, amb el kit `1-4` i amb la preparació docent directa del curs
- manté visibles l'avaluació individual, la traçabilitat i l'ús guiat i verificable de la IA
