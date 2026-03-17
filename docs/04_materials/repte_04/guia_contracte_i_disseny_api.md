# Guia de contracte i disseny d'API

## Finalitat
Convertir el Repte 4 en una publicació d'API clara, usable i defensable, on el contracte no siga una descripció posterior del que "més o menys fa" el backend, sinó una definició operativa del que un consumidor pot esperar.

Esta guia servix per decidir què s'exposa, com s'anomena, quines regles mínimes governen peticions i respostes, i com mantindre coherència entre l'API publicada i el producte real del curs.

## Què és un contracte API mínim usable
Un contracte API mínim usable ha de deixar clar:
- quins recursos o casos d'ús del producte s'exposen
- quins endpoints existixen per a cada recurs
- quin mètode HTTP s'espera en cada operació
- quines dades d'entrada són necessàries o opcionals
- quina resposta s'ha d'esperar quan l'operació és correcta
- quins errors previsibles poden aparéixer i com s'expressen
- si l'endpoint requerix autenticació o control d'accés

Criteri pràctic:
- el contracte ha de nàixer dels casos d'ús prioritaris del producte, no d'una llista arbitrària de rutes
- l'API del Repte 4 no ha d'exposar-ho tot, però allò que expose ha d'estar ben resolt
- la documentació d'API ha de correspondre exactament amb el comportament real de l'endpoint

## Recursos, endpoints i operacions mínimes
Un mínim usable del Repte 4 hauria d'incloure:
- un recurs principal del domini del projecte
- almenys una operació de consulta
- almenys una operació de creació o actualització, segons tinga sentit al domini
- almenys un endpoint protegit si el domini exigix autenticació

Exemples d'operacions mínimes:
- llistar o consultar un recurs principal
- crear un recurs principal
- consultar el detall d'un element concret
- modificar un estat o una dada clau si forma part del flux prioritari

Criteri de disseny:
- usar noms consistents per a recursos i rutes
- evitar mesclar accions de negoci i noms tècnics confusos en el mateix endpoint
- mantindre una correspondència clara entre el model intern i la resposta exposada
- no publicar endpoints que encara no es poden provar ni mantindre

## Criteris de coherència de respostes, codis d'estat i errors
L'API ha de mantindre coherència com a mínim en estos punts:
- format de resposta recognoscible entre endpoints similars
- codis d'estat justificables segons el resultat de l'operació
- missatges o estructures d'error comprensibles
- diferència visible entre error de validació, error d'autenticació, absència de recurs i error intern
- resposta alineada amb el contracte documentat

Mínim exigible:
- casos correctes amb resposta estable
- errors de validació amb resposta identificable
- errors d'accés amb comportament coherent
- absència de codis d'estat posats per costum sense justificació real

## Errors habituals
- documentar endpoints que no existixen o que no responen com s'ha escrit
- dissenyar rutes sense relació clara amb els recursos del domini
- retornar estructures diferents per al mateix tipus d'operació sense motiu
- usar codis d'estat incoherents o intercanviables
- exposar lògica interna o noms de persistència en lloc d'un contracte pensat per a consum extern
- acceptar esborranys d'OpenAPI o dissenys suggerits per IA sense contrastar-los amb el backend real

## Checklist final
- existix almenys un recurs principal exposat com a API
- hi ha endpoints prioritaris prou clars per a consulta i operació principal
- el contracte d'entrada i eixida és recognoscible i coherent
- els codis d'estat i errors tenen criteri tècnic i no són arbitraris
- la documentació d'API reflectix el comportament real del backend
- l'API resultant és prou clara per preparar el consum i la integració del Repte 5
