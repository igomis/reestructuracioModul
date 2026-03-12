# Projecte backend base del curs

## Finalitat del document
Definir una guia operativa del producte tècnic evolutiu del mòdul DWES que servisca de base comuna per als reptes del curs i per als projectes tècnics futurs, sense tancar encara l’arquitectura d’un domini concret.

## Per què cal un producte base comú
- evita que cada repte es convertisca en un exercici aïllat sense continuïtat tècnica
- facilita traçabilitat d’evidències i comparabilitat d’avaluació entre equips i itineraris
- permet connectar materials, enunciats i criteris de qualitat sobre un mateix producte viu
- prepara una transició coherent cap als Reptes 3, 4 i 5, on augmenta la complexitat arquitectònica, API i integració
- reduïx dispersió docent i ajuda a focalitzar decisions tècniques realment rellevants

## Principis de disseny del projecte base
- un únic producte backend evolutiu al llarg dels Reptes 1-5
- enfocament professional realista: traçabilitat, proves, documentació i manteniment
- comparabilitat docent: mateixos criteris d’avaluació, independentment de la stack
- creixement incremental: cada repte amplia el producte anterior
- neutralitat de domini: el valor didàctic depén dels requisits tècnics, no del sector escollit

## Criteris que ha de complir qualsevol domini de projecte
Qualsevol domini triat ha de permetre, com a mínim:
- backend real amb casos d’ús de negoci no trivials
- persistència de dades i evolució de model
- API documentada i consumible
- autenticació i control bàsic d’accés
- proves tècniques (funcionals i/o integració) amb evidència executada
- documentació operativa del projecte (README, decisions tècniques i API docs)
- integracions amb serveis externs o fluxos híbrids
- manteniment evolutiu (correccions, millores, regressió i traçabilitat)

Si un domini no permet cobrir estos punts amb càrrega docent raonable, no és apte com a projecte base.

## Dominis de projecte proposats
1. **Gestor d’incidències / tickets**
Objectiu docent: modelar cicle de vida d’incidències, priorització, assignació i seguiment.
Punts forts: facilita autenticació per rols, API de consulta/actualització i manteniment amb historial de canvis.

2. **Sistema de reserves / cites**
Objectiu docent: gestionar disponibilitat, calendari, conflictes i confirmacions.
Punts forts: força validacions de negoci, control d’estat i integracions de notificació.

3. **Gestor intern de recursos / inventari**
Objectiu docent: controlar altes/baixes, moviments, estat i disponibilitat de recursos.
Punts forts: bona base per persistència, API de consulta operativa i auditories de manteniment.

## Components comuns mínims del producte
- model d’usuaris amb autenticació i rols mínims
- entitats de domini i regles de negoci principals
- capa de persistència amb accés segur a dades
- API per a operacions clau del sistema
- bateria mínima de proves i registre de validació
- documentació tècnica executable i coherent amb el codi
- mecanisme d’integració externa (API externa, webhook o automatització)
- pauta de manteniment: incidències, correccions i evidència de millores

## Relació amb els reptes del curs
| Repte | Aportació del projecte base |
|---|---|
| Repte 1. Kickoff tècnic | Definir repositori, entorn, convencions i ADR del producte backend comú. |
| Repte 2. Sessions i autenticació | Implementar usuaris/sessions sobre el domini seleccionat amb evidència funcional. |
| Repte 3. MVC i persistència | Reestructurar el producte a arquitectura mantenible i consolidar model de dades. |
| Repte 4. API i consum | Exposar funcionalitats del domini via API i validar consum amb contractes clars. |
| Repte 5. Integració híbrida i manteniment | Connectar serveis externs/automatització i demostrar manteniment evolutiu del producte. |

## Compatibilitat amb els itineraris tecnològics
El projecte base s’ha de poder desplegar en qualsevol itinerari autoritzat:
- PHP + Laravel
- Node.js + Express o Nest
- Python + FastAPI

La compatibilitat implica equivalència d’objectius, evidències i criteris d’avaluació, no uniformitat d’implementació interna.

## Paper de la IA
La IA és una eina habitual de suport per explorar arquitectura, accelerar esquelets, depurar errors i millorar documentació.

Condició obligatòria:
- tota aportació assistida s’ha de validar amb proves/execució real
- l’alumnat ha de poder justificar i defensar les decisions tècniques

## Línia futura de projectes relacionats amb tokenització
Es deixa oberta una línia futura per incorporar mecanismes de tokenització en context backend (p. ex. tokens d’accés, invitació o traçabilitat), sempre amb enfocament docent i verificable.

Esta línia no desplega encara un projecte complet ni tanca decisions d’arquitectura.

## Decisió provisional recomanada
Per iniciar la consolidació del model, es recomana prioritzar com a domini pilot el **gestor d’incidències / tickets**, perquè facilita cobrir de manera equilibrada autenticació, persistència, API, integracions i manteniment.

La decisió és provisional: es manté oberta la possibilitat d’adoptar reserves/cites o inventari si el centre o l’equip docent ho considera més adequat, sempre complint els criteris comuns d’este document.

## Definition of done del document
Este document es considera completat quan:
- defineix un marc operatiu del projecte backend base sense tancar encara un projecte únic
- explicita criteris mínims de domini compatibles amb Reptes 1-5
- incorpora almenys tres dominis viables i comparables en clau docent
- assegura compatibilitat amb PHP+Laravel, Node.js+Express/Nest i Python+FastAPI
- fixa el paper de la IA com a suport verificable
- deixa registrada la línia futura de tokenització com a evolució posterior
- queda preparat per servir de base als Reptes 3-5 i als futurs materials/enunciats
