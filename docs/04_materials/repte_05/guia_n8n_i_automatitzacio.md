# Guia de n8n i automatització

## Finalitat
Donar una base mínima perquè `n8n`, o una eina equivalent, s'use al Repte 5 com a infraestructura d'orquestració amb criteri tècnic, i no només com a suport visual per a una demo.

Esta guia servix per decidir quan compensa usar `n8n`, com ha de ser un workflow mínim usable i quines evidències s'han de deixar perquè el procés siga verificable i mantingut.

## Quan usar n8n dins del projecte
Convé usar `n8n` quan:
- hi ha un flux amb diversos passos o sistemes implicats
- cal consumir l'API pròpia i reenviar dades a un altre servei
- el procés guanya claredat si es representa com a workflow
- l'orquestració aporta més valor que un simple script puntual

No cal forçar `n8n` si:
- el cas d'ús és més simple i un script o integració directa és suficient
- el workflow no aporta res més que aparença visual
- l'equip no pot explicar què fa cada node ni què passa quan el flux falla

## Estructura mínima d'un workflow usable
Un workflow usable del Repte 5 hauria de tindre:
- un desencadenant recognoscible: webhook, crida manual, polling o esdeveniment equivalent
- una crida a l'API pròpia del curs o recepció de dades des d'ella
- una transformació o validació mínima si cal
- una eixida clara: servei extern, notificació, registre o acció final
- almenys un punt de control d'error o de diagnòstic

El workflow ha de permetre respondre:
- què inicia el procés
- quines dades es mouen entre passos
- quina part depén de l'API del curs
- què es considera èxit
- què es considera fallada

## Nodes o passos habituals
Segons el cas triat, és habitual trobar:
- node de trigger o webhook
- node HTTP Request per consumir o cridar l'API pròpia
- node de transformació o mapping de dades
- node de validació o decisió condicional
- node de crida a servei extern
- node de registre, notificació o eixida final

Criteri pràctic:
- cada node ha de tindre una funció clara
- si dos passos poden simplificar-se sense perdre claredat, convé fer-ho
- si un node és crític per al flux, ha d'estar explicat en documentació o defensa

## Validació del flux i traçabilitat
La validació mínima d'un workflow ha d'incloure:
- execució correcta de punta a punta
- comprovació del payload d'entrada i del resultat final
- almenys una fallada reproduïda: API, servei extern, dades incorrectes o pas intermedi
- registre o evidència de com s'ha detectat i corregit la incidència

Traçabilitat mínima recomanada:
- export del workflow o artefacte equivalent
- descripció del flux i dels nodes principals
- captura o registre d'execució quan aporte context
- correspondència clara entre workflow, API i cas d'ús del domini

## Riscos habituals d'automatització
- crear workflows massa visuals però poc comprensibles
- dependre de credencials, webhooks o configuracions no documentades
- no controlar respostes inesperades o errors intermedis
- duplicar lògica de negoci dins del workflow en lloc de deixar-la al backend
- no poder reproduir el flux fora de la demo puntual
- acceptar configuracions suggerides per IA sense contrastar l'execució real

## Evidències esperades
S'espera trobar evidències com:
- workflow exportat o descrit de manera reproduïble
- integració real amb l'API del curs
- prova d'execució correcta i d'error rellevant
- documentació dels nodes o passos crítics
- registre de manteniment o troubleshooting
- AI log si la IA ha ajudat a dissenyar nodes, transformacions o estratègies d'error

## Checklist final
- `n8n` o l'eina equivalent s'ha triat perquè aporta valor al cas d'ús
- el workflow té un trigger recognoscible, consum d'API i eixida clara
- hi ha almenys una validació de flux correcte i una de fallada
- el workflow deixa rastre suficient per ser revisat i reproduït
- l'automatització és comprensible, documentada i defensable
- el resultat reforça el tancament professional del Repte 5 i no una demo ornamental
