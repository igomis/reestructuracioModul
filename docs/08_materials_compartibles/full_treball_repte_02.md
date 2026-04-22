# Full de treball del Repte 2

## Objectiu

Convertir la primera peça funcional del producte en una operació de negoci protegida i verificable sobre una base comuna en `PHP` i tancar-la amb una revisió final de mantenibilitat, organització en fitxers i un objecte mínim del domini.

## Has de fer

- tractar dades d'entrada al servidor amb criteri
- mostrar errors de validació de manera visible i permetre correcció
- ordenar la lògica bàsica del flux
- conservar la informació correcta amb un mecanisme simple i controlat
- reutilitzar després eixa informació dins del projecte
- implementar alta/login/logout o estat equivalent
- definir un actor clar del domini
- protegir una operació real del producte
- controlar tractament bàsic de fitxer o imatge si el flux ho necessita
- provar accés autoritzat i accés denegat
- controlar almenys un error de validació o credencial
- actualitzar `README` amb com reproduir el flux
- revisar el codi al final del repte
- netejar parts repetides o massa mesclades
- extraure funcions comunes a un fitxer separat quan es repetixen
- usar `include` / `require` o `include_once` / `require_once` amb sentit
- millorar funcions, noms o separació de dades i renderitzat
- representar almenys una entitat del projecte amb un objecte simple
- justificar per què la versió final és millor

En `R2` la persistència pot ser simple o, si cal, amb base de dades. El punt principal no és la sofisticació tècnica d'eixa persistència, sinó que el flux complet tinga sentit funcional.

## Sessió 7. Revisió final del codi

- revisa si hi ha barreja excessiva de `HTML + PHP`
- extrau funcions comunes quan ajuden a entendre millor el flux
- reparteix responsabilitats simples en fitxers i importa-les amb `include` / `require`
- millora noms i elimina duplicació clara
- separa millor preparació de dades i renderitzat si el teu codi ho demana
- crea almenys una entitat mínima del domini com a objecte simple
- justifica breument per què la versió final és més clara que la inicial

Esta sessió no vol dir “ara toca convertir-ho tot a objectes”, ni “ara toca fer `MVC`”, ni “ara toca passar-ho tot a base de dades”.

Si apareixen més classes, més objectes o una persistència més formal, han de quedar com a ampliació o pont cap al repte següent, no com a exigència central de `R2`.

## Evidència mínima

- usuari o estat operatiu
- una operació del domini protegida
- una dada correcta conservada i reutilitzable
- prova del cas correcte
- prova del cas denegat o incorrecte
- resposta d'error interpretable
- `README` actualitzat
- comparativa breu abans/després o justificació equivalent de la revisió final
- almenys un fitxer comú importat amb criteri i un objecte simple del domini

## Com ho valides

- crea o autentica un usuari de prova
- executa l'operació protegida amb accés vàlid
- comprova que la informació correcta es pot tornar a mostrar, recuperar o llistar
- torna a provar-la sense accés o amb estat invalidat
- mostra almenys un error rellevant
- ensenya com reproduir-ho des del `README`
- comprova que el flux continua funcionant després de la sessió `7`

## Errors habituals

- fer login però no protegir res útil
- quedar-se en formulari, validació i missatge d'error sense reutilitzar la dada bona
- protegir una ruta decorativa
- no diferenciar autenticació i autorització
- provar només el cas feliç
- complicar massa la persistència abans de tancar el flux principal
- no saber què passa després del logout
- convertir la sessió `7` en una reescriptura completa fora d'escala o en un “ara tot a objectes”

## Si et bloqueges

- treballa amb un únic actor i una sola operació protegida
- tria una dada del domini que després pugues recuperar o tornar a mostrar
- elimina extensions de rols fins que el flux principal estiga tancat
- no canvies encara de framework per intentar desbloquejar `R2`
- revisa la [consulta tècnica sobre cookies, sessions i estat](../alumnat/consulta_tecnica/cookies_sessions_i_estat.md)
- revisa la [consulta tècnica sobre autenticació i autorització](../alumnat/consulta_tecnica/autenticacio_i_autoritzacio.md)

## Si acabes prompte

- afegeix una restricció simple de rol o permís
- reforça missatges d'error
- deixa una prova més clara del cas denegat
- millora la revisió final amb una comparativa més clara del abans/després
