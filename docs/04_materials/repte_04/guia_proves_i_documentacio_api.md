# Guia de proves i documentació d'API

## Finalitat

Assegurar que el Repte 4 no es tanque només amb endpoints aparentment funcionals, sinó amb una API provada, documentada i revisable per altres persones o serveis.

Esta guia s'ha d'usar per decidir què s'ha de provar, quina col·lecció mínima d'evidències s'ha d'aportar i quina documentació és exigible perquè l'API siga realment usable dins del curs.

## Què s'ha de provar en una API del curs

Com a mínim, s'han de provar:

- els endpoints principals del repte
- almenys un cas correcte per cada endpoint prioritari
- almenys un cas d'error rellevant: validació, autenticació, recurs inexistent o accés no permés
- coherència del contracte entre petició, resposta i codi d'estat
- el consum real des d'una eina, col·lecció o client de prova

Criteri pràctic:

- importa més la traçabilitat i la reproduïbilitat de la prova que no el volum brut de peticions
- la prova ha d'estar lligada al contracte publicat, no a supòsits implícits de l'equip
- el resultat s'ha de poder revisar sense dependre d'una demo improvisada

## Col·lecció mínima de proves

Una col·lecció mínima del Repte 4 hauria d'incloure:

- petició correcta a un endpoint principal de lectura
- petició correcta a un endpoint principal d'escriptura o acció
- cas de validació incorrecta
- cas de credencial o accés incorrecte si hi ha autenticació
- cas de recurs no trobat o equivalent quan tinga sentit

Formats acceptables:

- col·lecció Postman o Insomnia
- fitxer de peticions `curl` o equivalent
- script de prova simple
- registre equivalent si és reproduïble i està alineat amb l'stack

## Documentació mínima exigible

La documentació mínima de l'API ha d'incloure:

- llistat d'endpoints prioritaris
- mètodes HTTP i ruta
- autenticació o prerequisits si n'hi ha
- camps d'entrada principals
- estructura bàsica de resposta correcta
- errors previsibles i codis d'estat rellevants
- instruccions mínimes per provar l'API

La documentació pot estar en:

- `README`
- document específic d'API
- col·lecció anotada o especificació equivalent

## Evidències a aportar

S'espera trobar evidències com:

- col·lecció o conjunt de proves executable
- proves registrades de casos correctes i d'error
- documentació alineada amb el comportament real
- commits que mostren ajustos de contracte, resposta o validació
- demostració o rastre de consum real de l'API
- AI log si la IA ha ajudat a redactar contractes, proves, col·leccions o clients de consum

## Errors habituals

- limitar-se a una única prova del cas feliç
- documentar l'API després de codificar sense revisar si coincidix amb el comportament real
- presentar captures soltes sense col·lecció reproductible
- provar l'API manualment però sense deixar evidència reutilitzable
- considerar "documentada" una API només perquè existixen noms de rutes al codi
- usar IA per generar documentació o proves sense validar que corresponen als endpoints reals

## Checklist final

- existix una col·lecció mínima de proves dels endpoints prioritaris
- hi ha casos correctes i casos d'error provats
- la documentació descriu rutes, entrades, respostes i errors rellevants
- qualsevol persona de l'equip podria provar l'API seguint la documentació
- les evidències de prova són reutilitzables i no depenen només d'una demo puntual
- el paquet actual deixa la base preparada per a consum i integració al Repte 5
