# Kit de pilotatge de les setmanes 13-16

## Finalitat del document

Iniciar la construcció operativa de la segona avaluació amb un paquet usable per al tram `13-16`, de manera que el professorat puga consolidar el tancament real de `R3`, obrir `R4` amb criteri professional i arribar a un checkpoint fort d'`API` abans de preparar l'entrada a `R5`.

Este kit prolonga la capa operativa iniciada en els trams `1-4`, `5-8` i `9-12`. La seua funció és traduir les setmanes `13-16` a una pauta de pilotatge real: què convé explicar, què s'ha de modelar, què ha de produir l'alumnat, què s'ha de verificar per alumne i què convé registrar per decidir si la segona avaluació s'està tornant realment pilotable.

El tram assumix que el bloc `9-12` ha deixat `R3` obert i prou encaminat, però no necessàriament blindat; per això la setmana `13` funciona com a consolidació pont abans d'obrir `R4` de manera explícita i verificable.

## Hipòtesi de treball

El kit manté el mateix escenari docent de referència:

- `20` setmanes aproximades
- `6` hores setmanals
- `120` hores lectives aproximades
- desenvolupament principal del projecte dins de les dues primeres avaluacions
- tercera avaluació fora del desenvolupament nuclear del projecte, com a espai residual o de connexió amb empresa o `FCT`

## Criteris d'ús

- cada setmana equival a un bloc d'unes `6` hores, repartible en dues o tres sessions si es manté el mateix objectiu
- Git/GitHub es tracta com a traçabilitat i repàs metodològic, no com a alfabetització inicial
- poden existir parelles de contrast tècnic, trios avançats puntuals o checkpoints coordinats, però l'evidència, la verificació, la defensa i la decisió docent s'han de resoldre individualment
- `R4` no s'ha d'obrir com a simple publicació de rutes; només té sentit si `R3` ha deixat una funcionalitat persistent, explicable i prou estable
- la IA es pot usar com a eina guiada per proposar contractes, col·leccions, proves o documentació, però qualsevol ús ha de quedar verificat, registrat i defensable
- si en una setmana no apareix l'evidència mínima, cal prioritzar reconducció abans d'avançar cap a consum extern o preparació d'integració

## Estructura del tram 13-16

- `Setmana 13`: consolidació final de `R3` i entrada explícita a `R4`
- `Setmana 14`: contracte d'`API` i definició de casos d'ús publicables
- `Setmana 15`: implementació, proves i consum real de l'`API`
- `Setmana 16`: checkpoint fort de `R4` i preparació de `R5`

## Peces que s'activen en este tram

- [kit_pilotatge_setmanes_09_12.md](kit_pilotatge_setmanes_09_12.md)
- [guia_sessio_a_sessio_20_setmanes.md](guia_sessio_a_sessio_20_setmanes.md)
- [annex_suport_i_ampliacio_ritmes.md](annex_suport_i_ampliacio_ritmes.md)
- [pla_execucio_pilotatge_real.md](../00_visio_general/pla_execucio_pilotatge_real.md)
- [repte_03_materials_sessio.md](../04_materials/materials_aula/repte_03_materials_sessio.md)
- [repte_04_materials_sessio.md](../04_materials/materials_aula/repte_04_materials_sessio.md)
- [repte_05_materials_sessio.md](../04_materials/materials_aula/repte_05_materials_sessio.md)
- [guia_contracte_i_disseny_api.md](../04_materials/repte_04/guia_contracte_i_disseny_api.md)
- [guia_proves_i_documentacio_api.md](../04_materials/repte_04/guia_proves_i_documentacio_api.md)
- [checklist_repte_04.md](../04_materials/repte_04/checklist_repte_04.md)
- [repte_04_api_i_consum.md](../04_materials/apunts_reals/repte_04_api_i_consum.md)
- [mini_briefings_setmanals.md](../04_materials/materials_aula/mini_briefings_setmanals.md)
- [checkpoints_curts_aula.md](../04_materials/materials_aula/checkpoints_curts_aula.md)
- [plantilles_feedback_rapid.md](../04_materials/materials_aula/plantilles_feedback_rapid.md)
- [fulls_treball_base.md](../04_materials/materials_aula/fulls_treball_base.md)
- [plantilla_recollida_feedback_pilotatge.md](../03_avaluacio/plantilla_recollida_feedback_pilotatge.md)
- [registre_incidents_i_ajustos_pilotatge.md](../03_avaluacio/registre_incidents_i_ajustos_pilotatge.md)

## Planificació operativa per setmanes

### Setmana 13

- Objectiu docent: consolidar la base persistent i mantenible de `R3` i obrir `R4` només sobre una funcionalitat real del producte
- Focus o repte: consolidació final de `R3` i entrada explícita a `R4`
- Què explica el professorat: què ha de quedar tancat de `R3` abans de publicar una `API`, per què no convé exposar com a servei una base encara fràgil i com seleccionar un cas d'ús publicable amb sentit dins del producte
- Què modela en directe: revisió curta d'un flux persistent ja defensable, lectura de regressió mínima, identificació del recurs o cas d'ús que es publicarà i primer esquema de contracte
- Què fa l'alumnat: tanca pendents nuclears de persistència i mantenibilitat, verifica que el flux principal continua viu, tria individualment quina part del producte publicarà i deixa rastre de per què eixa peça és prou estable per entrar a `R4`
- Materials concrets que s'activen: [kit_pilotatge_setmanes_09_12.md](kit_pilotatge_setmanes_09_12.md), [repte_03_materials_sessio.md](../04_materials/materials_aula/repte_03_materials_sessio.md), [repte_04_materials_sessio.md](../04_materials/materials_aula/repte_04_materials_sessio.md), guia de persistència i modelat, [guia_contracte_i_disseny_api.md](../04_materials/repte_04/guia_contracte_i_disseny_api.md) i guies comunes de testing/debugging
- Evidència mínima a arreplegar: flux principal persistent reproduïble, `README` tècnic actualitzat i cas d'ús d'`API` triat i justificat individualment
- Checkpoint docent: validar si cada alumne pot defensar que `R3` queda prou estable i explicar quin recurs o operació publicarà sense convertir `R4` en un `CRUD` ornamental
- Intervenció per alumnat endarrerit: congelar qualsevol extensió lateral, assegurar una sola operació persistent de punta a punta i reduir `R4` a un recurs nuclear del domini
- Ampliació per alumnat avançat: deixar predefinits errors mínims, permisos o una segona operació coherent sobre el mateix recurs, sempre sense obrir encara massa superfície d'`API`
- Què s'ha de registrar al pilotatge: si la consolidació real de `R3` arriba amb la càrrega prevista, quins bloquejos continuen apareixent abans d'obrir `R4` i si la transició a `API` es comprén com a continuïtat del producte o com a canvi artificial de repte

### Setmana 14

- Objectiu docent: convertir el flux triat en un contracte d'`API` clar, usable i publicable, connectat amb casos d'ús reals del producte
- Focus o repte: contracte d'`API` i casos d'ús publicables
- Què explica el professorat: com passar d'un flux intern del backend a una interfície usable per tercers, quina relació hi ha entre recurs, endpoint, entrada, eixida, codi d'estat i error, i per què el contracte s'ha de poder llegir com a part del producte i no com a llista arbitrària de rutes
- Què modela en directe: definició d'un recurs principal, una operació de consulta o lectura, una operació d'acció o escriptura, la seua resposta correcta i un error mínim controlat, deixant clar com es documenta sense separar-se del comportament real
- Què fa l'alumnat: decideix recursos i endpoints nuclears, concreta camps d'entrada i eixida, fixa casos correctes i errors previsibles, i deixa documentat individualment el contracte mínim que publicarà
- Materials concrets que s'activen: [repte_04_materials_sessio.md](../04_materials/materials_aula/repte_04_materials_sessio.md), [guia_contracte_i_disseny_api.md](../04_materials/repte_04/guia_contracte_i_disseny_api.md), [repte_04_api_i_consum.md](../04_materials/apunts_reals/repte_04_api_i_consum.md), [fulls_treball_base.md](../04_materials/materials_aula/fulls_treball_base.md) i l'itinerari triat reutilitzat en context d'`API`
- Evidència mínima a arreplegar: contracte mínim d'`API` amb recurs, endpoints nuclears, entrades, respostes i errors recognoscibles, vinculat a un cas d'ús real del producte
- Checkpoint docent: comprovar que cada alumne pot explicar per a qui i per a què publica la seua `API`, i que el contracte no desconnecta de la persistència i les regles del domini
- Intervenció per alumnat endarrerit: limitar el contracte a pocs endpoints nuclears, una operació de consulta i una operació d'acció, ajornant qualsevol recurs secundari
- Ampliació per alumnat avançat: afinar millor errors, permisos, coherència entre respostes similars o una documentació inicial més robusta del mateix contracte
- Què s'ha de registrar al pilotatge: si el grup entén bé què fa publicable un cas d'ús, quina part del contracte resulta més costosa de modelar i si els materials actuals eviten l'obertura d'`API` superficials

### Setmana 15

- Objectiu docent: portar el contracte a una `API` funcional, provada, documentada i consumible de manera reproduïble
- Focus o repte: implementació, proves, documentació i consum real de l'`API`
- Què explica el professorat: per què implementar no és suficient si no hi ha prova i consum real, com alinear contracte, codis d'estat, validacions i documentació, i quin tipus de consum mínim ja prepara amb sentit l'entrada a `R5`
- Què modela en directe: un endpoint nuclear complet amb cas correcte, cas de validació incorrecta i cas d'accés o error previsibles; també una prova reproduïble amb col·lecció, `curl`, script o client simple i una anotació curta al `README`
- Què fa l'alumnat: implementa endpoints principals, ajusta validacions i respostes, prepara col·lecció de proves o equivalent, documenta com reproduir-les i demostra un consum real de la seua `API`
- Materials concrets que s'activen: [repte_04_materials_sessio.md](../04_materials/materials_aula/repte_04_materials_sessio.md), [guia_proves_i_documentacio_api.md](../04_materials/repte_04/guia_proves_i_documentacio_api.md), [checklist_repte_04.md](../04_materials/repte_04/checklist_repte_04.md), guia de testing/debugging, [plantilles_feedback_rapid.md](../04_materials/materials_aula/plantilles_feedback_rapid.md) i [checkpoints_curts_aula.md](../04_materials/materials_aula/checkpoints_curts_aula.md)
- Evidència mínima a arreplegar: endpoints nuclears funcionals, prova reproduïble amb cas correcte i cas d'error, documentació alineada amb el comportament real i una evidència mínima de consum
- Checkpoint docent: validar que cada alumne pot mostrar l'`API` en funcionament, provar-la sense improvisació i explicar quina part del consum és realment seua encara que compartisca encàrrec funcional amb altres alumnes
- Intervenció per alumnat endarrerit: tancar només un recurs nuclear, una prova clara i una documentació curta; ajornar qualsevol consumidor complex o endpoint lateral
- Ampliació per alumnat avançat: reforçar col·lecció de proves, tractament d'errors, control d'accés o qualitat del consumidor sobre la mateixa `API`
- Què s'ha de registrar al pilotatge: quins punts fallen més entre contracte, implementació i documentació, si la càrrega de prova i consum és assumible i quins patrons d'ús de la IA necessiten més verificació docent

### Setmana 16

- Objectiu docent: tancar `R4` amb un checkpoint fort d'`API` usable i deixar preparada la decisió d'integració de `R5`
- Focus o repte: checkpoint fort de `R4` i preparació de `R5`
- Què explica el professorat: què compta com a `R4` realment tancat, quina diferència hi ha entre una `API` que respon i una `API` publicable per a integració, i com seleccionar una necessitat de `R5` sense obrir una integració ornamental
- Què modela en directe: lectura curta de checkpoint amb contracte, proves, documentació i consum visibles; identificació de l'endpoint o recurs que serà més útil per a una integració externa o un workflow híbrid
- Què fa l'alumnat: tanca pendents de contracte, proves i `README`, deixa evidències individuals del que pot verificar i defensar, identifica quina necessitat real del producte passarà a `R5` i documenta la decisió d'entrada
- Materials concrets que s'activen: [repte_04_materials_sessio.md](../04_materials/materials_aula/repte_04_materials_sessio.md), [repte_05_materials_sessio.md](../04_materials/materials_aula/repte_05_materials_sessio.md), [checklist_repte_04.md](../04_materials/repte_04/checklist_repte_04.md), [plantilla_recollida_feedback_pilotatge.md](../03_avaluacio/plantilla_recollida_feedback_pilotatge.md) i [registre_incidents_i_ajustos_pilotatge.md](../03_avaluacio/registre_incidents_i_ajustos_pilotatge.md)
- Evidència mínima a arreplegar: `API` usable, documentada i provada; `README` actualitzat; evidència de consum reproduïble; i decisió justificada del flux o integració que entrarà a `R5`
- Checkpoint docent: decidir si cada alumne té `R4` prou tancat per passar a integració o si encara necessita consolidar contracte, prova o consum abans d'obrir `R5`
- Intervenció per alumnat endarrerit: freeze total de noves operacions, tancament d'un únic flux d'`API` verificable i definició d'una integració mínima molt curta per al pas següent
- Ampliació per alumnat avançat: deixar millor preparat el consum extern, afinar errors o permisos o anticipar criteris de traçabilitat del flux híbrid, sense desplaçar el centre del treball fora de `R4`
- Què s'ha de registrar al pilotatge: si `CP-P4` és assumible dins del temps real, quins equips arriben a `R4` només de manera aparent, quina qualitat té la documentació per a tercers i si la preparació de `R5` queda prou clara per obrir la integració sense improvisació

## Registre mínim de pilotatge per al tram 13-16

Per a les setmanes `13-16`, convé deixar com a mínim:

- una nota setmanal per alumne amb estat real de `R3`/`R4`, bloqueig principal i decisió docent següent
- una síntesi de si `R3` arriba prou consolidat per obrir `R4` i de si `R4` es tanca com a `API` realment usable
- almenys una entrada de feedback al tancament fort d'`R4`
- una entrada al registre d'incidents si apareixen patrons recurrents en contracte d'`API`, proves, documentació, consum, autoria o acreditació individual

## Criteri de pas a la setmana 17

Només convé entrar al bloc següent si:

- hi ha una funcionalitat del producte publicada com a `API` amb contracte recognoscible i sentit real dins del domini
- existixen proves reproduïbles, documentació alineada amb el comportament real i consum mínim verificat
- cada alumne pot explicar i defensar la seua part del flux publicat, encara que hi haja hagut cooperació tècnica coordinada o un mateix encàrrec funcional
- el `README`, la traçabilitat i les evidències permeten identificar quin endpoint o recurs serà la base útil per a `R5`

## Definition of done del document

Este kit es considera completat quan:

- concreta les setmanes `13-16` com a quart tram operatiu del curs
- indica per a cada setmana objectiu, paper docent, treball de l'alumnat, materials activats, evidència mínima, checkpoint, suport, ampliació i registre de pilotatge
- connecta la consolidació final de `R3`, l'entrada explícita a `R4`, el contracte d'`API`, les proves, la documentació, el consum real i la preparació de `R5`
- deixa clar que pot haver-hi cooperació tècnica coordinada, però que l'evidència, la verificació i la defensa són individuals
- deixa la segona avaluació iniciada com a bloc pilotable real, no només descrita de manera abstracta
