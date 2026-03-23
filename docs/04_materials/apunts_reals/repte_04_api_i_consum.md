# Apunts reals del Repte 4. API i consum

## Finalitat del document
Convertir el Repte 4 en un apunt de treball real, curt i executable, pensat perquè professorat i alumnat tinguen clara la seqüència mínima per publicar com a API una part rellevant del producte, documentar-la, provar-la i demostrar que pot ser consumida amb criteri professional.

Este repte no consistix a "fer endpoints" ni a "fer un CRUD perquè sí". El que s'espera és exposar com a API una funcionalitat real i usable del producte, amb contracte recognoscible, errors coherents, proves mínimes i consum verificable.

## Què sap ja l'alumnat
- ja té una funcionalitat real del producte reorganitzada en una estructura més mantenible
- ja treballa amb persistència funcional i amb un model de dades mínim recognoscible
- ja sap què és una evidència autèntica, com actualitzar el `README` i quan toca registrar un `AI log`
- ja té base prèvia de Git/GitHub; per tant, ací només es revisa com a metodologia de treball i traçabilitat, no com a iniciació

## Què s'ha de recordar breument
- el repte no consistix a obrir rutes, sinó a publicar una interfície usable del producte
- una `API` només compta si naix d'un cas d'ús real del domini i no d'un llistat arbitrari d'endpoints
- documentar no és descriure "més o menys" què fa el backend, sinó fixar el contracte que després s'ha de provar i consumir
- la IA pot ajudar a esbossar contractes, col·leccions o proves, però s'ha de poder justificar què s'ha verificat després

## Què ha d'explicar el professorat
- quin és el mínim exigible perquè una funcionalitat passe a ser una `API` usable
- per què no és suficient fer un `CRUD` genèric si no resol una part rellevant del producte
- com es relacionen recurs, endpoint, validació, codi d'estat, error i consum real
- per què este repte es tanca només si deixa preparada una base estable per a la integració híbrida del Repte 5

## Què s'ha de modelar en directe
- la selecció d'un recurs o cas d'ús real del domini que té sentit exposar com a `API`
- la definició d'un endpoint amb entrada, resposta correcta i error controlat
- una prova mínima d'un endpoint prioritari des d'una col·lecció, script o client simple
- un exemple curt de documentació coherent amb el comportament real de l'endpoint
- una defensa curta de per què el contracte publicat respon a una funcionalitat real i no a un `CRUD` ornamental
- una anotació breu al `README` o a l'`AI log` explicant una decisió de contracte o de prova

## Què treballa l'alumnat amb autonomia
- decidir quines funcionalitats del producte passen a `API` i quines encara no
- publicar endpoints prioritaris amb contracte clar i comportament coherent
- provar casos correctes i casos d'error rellevants
- preparar una evidència real de consum des d'un client, col·lecció o servei auxiliar
- actualitzar documentació, traçabilitat i registre d'ús de la IA si correspon

## Exemple mínim orientatiu
Exemple orientatiu de recorregut mínim:
1. Triar un cas d'ús del domini que ja funcione al backend, per exemple crear una incidència, consultar una reserva o recuperar un recurs intern.
2. Publicar com a `API` almenys una operació de consulta i una operació d'acció o escriptura amb sentit real.
3. Definir quins camps d'entrada són obligatoris, quina resposta correcta s'espera i quins errors mínims poden aparéixer.
4. Provar un cas correcte, un cas de validació incorrecta i un cas d'accés no permés o equivalent si toca.
5. Documentar com es prova l'endpoint i demostrar el consum real des d'una eina o client controlat.
6. Deixar identificat quin endpoint o recurs serà més útil per a la integració del Repte 5.

Criteri docent:
- l'exemple no s'ha de copiar literalment
- servix per entendre el mínim que s'ha de poder demostrar en qualsevol domini o stack
- el punt no és multiplicar rutes, sinó exposar una part real del producte de manera usable per tercers

## Errors habituals
- convertir el repte en una pràctica de "fer endpoints" sense relació clara amb el producte
- publicar un `CRUD` genèric sense prioritzar quina funcionalitat té valor real
- documentar una `API` que no coincidix amb el comportament real del backend
- provar només el cas feliç i no deixar rastre de validacions o errors
- confondre una captura puntual amb una evidència reproduïble de consum
- acceptar contractes, `Swagger` o col·leccions generades amb IA sense contrastar-les amb l'execució real

## Com es verifica que funciona
Per donar el repte per verificat, cal poder demostrar com a mínim:
- existixen endpoints prioritaris associats a un cas d'ús real del producte
- hi ha almenys una operació de consulta i una operació d'acció o escriptura amb sentit dins del domini
- el contracte d'entrada i eixida és recognoscible i coherent
- el sistema respon amb criteri mínim en casos correctes, de validació incorrecta i d'accés o recurs problemàtic quan toca
- hi ha una evidència real de consum des d'una eina, col·lecció, script o client simple
- la documentació descriu allò que realment fa l'API i deixa la base preparada per al Repte 5

Formats de verificació acceptables:
- col·lecció Postman o Insomnia
- fitxer de peticions `curl` o equivalent
- script de prova simple
- revisió docent amb backend obert, documentació visible i consum reproduïble

## Evidències que s'han d'entregar
- repositori amb traçabilitat recognoscible del pas de backend intern a `API` publicada
- `README` actualitzat amb com provar o consumir el Repte 4
- documentació d'`API` alineada amb el comportament real del backend
- col·lecció de proves o equivalent amb casos correctes i casos d'error
- evidència d'un consum real d'una funcionalitat significativa del producte
- `AI log` si s'ha utilitzat IA en contractes, proves, col·leccions, clients o debugging

## Checklist final del repte
- [ ] existixen endpoints prioritaris lligats a una funcionalitat real del producte
- [ ] hi ha almenys una operació de consulta i una operació d'acció o escriptura amb valor funcional clar
- [ ] el contracte d'entrada i eixida és coherent i recognoscible
- [ ] hi ha validacions, codis d'estat i errors mínims justificables
- [ ] existix almenys una prova o col·lecció reutilitzable dels endpoints principals
- [ ] existix una evidència real de consum de l'`API`
- [ ] el `README` explica com reproduir el Repte 4 i com provar l'`API`
- [ ] l'ús de la IA, si existix, està registrat i contrastat

## Connexió amb el Repte 5
El Repte 4 no queda tancat només quan "respon JSON", sinó quan deixa una `API` prou clara i estable per entrar en un flux híbrid. En concret, hauria de deixar identificat:
- quins endpoints o recursos seran més útils per a integració externa o automatització
- quins errors i prerequisits s'han de tindre en compte quan un consumidor extern use l'`API`
- quina part del contracte ja és prou estable per ser reutilitzada al Repte 5

Lectura de transició:
- si el Repte 4 deixa una `API` realment usable i provada, el Repte 5 pot centrar-se en integració i manteniment
- si el Repte 4 només obri rutes o fa un `CRUD` ornamental, el Repte 5 naixerà sobre una interfície feble o poc fiable
