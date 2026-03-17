# Checklist de l'itinerari FastAPI

## Finalitat
Esta checklist servix per revisar si l'itinerari `FastAPI` ja disposa d'una base prou sòlida per aplicar-se al projecte del curs i adaptar-se després als Reptes 2, 3, 4 i 5 sense improvisació estructural.

## Contingut operatiu
La revisió final de l'itinerari no s'ha de limitar al fet que l'aplicació arranque. També ha de comprovar autenticació, persistència, validació, proves, documentació, `AI log` i capacitat real de continuar el projecte base sobre ecosistema Python.

Preparació per als Reptes 2-5:
- el tancament d'esta primera guia d'itinerari ha de deixar clar com es cobriran autenticació, persistència, API i integració híbrida dins de `FastAPI`
- també ha de deixar identificades les peces pròpies de l'ecosistema Python que funcionaran com a patró reusable i comparable amb els altres itineraris

## Errors habituals o riscos
- confondre "servidor arranca" amb "itinerari preparat"
- no distingir models persistents, esquemes i operacions
- mantindre punts crítics de negoci massa acoblats als `routers`
- dependre de snippets o de IA sense validació posterior

## Checklist final
### Projecte arranca correctament
- [ ] el projecte `FastAPI` arranca sense passos opacs o no documentats
- [ ] la configuració mínima d'entorn i dependències és reproduïble
- [ ] el `README` explica la posada en marxa real

### Autenticació funcional
- [ ] existix un flux funcional d'autenticació o estat equivalent defensable
- [ ] almenys una operació del domini està protegida
- [ ] l'equip pot explicar on es comprova autenticació i accés

### Persistència coherent
- [ ] hi ha model persistent mínim alineat amb el projecte base
- [ ] l'evolució d'esquema o persistència principal està definida i verificada
- [ ] les relacions bàsiques tenen sentit funcional i es poden defensar

### Validacions mínimes
- [ ] les dades d'entrada rellevants es validen amb criteri
- [ ] existix tractament mínim d'errors o de casos no vàlids
- [ ] la validació reflectix el comportament real del codi

### Documentació actualitzada
- [ ] el `README` o documentació tècnica reflectix l'estat real del projecte
- [ ] les decisions mínimes de stack queden escrites quan aporten mantenibilitat

### Proves mínimes
- [ ] hi ha almenys una verificació funcional del flux principal
- [ ] hi ha almenys una comprovació de fallada o dada invàlida
- [ ] el resultat deixa rastre revisable al repositori

### AI log si s'ha usat IA
- [ ] existix AI log o registre equivalent si s'ha utilitzat IA
- [ ] les propostes assistides han sigut executades, revisades o contrastades

### Preparació per adaptar-se als Reptes 2-5
- [ ] el stack està preparat per cobrir sessions i autenticació del Repte 2
- [ ] el projecte es pot reorganitzar o mantindre per capes clares al Repte 3
- [ ] la base és prou estable per exposar API al Repte 4
- [ ] l'itinerari deixa marge per a integració i automatització al Repte 5
