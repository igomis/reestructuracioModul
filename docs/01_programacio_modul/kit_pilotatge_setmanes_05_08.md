# Kit de pilotatge de les setmanes 5-8

## Finalitat del document
Continuar la capa operativa del curs amb un paquet usable per al tram `5-8`, de manera que el professorat puga desplegar `R2`, consolidar el tancament funcional real de `R1` i preparar l'entrada a `R3` sense haver de reconstruir la seqüència a partir de peces disperses.

Este kit no substituïx la planificació general del curs. La seua funció és concentrar què convé activar en aula durant el segon bloc del primer període lectiu: què s'explica, què es modela, què ha de produir l'alumnat, què s'ha de revisar en cada checkpoint i què convé registrar durant el pilotatge.

## Hipòtesi de treball
El kit manté la mateixa base temporal i docent del paquet:
- `20` setmanes aproximades
- `6` hores setmanals
- `120` hores lectives aproximades
- desenvolupament principal del projecte dins de les dues primeres avaluacions
- tercera avaluació fora del desenvolupament nuclear del projecte, com a espai residual o de connexió amb empresa o `FCT`

## Criteris d'ús
- cada setmana equival a un bloc d'unes `6` hores, repartible en dues o tres sessions si es manté el mateix objectiu
- Git/GitHub es tracta com a traçabilitat i repàs metodològic, no com a alfabetització inicial
- este tram no pot començar com si `R1` estiguera tancat si encara no hi ha primera funcionalitat real, validada i registrada
- `R2` no es considera superat quan hi ha login, sinó quan hi ha una primera funcionalitat de negoci protegida, verificable i defensable
- si en una setmana no apareix l'evidència mínima, cal prioritzar reconducció abans d'obrir el pas següent

## Estructura del tram 5-8
- `Setmana 5`: tancament usable de `R1` i entrada controlada a auth o estat equivalent
- `Setmana 6`: desplegament real de `R2` com a funcionalitat de negoci autenticada
- `Setmana 7`: validació, errors, control d'accés i proves mínimes de `R2`
- `Setmana 8`: tancament de `R2` i preparació explícita de l'entrada a `R3`

## Peces que s'activen en este tram
- [kit_pilotatge_setmanes_01_04.md](kit_pilotatge_setmanes_01_04.md)
- [guia_sessio_a_sessio_20_setmanes.md](guia_sessio_a_sessio_20_setmanes.md)
- [annex_suport_i_ampliacio_ritmes.md](annex_suport_i_ampliacio_ritmes.md)
- [pla_execucio_pilotatge_real.md](../00_visio_general/pla_execucio_pilotatge_real.md)
- [repte_01_materials_sessio.md](../04_materials/materials_aula/repte_01_materials_sessio.md)
- [repte_02_materials_sessio.md](../04_materials/materials_aula/repte_02_materials_sessio.md)
- [repte_03_materials_sessio.md](../04_materials/materials_aula/repte_03_materials_sessio.md)
- [mini_briefings_setmanals.md](../04_materials/materials_aula/mini_briefings_setmanals.md)
- [checkpoints_curts_aula.md](../04_materials/materials_aula/checkpoints_curts_aula.md)
- [plantilles_feedback_rapid.md](../04_materials/materials_aula/plantilles_feedback_rapid.md)
- [fulls_treball_base.md](../04_materials/materials_aula/fulls_treball_base.md)
- [plantilla_recollida_feedback_pilotatge.md](../03_avaluacio/plantilla_recollida_feedback_pilotatge.md)
- [registre_incidents_i_ajustos_pilotatge.md](../03_avaluacio/registre_incidents_i_ajustos_pilotatge.md)

## Planificació operativa per setmanes
### Setmana 5
- Objectiu docent: confirmar que `R1` queda realment usable i obrir `R2` sense començar sobre una base falsa
- Focus o repte: tancament funcional de `R1` i entrada a autenticació o estat equivalent
- Què explica el professorat: què s'entén per pas net de `R1` a `R2`, diferència entre funcionalitat d'entrada i infraestructura d'accés, i per què no convé obrir auth si el flux inicial encara no és real
- Què modela en directe: revisió curta d'un `R1` tancat, definició d'actor del domini i primer mecanisme mínim d'accés o identificació
- Què fa l'alumnat: corregeix pendents de `R1`, identifica l'actor del domini, prepara alta, login o estat equivalent i fixa quin flux del producte quedarà protegit
- Materials concrets que s'activen: [kit_pilotatge_setmanes_01_04.md](kit_pilotatge_setmanes_01_04.md), [repte_01_materials_sessio.md](../04_materials/materials_aula/repte_01_materials_sessio.md), [repte_02_materials_sessio.md](../04_materials/materials_aula/repte_02_materials_sessio.md), guies comunes de testing/debugging i ús verificable de la IA
- Evidència mínima a arreplegar: `R1` reproduïble, actor del domini definit i primer mecanisme d'accés operatiu
- Checkpoint docent: decidir si l'equip entra a `R2` amb una base real o si encara necessita freeze de funcionalitat i reconducció de `R1`
- Intervenció per alumnat endarrerit: obligar a tancar una sola entrada funcional i un únic mecanisme d'accés; ajornar qualsevol rol o extensió no nuclear
- Ampliació per alumnat avançat: justificar millor la decisió d'actor, separar autenticació i autorització o afegir un primer cas d'accés denegat
- Què s'ha de registrar al pilotatge: equips que encara confonen `R1` amb esquelet tècnic, càrrega real per passar a `R2` i claredat dels criteris de pas

### Setmana 6
- Objectiu docent: desplegar `R2` com a primera funcionalitat de negoci autenticada
- Focus o repte: nucli funcional de `R2`
- Què explica el professorat: que el repte no és “fer login”, sinó protegir una operació real del domini amb una regla mínima de negoci
- Què modela en directe: un flux autenticat complet amb operació central, accés autoritzat i primer cas d'accés restringit
- Què fa l'alumnat: connecta auth o estat equivalent amb una operació rellevant del producte i implementa la primera restricció o control d'accés recognoscible
- Materials concrets que s'activen: [repte_02_materials_sessio.md](../04_materials/materials_aula/repte_02_materials_sessio.md), [fulls_treball_base.md](../04_materials/materials_aula/fulls_treball_base.md), [plantilles_feedback_rapid.md](../04_materials/materials_aula/plantilles_feedback_rapid.md) i l'itinerari tecnològic corresponent
- Evidència mínima a arreplegar: operació de negoci protegida, cas autoritzat reproduïble i primer cas denegat recognoscible
- Checkpoint docent: comprovar que hi ha valor funcional del producte i no només formularis d'accés
- Intervenció per alumnat endarrerit: reduir el repte a un sol actor i una sola operació protegida de punta a punta
- Ampliació per alumnat avançat: afegir una segona restricció o un primer tractament més fi d'autorització sobre el mateix flux
- Què s'ha de registrar al pilotatge: si el pas de infraestructura a funcionalitat real és assumible, quins bloquejos apareixen per domini o itinerari i quina part del modelatge docent desbloqueja més

### Setmana 7
- Objectiu docent: consolidar `R2` amb validació, tractament d'errors i verificació mínima
- Focus o repte: control d'accés, casos límit i proves mínimes del flux autenticat
- Què explica el professorat: diferència entre funcionalitat aparent i funcionalitat verificable, com provar casos correctes i incorrectes i per què el control d'accés ha de poder-se defensar
- Què modela en directe: un recorregut complet amb dades correctes, dades incorrectes i acció denegada, deixant rastre al `README` i en les evidències
- Què fa l'alumnat: reforça validacions del servidor, controla errors mínims, prova el flux complet i actualitza documentació operativa
- Materials concrets que s'activen: [repte_02_materials_sessio.md](../04_materials/materials_aula/repte_02_materials_sessio.md), guia de testing i debugging, [checkpoints_curts_aula.md](../04_materials/materials_aula/checkpoints_curts_aula.md) i [plantilla_recollida_feedback_pilotatge.md](../03_avaluacio/plantilla_recollida_feedback_pilotatge.md)
- Evidència mínima a arreplegar: flux complet provat amb cas correcte, cas incorrecte, cas denegat i `README` actualitzat
- Checkpoint docent: validar que `R2` és ja reproduïble, comprensible i defensable davant d'una revisió curta
- Intervenció per alumnat endarrerit: congelar qualsevol ampliació, deixar només dos casos clau i fer microcheckpoint obligatori abans de passar de setmana
- Ampliació per alumnat avançat: sistematitzar millor proves, refinar missatges d'error o registrar incidències de manera més clara
- Què s'ha de registrar al pilotatge: quins errors es repetixen, si l'evidència demanada és massa ambigua o massa costosa i si la càrrega setmanal és assumible dins del temps real

### Setmana 8
- Objectiu docent: tancar `R2` i deixar triada la funcionalitat que entrarà a `R3`
- Focus o repte: tancament de `R2` i preparació d'arquitectura/persistència
- Què explica el professorat: què fa que una funcionalitat autenticada siga prou madura per entrar a `R3`, quina part del flux convé professionalitzar i per què `R3` no és “fer MVC” sinó fer mantingible i persistent una operació real
- Què modela en directe: lectura tècnica del flux de `R2`, identificació de punts fràgils i mapa mínim de la funcionalitat que es refactoritzarà o persistirà després
- Què fa l'alumnat: tanca evidències de `R2`, revisa el flux principal, selecciona el cas d'ús que passarà a `R3` i documenta l'estat del producte al final del bloc
- Materials concrets que s'activen: [repte_02_materials_sessio.md](../04_materials/materials_aula/repte_02_materials_sessio.md), [repte_03_materials_sessio.md](../04_materials/materials_aula/repte_03_materials_sessio.md), [mini_briefings_setmanals.md](../04_materials/materials_aula/mini_briefings_setmanals.md), [registre_incidents_i_ajustos_pilotatge.md](../03_avaluacio/registre_incidents_i_ajustos_pilotatge.md)
- Evidència mínima a arreplegar: `R2` tancat amb flux defensable i cas d'ús de `R3` triat i justificat
- Checkpoint docent: decidir si l'equip està en condicions d'obrir `R3` o si ha de continuar consolidant `R2`
- Intervenció per alumnat endarrerit: mantindre només el flux autenticat principal, ajornar rols secundaris i triar una única operació a professionalitzar en `R3`
- Ampliació per alumnat avançat: avançar model mínim de dades, mapa de capes o criteri de servei sense obrir encara persistència completa
- Què s'ha de registrar al pilotatge: si el tancament de `R2` arriba dins del temps previst, quins equips encara arrosseguen una lectura trivial del repte i quins ajustos caldria aplicar abans del bloc `R3`

## Registre mínim de pilotatge per al tram 5-8
Per a les setmanes `5-8`, convé deixar com a mínim:
- una nota setmanal per equip amb estat funcional, bloqueig principal i decisió docent
- una síntesi de si el pas de `R1` a `R2` ha sigut net o ha necessitat reconducció
- almenys una entrada de feedback al tancament de `R2`
- una entrada al registre d'incidents si apareixen patrons recurrents en auth, control d'accés, validació, càrrega o comprensió del repte

## Criteri de pas a la setmana 9
Només convé obrir `R3` si:
- l'equip pot reproduir un flux autenticat complet amb valor real del producte
- hi ha almenys un cas correcte, un cas incorrecte i un cas denegat recognoscibles
- el `README` i les evidències expliquen què fa el producte i quin flux es refactoritzarà o persistirà
- el grup pot defensar que `R2` és funcionalitat de negoci i no infraestructura decorativa

## Definition of done del document
Este kit es considera completat quan:
- concreta les setmanes `5-8` com a segon tram operatiu del curs
- indica per a cada setmana objectiu, paper docent, treball de l'alumnat, materials activats, evidència mínima, checkpoint, suport, ampliació i registre de pilotatge
- connecta el tancament de `R1`, el desplegament real de `R2` i la preparació d'entrada a `R3`
- manté coherència explícita amb el kit de les setmanes `1-4`, la seqüència setmanal del curs i el pla d'execució del pilotatge
- deixa el professorat en condicions d'estirar el pilotatge més enllà del primer mes sense tornar a un nivell abstracte
