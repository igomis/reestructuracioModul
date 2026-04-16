# Kit de pilotatge de les setmanes 1-4

## Finalitat del document

Convertir l'arrancada del curs en una peça operativa directament usable per al pilotatge real, de manera que el professorat puga conduir les primeres quatre setmanes sense reconstruir la seqüència a partir de documents separats.

Este kit concentra, per al primer tram del curs, què cal explicar, què convé modelar, què ha de fer l'alumnat, quines evidències s'han de recollir i què s'ha de registrar per validar el model amb alumnat real.

## Hipòtesi de treball

El kit s'ha calibrat sobre l'escenari docent que ja assumix el paquet:

- `20` setmanes aproximades
- `6` hores setmanals
- `120` hores lectives aproximades
- desenvolupament principal del projecte dins de les dues primeres avaluacions
- tercera avaluació fora del desenvolupament nuclear del projecte, com a espai residual o de connexió amb empresa o `FCT`

## Criteris d'ús

- cada setmana equival a un bloc d'unes `6` hores; el centre pot repartir-lo en dues o tres sessions si manté el mateix objectiu
- Git/GitHub es tracta com a repàs metodològic, traçabilitat i criteri de treball, no com a iniciació bàsica
- el kit activa materials ja existents; no substituïx ni la guia sessió a sessió ni els materials de repte, sinó que els empaqueta per a l'arrancada real
- si no apareix l'evidència mínima setmanal, no convé donar per superat el bloc encara que l'equip “parega” avançat
- el criteri docent clau és assegurar que `R1` queda com a primera funcionalitat real del producte i no com a kickoff abstracte

## Estructura del tram inicial

- `Setmana 1`: marc comú, producte, repositori i traçabilitat
- `Setmana 2`: domini, model client/servidor i decisió tècnica justificada
- `Setmana 3`: `R1` com a microreptes `1-2` en `2` sessions de `3` hores
- `Setmana 4`: `R1` com a microreptes `3-4` en `2` sessions de `3` hores

## Peces que s'activen en este tram

- [guia_sessio_a_sessio_20_setmanes.md](guia_sessio_a_sessio_20_setmanes.md)
- [annex_suport_i_ampliacio_ritmes.md](annex_suport_i_ampliacio_ritmes.md)
- [pla_execucio_pilotatge_real.md](../00_visio_general/pla_execucio_pilotatge_real.md)
- [repte_01_materials_sessio.md](../04_materials/materials_aula/repte_01_materials_sessio.md)
- [mini_briefings_setmanals.md](../04_materials/materials_aula/mini_briefings_setmanals.md)
- [checkpoints_curts_aula.md](../04_materials/materials_aula/checkpoints_curts_aula.md)
- [plantilles_feedback_rapid.md](../04_materials/materials_aula/plantilles_feedback_rapid.md)
- [fulls_treball_base.md](../04_materials/materials_aula/fulls_treball_base.md)
- [plantilla_recollida_feedback_pilotatge.md](../03_avaluacio/plantilla_recollida_feedback_pilotatge.md)
- [registre_incidents_i_ajustos_pilotatge.md](../03_avaluacio/registre_incidents_i_ajustos_pilotatge.md)

## Planificació operativa per setmanes

### Setmana 1

- Objectiu docent: obrir el curs amb criteri comú de producte, evidències i traçabilitat
- Focus o repte: marc del curs i entrada a `R1`
- Què explica el professorat: model per reptes, projecte base, dominis admesos, criteri de no trivialitat, ús verificable de la IA i paper de Git/GitHub com a metodologia de treball
- Què modela en directe: obertura d'un repositori de treball, estructura mínima de `README` i una explicació curta de com deixar rastre de decisions
- Què fa l'alumnat: forma equip, crea repositori, obri `README`, fixa domini provisional i acorda convencions bàsiques de treball
- Materials concrets que s'activen: guies comunes de Git, `README` i ús verificable de la IA; [repte_01_materials_sessio.md](../04_materials/materials_aula/repte_01_materials_sessio.md); plantilles de briefing i full de treball base
- Evidència mínima a arreplegar: repositori creat, `README` inicial, domini provisional i primera traça de decisió tècnica
- Checkpoint docent: comprovar que l'equip pot explicar quin producte començarà a construir i com ho documentarà
- Intervenció per alumnat endarrerit: reduir el bloc a repositori usable, `README` curt i una sola descripció de cas d'ús inicial
- Ampliació per alumnat avançat: comparar dues opcions de domini o dos enfocaments funcionals i justificar la triada amb un mini `ADR`
- Què s'ha de registrar al pilotatge: dubtes recurrents sobre el model del curs, comprensió real d'evidències, bloquejos inicials amb `README` o traçabilitat i adequació del temps de la setmana

### Setmana 2

- Objectiu docent: convertir el kickoff en una decisió tècnica i funcional recognoscible
- Focus o repte: `R1` com a decisió de domini, base comuna en `PHP` i flux d'entrada
- Què explica el professorat: què no és suficient en `R1`, com acotar un primer flux funcional i per què encara no toca obrir itineraris ni debat de frameworks
- Què modela en directe: decisió tècnica breu, cas d'ús inicial del producte i esquema del primer flux que s'hauria de poder ensenyar
- Què fa l'alumnat: concreta el primer cas d'ús, descriu el flux d'entrada i prepara l'estructura mínima del projecte sobre la base comuna en `PHP`
- Materials concrets que s'activen: [repte_01_materials_sessio.md](../04_materials/materials_aula/repte_01_materials_sessio.md), [fulls_treball_base.md](../04_materials/materials_aula/fulls_treball_base.md), base comuna del curs i guia `README`/`ADR`
- Evidència mínima a arreplegar: domini triat, base comuna en `PHP` arrancada, flux inicial descrit i estructura mínima del projecte recognoscible
- Checkpoint docent: validar que hi ha producte i primer cas d'ús, no només infraestructura o projecte buit
- Intervenció per alumnat endarrerit: forçar un únic cas d'ús d'entrada i bloquejar qualsevol ampliació lateral
- Ampliació per alumnat avançat: afegir una alternativa descartada amb trade-off curt o un criteri tècnic addicional de decisió
- Què s'ha de registrar al pilotatge: quins punts generen més dispersió en la tria de domini, quines instruccions del `R1` demanen més aclariment i quins equips confonen producte amb infraestructura

### Setmana 3

- Objectiu docent: resoldre la primera mitat de `R1` en `2` sessions de `3` hores sense inflar el repte
- Focus o repte: microreptes `1-2` de `R1`: model client/servidor i entorn executable
- Què explica el professorat: com acotar una decisió tècnica guiada i com convertir-la en un entorn executable amb `Docker`, `PHP` i servidor web
- Què modela en directe: una arrencada mínima reproduïble i una actualització del `README` amb passos reals
- Què fa l'alumnat: justifica el stack base, prepara l'entorn i deixa el projecte arrancant
- Materials concrets que s'activen: [repte_01_materials_sessio.md](../04_materials/materials_aula/repte_01_materials_sessio.md), [mini_briefings_setmanals.md](../04_materials/materials_aula/mini_briefings_setmanals.md), [checkpoints_curts_aula.md](../04_materials/materials_aula/checkpoints_curts_aula.md) i la base comuna del curs
- Evidència mínima a arreplegar: decisió tècnica visible, projecte arrancant i `README` inicial usable
- Checkpoint docent: verificar en `2-3` minuts que el projecte arranca de veritat i que el grup sap explicar la base tècnica
- Intervenció per alumnat endarrerit: simplificar l'entorn i congelar qualsevol ampliació lateral fins que l'arrencada siga reproduïble
- Ampliació per alumnat avançat: millorar scripts, justificar millor la base tècnica o documentar un trade-off addicional
- Què s'ha de registrar al pilotatge: dificultats reals per passar de decisió tècnica a arrencada i si la seqüència de `2` sessions és suficient

### Setmana 4

- Objectiu docent: tancar `R1` amb primer punt d'entrada funcional, documentació i checkpoint net cap a `R2`
- Focus o repte: microreptes `3-4` de `R1`
- Què explica el professorat: diferència entre infraestructura i punt d'entrada funcional, necessitat de deixar rastre de prova i què ha d'arribar preparat al checkpoint `R1 -> R2`
- Què modela en directe: una ruta, vista, `endpoint` o `healthcheck` simple i la seua verificació seguint el `README`
- Què fa l'alumnat: completa el primer punt d'entrada funcional del backend, actualitza `README` i prepara el pas a auth o estat equivalent
- Materials concrets que s'activen: [repte_01_materials_sessio.md](../04_materials/materials_aula/repte_01_materials_sessio.md), guia de testing i debugging, [plantilles_feedback_rapid.md](../04_materials/materials_aula/plantilles_feedback_rapid.md) i plantilla de feedback de pilotatge
- Evidència mínima a arreplegar: prova reproduïble del punt d'entrada funcional i `README` actualitzat
- Checkpoint docent: decidir si l'equip té prou base real per obrir `R2` sense començar sobre un esquelet buit
- Intervenció per alumnat endarrerit: tancar un únic punt d'entrada funcional i una única prova clara; ajornar qualsevol millora lateral
- Ampliació per alumnat avançat: reforçar documentació tècnica, onboarding o una segona resposta simple del backend
- Què s'ha de registrar al pilotatge: si el temps de `R1` és suficient, quines evidències costen més de fer emergir, si els checkpoints són prou clars i quins ajustos immediats convé aplicar abans d'entrar en `R2`

## Registre mínim de pilotatge per al tram inicial

Per a les setmanes `1-4`, convé deixar com a mínim:

- una nota setmanal breu per equip amb estat del producte, bloqueig principal i decisió docent
- una síntesi curta de si l'evidència mínima ha aparegut o no
- almenys una entrada de feedback al tancament de `R1`
- una entrada al registre d'incidents si es repetixen patrons de bloqueig en domini, traçabilitat, funcionalitat real o càrrega temporal

## Criteri de pas a la setmana 5

Només convé entrar en `R2` si:

- el producte ja té una primera interacció real i visible
- el projecte arranca de manera reproduïble i deixa un primer punt d'entrada funcional del backend
- l'equip pot defensar què fa ja el producte i quin serà el flux que es protegirà a `R2`
- el `README` i la traçabilitat permeten entendre on està el projecte real

## Definition of done del document

Este kit es considera completat quan:

- concreta l'arrancada real del curs en les setmanes `1-4`
- indica per a cada setmana objectiu, paper docent, treball de l'alumnat, materials activats, evidència mínima, checkpoint, suport, ampliació i registre de pilotatge
- connecta de manera explícita la seqüència setmanal amb `R1` i amb l'entrada posterior a `R2`
- reutilitza de manera recognoscible les peces de seqüència, ritmes, materials d'aula i instruments de pilotatge ja existents
- deixa el professorat en condicions d'obrir el curs sense haver de reconstruir manualment el primer mes
