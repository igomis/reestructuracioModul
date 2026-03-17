# Checklist del Repte 3

## Ús de la checklist
Esta checklist servix per revisar si el Repte 3 ja ha convertit el backend funcional dels reptes anteriors en una base mantenible, persistent i prou estable per obrir-se després a API.

## Arquitectura per capes o equivalent
- [ ] existix separació recognoscible entre entrada, negoci i persistència
- [ ] el controlador o equivalent no concentra tota la lògica del flux
- [ ] almenys un cas d'ús clau està migrat completament a l'estructura nova
- [ ] l'arquitectura adoptada és coherent amb l'itinerari tecnològic triat

## Persistència funcional i coherent
- [ ] el domini disposa de model de dades mínim persistent
- [ ] les operacions prioritàries llegixen i escriuen dades de manera coherent
- [ ] hi ha tractament bàsic de recursos inexistents o d'estats no vàlids
- [ ] la capa de persistència no està barrejada críticament amb resposta o presentació

## Validacions i errors mínims
- [ ] les validacions rellevants no queden només al punt d'entrada
- [ ] es diferencien almenys errors de validació, de negoci i de dades quan toque
- [ ] el comportament d'error és coherent i reproduïble

## Proves mínimes
- [ ] existix almenys una prova o verificació del flux principal després de la refactorització
- [ ] existix almenys una comprovació sobre persistència o cas de dada invàlida
- [ ] una correcció rellevant deixa rastre de verificació posterior

## Documentació actualitzada
- [ ] el `README` o documentació tècnica explica l'estat actual de l'arquitectura
- [ ] les decisions importants de refactorització o persistència estan registrades

## AI log si s'ha usat IA
- [ ] existix AI log o registre equivalent si s'ha utilitzat IA
- [ ] l'ús de IA queda validat amb execució, prova o revisió tècnica

## Preparació per al Repte 4
- [ ] la base actual es pot exposar com a API sense reorganització crítica addicional
- [ ] estan identificats els casos d'ús que passen millor a endpoint
- [ ] el model i la persistència són prou clars per documentar contractes API després
