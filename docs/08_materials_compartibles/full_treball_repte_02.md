# Full de treball del Repte 2

## Objectiu
Convertir la primera peça funcional del producte en una operació de negoci protegida i verificable.

## Has de fer
- implementar alta/login/logout o estat equivalent
- definir un actor clar del domini
- protegir una operació real del producte
- provar accés autoritzat i accés denegat
- controlar almenys un error de validació o credencial
- actualitzar `README` amb com reproduir el flux

## Evidència mínima
- usuari o estat operatiu
- una operació del domini protegida
- prova del cas correcte
- prova del cas denegat o incorrecte
- resposta d'error interpretable
- `README` actualitzat

## Com ho valides
- crea o autentica un usuari de prova
- executa l'operació protegida amb accés vàlid
- torna a provar-la sense accés o amb estat invalidat
- mostra almenys un error rellevant
- ensenya com reproduir-ho des del `README`

## Errors habituals
- fer login però no protegir res útil
- protegir una ruta decorativa
- no diferenciar autenticació i autorització
- provar només el cas feliç
- no saber què passa després del logout

## Si et bloqueges
- treballa amb un únic actor i una sola operació protegida
- elimina extensions de rols fins que el flux principal estiga tancat
- revisa la [consulta tècnica sobre cookies, sessions i estat](../alumnat/consulta_tecnica/cookies_sessions_i_estat.md)
- revisa la [consulta tècnica sobre autenticació i autorització](../alumnat/consulta_tecnica/autenticacio_i_autoritzacio.md)

## Si acabes prompte
- afegeix una restricció simple de rol o permís
- reforça missatges d'error
- deixa una prova més clara del cas denegat
