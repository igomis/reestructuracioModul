# Projecte backend base del curs

## Finalitat del document

Definir el marc operatiu del projecte backend base del curs perquè funcione com a producte tècnic evolutiu, útil per a la planificació docent i per a la generació d’evidències reals d’aprenentatge.

## Funció del document dins del projecte docent

Este document fixa una base comuna abans de tancar nous enunciats i materials.
La seua funció és:

- establir què s’entén per projecte backend base en el mòdul
- assegurar coherència entre reptes, avaluació i materials
- facilitar que els Reptes 3, 4 i 5 es redacten sobre un producte comú i no sobre activitats aïllades
- permetre comparabilitat de resultats entre itineraris tecnològics diferents

Lectura metodològica vinculada:

- `R2` consolida el producte sobre una base comuna en `PHP`
- `R3-R5` obrin el contrast de frameworks sobre el mateix projecte
- la cooperació pot existir, però la implementació acreditable continua sent individual

## Principis de disseny del projecte base

- producte evolutiu únic durant el curs, amb creixement incremental per reptes
- no trivialitat funcional: cada repte ha d’aportar una funcionalitat professional mínima del producte, no una tècnica aïllada
- orientació professional: qualitat de codi, proves, documentació i manteniment
- neutralitat de domini: importa la cobertura tècnica, no el sector triat
- verificabilitat: cada avanç ha de tindre evidència executable al repositori
- independència d’stack: mateixos objectius docents amb tecnologies diferents

## Requisits mínims comuns

Qualsevol domini triat per al projecte base ha de permetre, de manera obligatòria:

- backend real amb casos d’ús no trivials
- persistència de dades i evolució del model
- API publicada i consumible
- autenticació i control d’accés bàsic
- proves automatitzades (unitàries, integració o equivalents)
- documentació tècnica operativa (README, decisions i contractes API)
- integracions amb serveis externs o fluxos híbrids
- manteniment evolutiu (correccions, millores, regressions i traçabilitat)

Si un domini no permet cobrir estes huit dimensions, no és apte com a projecte base.

Criteri transversal obligatori:

- cap repte es considera resolt si només aporta una tècnica solta, una demo ornamental o un esquelet sense valor funcional
- cada fase del curs ha de professionalitzar una part recognoscible del mateix producte

## Dominis de projecte proposats

1. **Gestor d’incidències / tickets**
Permet modelar estats, prioritats, assignacions i historial. És un domini equilibrat per treballar autenticació, API, persistència i manteniment amb incidències reals.

2. **Sistema de reserves / cites**
Permet tractar disponibilitat, conflictes i validacions de negoci. És adequat per a API, persistència temporal, integracions de notificació i proves funcionals.

3. **Gestor intern de recursos / inventari**
Permet controlar altes, baixes, moviments i disponibilitat. És útil per a traçabilitat, manteniment i integració amb processos interns.

Els tres dominis són vàlids sempre que cobrisquen els requisits mínims comuns i es puguen mantenir amb càrrega docent realista.

## Components comuns del producte

Sense definir encara una arquitectura tancada, el projecte base ha d’incorporar:

- primera peça funcional d’entrada al producte (landing page o equivalent, captura de dades i primera traçabilitat)
- model d’usuaris i mecanisme d’autenticació
- primera funcionalitat de negoci autenticada amb rols o restriccions
- model de domini i regles de negoci principals
- capa de persistència i gestió de dades
- API per a les operacions clau del sistema
- conjunt mínim de proves automatitzades
- documentació tècnica de posada en marxa i ús
- punt d’integració externa (API externa, webhook o automatització)
- criteri de manteniment i registre d’evolució

## Relació amb els reptes del curs

| Repte | Connexió amb el projecte backend base |
|---|---|
| Repte 1. Kickoff funcional | Arrancada funcional del producte: repositori, decisió tècnica i primera peça real d’entrada amb captura de dades. |
| Repte 2. Sessions, autenticació i primera funcionalitat de negoci | Primera funcionalitat de negoci autenticada, amb control d’accés i restriccions recognoscibles del domini. |
| Repte 3. MVC i persistència | Professionalització d’eixa funcionalitat amb arquitectura mantenible, persistència i proves mínimes. |
| Repte 4. API i consum | Publicació i consum d’API sobre casos d’ús reals del producte, no sobre rutes aïllades. |
| Repte 5. Integració híbrida i manteniment | Integració externa del mateix producte i demostració de manteniment evolutiu amb un flux complet. |

Este encaix converteix el projecte base en referència directa per als enunciats i materials dels Reptes 3-5.

## Compatibilitat amb els itineraris tecnològics

El projecte backend base ha de ser compatible amb:

- Laravel
- Symfony
- NestJS

La compatibilitat exigida és de resultats i evidències, no d’implementació interna idèntica.

`FastAPI` només s'hauria d'obrir com a via avançada o excepcional.

## Paper de la IA

La IA s’assumeix com a eina habitual de suport (ideació tècnica, prototipat, depuració i documentació), però mai com a substitut de validació.

Condicions docents mínimes:

- tota aportació assistida per IA s’ha de verificar amb execució real, proves i revisió de codi
- l’equip ha de poder explicar i defensar les decisions tècniques adoptades

## Línia futura relacionada amb tokenització

Es deixa oberta una línia futura per estudiar mecanismes de tokenització en context backend (per exemple, tokens d’accés, invitació o traçabilitat), com a extensió del producte base.

Esta línia queda intencionadament oberta: no es defineix ara un projecte complet ni una arquitectura específica de tokenització.

## Decisió provisional recomanada

Es recomana començar amb el domini **gestor d’incidències / tickets** com a opció provisional prioritària, perquè facilita cobrir de manera equilibrada autenticació, persistència, API, integracions i manteniment.

La decisió no és tancada. Es poden adoptar **sistema de reserves / cites** o **gestor intern de recursos / inventari** si mantenen els mateixos requisits mínims comuns i la mateixa traçabilitat docent.

## Definition of done del document

Este document es considera completat quan:

- defineix un marc operatiu clar del projecte backend base del curs
- concreta els requisits mínims comuns que qualsevol domini ha de cobrir
- proposa com a mínim tres dominis viables i comparables
- connecta explícitament el projecte base amb els Reptes 1-5
- deixa clar que cada repte ha d’aportar una funcionalitat professional mínima i no una tècnica aïllada
- confirma compatibilitat amb `Laravel`, `Symfony` i `NestJS`
- fixa el paper de la IA com a eina habitual però verificable
- deixa oberta la línia futura de tokenització sense desplegar encara el projecte complet
- queda preparat com a base real per als Reptes 3-5 i per als futurs materials/enunciats
