# Full de treball del Repte 2

## Objectiu

Convertir la primera peça funcional del producte en una operació de negoci protegida i verificable sobre una base comuna en `PHP` i tancar-la amb una primera peça testable amb POO, Composer i prova unitària.

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
- crear o ajustar `composer.json`
- configurar autoload per a classes pròpies
- crear una classe simple del domini o servei
- escriure una prova unitària mínima
- comprovar que el flux web continua funcionant
- justificar què queda ara més testable

En `R2` la persistència pot ser simple o, si cal, amb base de dades. El punt principal no és la sofisticació tècnica d'eixa persistència, sinó que el flux complet tinga sentit funcional.

## Sessió 7. Primera peça testable

- tria una regla, comprovació o càlcul del flux ja provat
- crea una classe simple en `src/` o carpeta equivalent
- carrega-la amb Composer/autoload
- escriu una prova unitària mínima amb `PHPUnit`, `Pest` o script equivalent
- executa la prova i documenta el resultat
- repeteix un cas clau del flux web

Esta sessió no vol dir “ara toca convertir-ho tot a objectes”, ni “ara toca fer `MVC`”, ni “ara toca passar-ho tot a base de dades”.

Si apareixen més classes, una llibreria externa o una API, han de quedar com a ampliació o pont cap als reptes següents, no com a exigència central de `R2`.

## Evidència mínima

- usuari o estat operatiu
- una operació del domini protegida
- una dada correcta conservada i reutilitzable
- prova del cas correcte
- prova del cas denegat o incorrecte
- resposta d'error interpretable
- `README` actualitzat
- `composer.json` o equivalent amb autoload
- classe simple del domini o servei
- prova unitària mínima executada

## Targeta fixa de traçabilitat

- **Criteri/objectiu**: `RA2`, `RA3` i `RA4`, flux funcional protegit.
- **Descriptor de rúbrica**: cas d'ús no trivial, verificació tècnica i defensa d'autoria.
- **Moment d'avaluació**: checkpoint funcional i revisió final del codi.
- **Agent d'avaluació**: professorat amb prova guiada de l'alumne.
- **Tipus d'evidència**: flux, proves, errors, `README` i justificació abans/després.

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
