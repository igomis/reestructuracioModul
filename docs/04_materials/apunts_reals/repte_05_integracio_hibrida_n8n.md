# Apunts reals del Repte 5. Integració híbrida, automatització i tancament

## Finalitat del document

Convertir el Repte 5 en un apunt de treball real, curt i executable, pensat perquè professorat i alumnat tinguen clara la seqüència mínima per tancar el producte del curs amb una integració, una automatització o un flux híbrid que aporte valor real i es puga provar, mantindre i defensar.

Este repte no consistix a "usar `n8n`" ni a "fer una automatització perquè sí". El que s'espera és resoldre una necessitat real del producte amb una integració o orquestració útil, basada en l'`API` publicada, amb recorregut complet de dades, tractament mínim d'errors i tancament professional del projecte.

## Què sap ja l'alumnat

- ja té una part rellevant del producte publicada com a `API` i consumida amb contracte recognoscible
- ja sap què és una evidència autèntica, com actualitzar el `README` i quan toca registrar un `AI log`
- ja ha treballat proves, errors i documentació tècnica operativa en els reptes anteriors
- ja té base prèvia de Git/GitHub; per tant, ací només es revisa com a metodologia de treball i traçabilitat, no com a iniciació

## Què s'ha de recordar breument

- el repte no consistix a construir un workflow vistós, sinó a completar un procés real del producte
- `n8n` o una eina equivalent només tenen sentit si aporten claredat, valor funcional i mantenibilitat
- una integració només compta si es pot provar tant en camí correcte com en camí de fallada
- el valor docent està en el procés resolt, no en l'eina triada
- la IA pot ajudar a mapar payloads, passos o errors, però s'ha de poder explicar què s'ha acceptat i com s'ha verificat després

## Què ha d'explicar el professorat

- quin és el mínim exigible perquè una integració o automatització tinga valor real dins del projecte
- per què no és suficient fer una crida externa ornamental o una demo visual de `n8n`
- com es relacionen `API`, trigger, transformació, eixida, tractament d'errors i manteniment
- per què este repte es tanca només si deixa el producte defensable de punta a punta i preparat per a la defensa final

## Què s'ha de modelar en directe

- la selecció d'un cas d'ús del domini que tinga sentit integrar o automatitzar
- l'esquema d'un flux híbrid mínim amb entrada, consum d'`API`, transformació i eixida clara
- una prova curta del flux complet amb almenys un punt de fallada controlat
- una anotació breu al `README` o a l'`AI log` explicant una decisió d'integració, d'error o de manteniment
- una defensa curta de per què el flux triat aporta valor real al producte i no només efecte visual

## Què treballa l'alumnat amb autonomia

- decidir quina necessitat real del producte es tanca amb una integració o automatització
- construir el workflow en `n8n` o amb una eina equivalent si està justificada
- connectar el flux amb l'`API` pròpia i amb el servei extern, webhook o eixida final que corresponga
- provar el recorregut complet, incloent almenys un cas de fallada rellevant
- documentar el flux, els punts crítics, el manteniment i el rastre d'ús de la IA si hi correspon

## Exemple mínim orientatiu

Exemple orientatiu de recorregut mínim:

1. Triar un esdeveniment real del producte, per exemple una incidència nova, una reserva confirmada o un canvi rellevant d'estat d'un recurs.
2. Consumir l'`API` pròpia per recuperar o enviar la informació necessària.
3. Transformar o validar dades mínimes abans de reenviar-les a un servei extern, una notificació o un registre automatitzat.
4. Generar una eixida observable, per exemple una notificació, un registre, una sincronització o una acció posterior.
5. Provar un cas correcte i un cas de fallada de `API`, de servei extern o de dada invàlida.
6. Deixar clar com s'explica i es defensa el flux complet al tancament del producte.

Criteri docent:

- l'exemple no s'ha de copiar literalment
- servix per entendre el mínim que s'ha de poder demostrar en qualsevol domini o stack
- el punt no és usar una eina concreta, sinó tancar un procés recognoscible del producte amb integració i manteniment bàsics

## Errors habituals

- convertir el repte en una pràctica de "fer `n8n`" sense necessitat real del producte
- triar una integració només perquè és fàcil de mostrar, no perquè resolga res rellevant
- no definir clarament quina dada entra, quina es transforma i quina ix
- provar només el cas feliç i no deixar rastre de fallades o incidències
- duplicar lògica de negoci al workflow en lloc de reutilitzar l'`API` i el backend
- acceptar workflows, nodes o configuracions suggerides amb IA sense contrastar l'execució real

## Com es verifica que funciona

Per donar el repte per verificat, cal poder demostrar com a mínim:

- existix una integració o flux híbrid lligat a una necessitat real del producte
- el flux reutilitza l'`API` pròpia com a contracte central i no com a element decoratiu
- hi ha una eixida observable i una traça mínima del recorregut complet
- s'ha provat almenys un cas correcte i un cas de fallada rellevant
- el flux és prou clar per explicar què inicia el procés, quines dades es mouen i què passa si falla
- el producte queda preparat per a una defensa final tècnica amb criteri de manteniment

Formats de verificació acceptables:

- workflow exportat o artefacte equivalent
- registre d'execució o evidència reproduïble del flux
- prova manual guiada amb backend, `API` i integració oberts
- revisió docent amb documentació visible, traçabilitat i defensa tècnica del procés complet

## Evidències que s'han d'entregar

- repositori amb traçabilitat recognoscible del tancament integrat del producte
- `README` actualitzat amb com reproduir o provar el flux híbrid del Repte 5
- workflow exportat o descrit de forma reproduïble, amb els punts crítics del procés
- evidència d'integració real entre `API` pròpia i servei extern, webhook o eixida equivalent
- prova o registre de funcionament correcte i de fallada rellevant
- `AI log` si s'ha utilitzat IA en disseny del flux, mapping de payloads, debugging o configuració

## Checklist final del repte

- [ ] existix una integració o flux híbrid lligat a una necessitat real del producte
- [ ] el flux reutilitza l'`API` pròpia com a peça central
- [ ] hi ha una eixida observable i una traça mínima del recorregut complet
- [ ] s'ha provat almenys un cas correcte i un cas de fallada rellevant
- [ ] el workflow o l'eina triada està documentat de manera reproduïble
- [ ] el `README` explica com reproduir el Repte 5 o com revisar el flux
- [ ] la defensa final pot recolzar-se en evidències clares del procés i del seu manteniment
- [ ] l'ús de la IA, si existix, està registrat i contrastat

## Connexió amb el tancament del producte o amb la defensa final

El Repte 5 no queda tancat només quan "fa una automatització", sinó quan deixa el producte del curs en un estat defensable com a sistema complet. En concret, hauria de deixar clar:

- quin problema real del producte resol la integració triada
- quins punts del flux han sigut més delicats i com s'han controlat
- quines evidències permeten defensar autoria, funcionament i manteniment del sistema

Lectura de tancament:

- si el Repte 5 deixa una integració útil, provada i explicable, el producte queda llest per a la defensa final
- si el Repte 5 només aporta una automatització ornamental o difícil de reproduir, el tancament del curs queda feble encara que el workflow "es veja"
