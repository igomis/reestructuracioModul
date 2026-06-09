# Guia sessió a sessió del curs en 20 setmanes

## Finalitat del document

Convertir la implantació del mòdul en una guia docent setmanal usable, pensada perquè el professorat puga saber què convé explicar, què modelar, què deixar a autonomia i com adaptar el ritme segons el progrés real de l'alumnat.

Esta peça complementa [programacio_aula_per_repte.md](programacio_aula_per_repte.md), [seqüenciacio_sessions_2_avaluacions.md](seqüenciacio_sessions_2_avaluacions.md) i [pla_execucio_pilotatge_real.md](../arxiu/pla_execucio_pilotatge_real.md). Aquells documents fixen la lògica global i els checkpoints; esta guia baixa el model a una lectura setmanal o de bloc docent real.

## Hipòtesi de treball

La guia està calibrada sobre l'escenari següent:

- `20` setmanes aproximades
- `6` hores setmanals
- `120` hores lectives aproximades
- desenvolupament principal del projecte dins de les dues primeres avaluacions
- tercera avaluació fora del desenvolupament nuclear del projecte, com a espai residual o de connexió amb empresa o `FCT`

## Criteris d'ús

- cada setmana equival a un bloc docent d'unes `6` hores; el centre pot repartir-lo en dues o tres sessions sense alterar el sentit del bloc
- Git/GitHub es treballa com a repàs metodològic i criteri de traçabilitat, no com a iniciació des de zero
- cada bloc combina explicació docent, modelatge en directe, treball guiat i autonomia supervisada
- poden existir moments de treball cooperatiu o sincronitzat, però l'evidència acreditativa, la verificació i l'avaluació s'han de recollir amb criteri individual
- si una evidència mínima no apareix, no s'ha d'obrir el bloc següent com si el pas estiguera assolit
- les microdefenses tècniques de `R2`, `R3`, `R4` i `R5` són punts de verificació d'autoria, comprensió real i ús verificable de la IA
- el criteri principal no és “arribar a tot”, sinó mantindre la progressió real del producte i la seua defensa tècnica dins de les dues primeres avaluacions

## Estructura general del curs

- `Avaluació 1` (`setmanes 1-10 / ~60h`): marc comú, `R1`, `R2`, microdefensa de `R2` i entrada real a `R3`
- `Avaluació 2` (`setmanes 11-20 / ~60h`): tancament de `R3`, microdefenses de `R3`, `R4` i `R5`, i defensa final
- `Avaluació 3`: sense desenvolupament central del projecte; només seguiment residual, connexió amb empresa o `FCT`

## Mapa reestructurat de reptes, setmanes i verificacions

| Bloc | Setmanes | Tancament verificable | Imprescindible | Recuperable | Ampliació |
|---|---:|---|---|---|---|
| Arrancada i `R1` | `1-4` | checkpoint `R1 -> R2` | repo, base en `PHP`, primer punt d'entrada i `README` executable | documentació, incidències i defensa curta | millora d'onboarding o scripts |
| `R2` | `5-8` | [R2SX. Microdefenses tècniques](programacio_aula_r2sx_microdefenses_tecniques_criteris.md) | formulari variat, validació de servidor, estat inicial, funcionalitat protegida i traçabilitat | prova unitària mínima, proves de flux i `AI log` incomplet | llibreria externa menuda, millor tractament d'errors o proves negatives |
| `R3` | `9-12` | [R3SX. Microdefenses tècniques](programacio_aula_r3sx_microdefenses_tecniques_criteris.md) | framework arrancable, separació de responsabilitats, persistència inicial i flux end-to-end | segon flux reduït, documentació de migracions o proves | relació de dades, serveis o validació reforçada |
| `R4` | `13-16` | [R4SX. Microdefenses tècniques](programacio_aula_r4sx_microdefenses_tecniques_criteris.md) | contracte d'API, endpoints, protecció o control d'accés, consum/prova i documentació | col·lecció de proves, cas denegat o documentació incompleta | permisos més fins, consumidor més complet o millor contracte |
| `R5` | `17-19` | [R5SX. Microdefenses tècniques](programacio_aula_r5sx_microdefenses_tecniques_criteris.md) | integració amb valor real, transformació, prova, errors i documentació | estabilització del flux i registre d'incidències | observabilitat, desplegament o integració més robusta |
| Defensa final | `20` | defensa final i tancament del curs | producte defensat, repo coherent i evidències finals | defensa ajustada al mínim funcional no trivial | proposta `v2` acotada |

Les microdefenses diferencien tres situacions que la revisió ordinària del repositori no sempre detecta: treball autònom comprés, treball assistit per IA però validat, i delegació excessiva en IA. Per això sempre combinen demo, codi o configuració, traçabilitat, `AI log` i preguntes de contrast.

## Estratègia general de suport a alumnat endarrerit

- reduir abast al mínim funcional no trivial del bloc actual
- reusar materials del repte i apunts reals com a pauta d'execució, no com a lectura opcional
- revisar primer `README`, traçabilitat i estat real del producte abans d'afegir noves funcions
- forçar un checkpoint curt de recuperació abans de permetre avançar
- prioritzar un sol flux funcional complet per damunt de diverses peces a mig fer

## Estratègia general d'ampliació per alumnat avançat

- aprofundir sense trencar la seqüència comuna del curs
- afegir proves, millor tractament d'errors, regles de negoci addicionals o documentació més sòlida
- explorar una variant més completa del mateix domini sense canviar el repte central
- documentar millor decisions, consum d'`API` o integració, en lloc d'obrir línies noves fora del producte

## Moments de classe guiada i moments d'autonomia

Patró recomanat dins de cada bloc setmanal de `6` hores:

- `1-2h` de marc i explicació docent
- `1-2h` de modelatge en directe o taller guiat
- `2-3h` de treball autònom o per equips amb seguiment curt del professorat

Regla pràctica:

- les setmanes de canvi de repte necessiten més classe guiada
- les setmanes de consolidació, proves o documentació necessiten més autonomia supervisada
- la cooperació tècnica pot existir, però cada alumne ha de mantindre rastre propi, evidència pròpia i capacitat de defensa individual

## Seqüència setmanal o per blocs

### Avaluació 1

#### Setmana 1

- Focus o repte: marc comú del curs i arranque del producte
- Què fa el professorat: presenta el model per reptes, el projecte base, els dominis admesos i el criteri d'evidències; revisa Git/GitHub com a metodologia i traçabilitat
- Què fa l'alumnat: crea repositori, obri la base de treball, fixa equip i primeres convencions
- Materials per a l'alumnat: projecte base, enunciat base, guies comunes de Git, `README` i ús verificable de la IA
- Evidència mínima del bloc: repositori creat, `README` inicial i criteri compartit de treball
- Checkpoint docent: comprovar que l'arrancada no queda en simple explicació oral
- Pla per a alumnat endarrerit: repositori mínim, `README` curt i checklist de posada en marxa
- Pla per a alumnat avançat: justificar dues alternatives de domini o dos enfocaments funcionals abans de decidir

#### Setmana 2

- Focus o repte: domini, base comuna en `PHP` i decisió tècnica inicial
- Què fa el professorat: modela una decisió tècnica breu, exemplifica un `ADR` curt i acota què no és suficient en `R1`
- Què fa l'alumnat: tria domini, assumix la base comuna en `PHP` i concreta el primer cas d'ús mínim del producte
- Materials per a l'alumnat: fitxa del Repte 1, base comuna del curs, guia `README` i `ADR`
- Evidència mínima del bloc: domini triat, decisió tècnica justificada i traçabilitat inicial
- Checkpoint docent: validar que hi ha producte pensat, no només infraestructura preparada
- Pla per a alumnat endarrerit: domini més acotat i un sol cas d'ús d'entrada
- Pla per a alumnat avançat: explorar riscos i trade-offs de la decisió tècnica

#### Setmana 3

- Focus o repte: `R1` com a microreptes `1-2`: model client/servidor i entorn executable
- Què fa el professorat: modela una decisió tècnica breu, una arrencada amb `Docker`, `PHP` i servidor web i l'estructura mínima del `README`
- Què fa l'alumnat: concreta la base tècnica i deixa el projecte arrancant de manera reproduïble
- Materials per a l'alumnat: apunt real del Repte 1, materials comuns i suport de la base comuna en `PHP`
- Evidència mínima del bloc: decisió tècnica visible, projecte arrancant i `README` inicial usable
- Checkpoint docent: revisar que hi ha arrencada real i no només fitxers de configuració
- Pla per a alumnat endarrerit: entorn més simple i un únic camí d'arrencada
- Pla per a alumnat avançat: millorar scripts o explicar millor els trade-offs de la base tècnica

#### Setmana 4

- Focus o repte: `R1` com a microreptes `3-4`: primer punt d'entrada funcional, documentació i checkpoint
- Què fa el professorat: modela una ruta, vista, `endpoint` o `healthcheck` simple i exemplifica com deixar rastre real al `README`
- Què fa l'alumnat: completa el primer punt d'entrada funcional del backend, revisa documentació i prepara el checkpoint `R1 -> R2`
- Materials per a l'alumnat: apunt real del Repte 1, guia de testing i debugging
- Evidència mínima del bloc: `R1` reproduïble amb punt d'entrada funcional i `README` executable
- Checkpoint docent: tancament de `R1` només si no és un esquelet buit
- Pla per a alumnat endarrerit: un únic punt d'entrada funcional i una única prova d'arrencada reproduïble
- Pla per a alumnat avançat: reforçar onboarding o documentació tècnica del bloc

#### Setmana 5

- Focus o repte: arranque de `R2` com a flux de dades i processament, no com a simple infraestructura d'auth
- Què fa el professorat: modela formulari, validació visible, codi servidor integrat amb `HTML` o plantilla i primer tram de processament amb reutilització funcional de la dada correcta
- Què fa l'alumnat: tanca `R2M1` i `R2M2`, prepara l'acció del domini, usa variables i sentències simples en el flux i deixa la informació correcta disponible dins del projecte
- Materials per a l'alumnat: materials del Repte 2, apunt real del Repte 2, base comuna en `PHP`, guia de validació i errors
- Evidència mínima del bloc: dades recuperades, codi servidor integrat amb marques, variables o operadors aplicats, errors visibles, tractament correcte i primera reutilització funcional
- Checkpoint docent: evitar que `R2` es reduïsca a formularis d'accés o a persistència ornamental
- Pla per a alumnat endarrerit: un únic formulari, una única dada central i una sola reutilització funcional
- Pla per a alumnat avançat: incorporar fitxer o imatge amb control bàsic si el flux ho demana

#### Setmana 6

- Focus o repte: lògica del flux i estat temporal del `R2`
- Què fa el professorat: modela una regla recognoscible del domini, l'ús de variables, operadors i àmbits en eixa regla, i un ús d'estat, sessió o cookies amb sentit funcional
- Què fa l'alumnat: implementa `R2M3` i `R2M4`, deixa una decisió observable, recupera un pas o dada temporal del flux i comprova el document resultant generat pel servidor
- Materials per a l'alumnat: apunt real del Repte 2, guia de flux d'usuari i sessions, materials comuns
- Evidència mínima del bloc: regla del projecte aplicada, variables i operadors usats amb sentit, resposta servidor comprovada, estat recuperable i frontera clara entre estat i conservació funcional
- Checkpoint docent: comprovar que el producte ja resol comportament de domini, no només recepció de dades
- Pla per a alumnat endarrerit: reduir la funcionalitat a un sol cas d'ús complet i una única dada temporal útil
- Pla per a alumnat avançat: incorporar segona regla de negoci o millor tractament d'estat

#### Setmana 7

- Focus o repte: autenticació, funcionalitat protegida, prova mínima i checkpoint tècnic de `R2`
- Què fa el professorat: modela una operació protegida amb valor real del domini, un cas denegat i una prova curta del flux complet
- Què fa l'alumnat: implementa `R2M5` i `R2M6`, protegix una acció real, prova casos correctes i incorrectes i actualitza `README`
- Materials per a l'alumnat: guia de validació i errors del Repte 2, guia de testing i debugging, checklist del Repte 2
- Evidència mínima del bloc: operació del domini protegida, cas autoritzat, cas denegat, prova mínima i documentació reproduïble
- Checkpoint docent: no obrir la sessió final de `R2` sense evidència reproduïble del flux complet
- Pla per a alumnat endarrerit: tancar només el cas d'ús principal i els errors crítics
- Pla per a alumnat avançat: afegir proves més sistemàtiques o millor missatge d'error

#### Setmana 8

- Focus o repte: tancament de `R2`, primera peça testable i [microdefensa tècnica de criteris](programacio_aula_r2sx_microdefenses_tecniques_criteris.md)
- Què fa el professorat: reserva una primera franja per tancar `R2M7` i una segona per defensar evidències; força demo amb cas correcte i cas incorrecte, revisa `AI log`, commits i pregunta de contrast
- Què fa l'alumnat: crea una classe simple carregada amb Composer, executa una prova unitària mínima, prepara `3-5` diapositives i defensa formularis, validació, estat o funcionalitat protegida sobre el seu projecte
- Materials per a l'alumnat: full de treball del Repte 2, checklist del Repte 2, [microdefensa de R2](programacio_aula_r2sx_microdefenses_tecniques_criteris.md), [instrument comú de microdefenses](../03_avaluacio/microdefenses_tecniques_criteris.md)
- Producte mínim: flux de `R2` funcional, peça testable explicable i primer mapa de pas a `R3`
- Evidència mínima del bloc: demo, codi rellevant, traçabilitat, `AI log`, mini justificació i resposta a preguntes sobre entrada, validació, estat o protecció
- Checkpoint docent: validar autoria i comprensió real abans d'entrar a `R3`; si la defensa no acredita, es planifica recuperació curta
- Pla per a alumnat endarrerit: defensar un únic formulari complet amb validació de servidor, error visible i commit identificable
- Pla per a alumnat avançat: afegir prova negativa, fitxer controlat o comparativa abans/després més sòlida

#### Setmana 9

- Focus o repte: arrencada de `R3` com a reconstrucció en framework
- Què fa el professorat: modela l'arrencada d'un projecte en framework amb Docker, `.env`, ruta mínima, primera resposta generada pel framework, connexió inicial a BBDD i una comparació breu entre stacks, seguint la [planificació d'aula del Repte 3](planificacio_aula_r3_mvc_i_persistencia.md)
- Què fa l'alumnat: crea o estabilitza el projecte base en framework, compara l'opció triada amb una alternativa, justifica els avantatges de separar responsabilitats, declara els `2` casos d'ús de `R3`, identifica quin ve de `R2` i marca quin serà server-rendered
- Materials per a l'alumnat: materials del Repte 3, guia d'itinerari triada, guia de persistència i [planificació d'aula del Repte 3](planificacio_aula_r3_mvc_i_persistencia.md)
- Evidència mínima del bloc: framework arrancable amb Docker, `.env` documentat, ruta mínima o vista inicial, nota comparativa de stack, esquema abans/després i abast dels `2` fluxos registrat
- Checkpoint docent: comprovar que no és només un esquelet de framework i que almenys un flux ve de `R2`
- Pla per a alumnat endarrerit: stack més acotat, una ruta mínima i declaració clara dels dos fluxos abans d'obrir més funcionalitat
- Pla per a alumnat avançat: preparar ja el model de dades inicial i scripts d'arrencada més còmodes

#### Setmana 10

- Focus o repte: model de dades, `migrations` i `seeders`
- Què fa el professorat: modela una migració, un seeder o equivalent, una consulta que retorna un conjunt de dades i la comprovació que eixes dades alimenten una vista, llistat o resposta
- Què fa l'alumnat: defineix l'esquema mínim de dades, executa migracions, carrega dades inicials, recupera un conjunt de dades real i documenta com reconstruir la BBDD
- Materials per a l'alumnat: checklist del Repte 3, programació per repte, [planificació d'aula del Repte 3](planificacio_aula_r3_mvc_i_persistencia.md)
- Evidència mínima del bloc: BBDD real creada amb `migrations`, dades de demostració carregades amb `seeders` o equivalent, consulta de conjunt de dades i ús verificable en un flux
- Checkpoint docent: decidir si l'equip entra a l'avaluació 2 amb una base reproduïble, no amb dades carregades a mà
- Pla per a alumnat endarrerit: una sola entitat central, seeder mínim i lectura verificable
- Pla per a alumnat avançat: afegir relació simple o una segona migració controlada si no trenca l'abast

### Avaluació 2

#### Setmana 11

- Focus o repte: primer cas d'ús complet migrat de `R2`
- Què fa el professorat: modela el recorregut ruta, controlador, model o servei, vista o plantilla, validació, lectura real de BBDD i resposta `HTML` generada en servidor
- Què fa l'alumnat: migra o reconstrueix en el framework el primer cas d'ús heretat de `R2`, passa dades del controlador a una vista o resposta i el verifica de punta a punta
- Materials per a l'alumnat: apunt real del Repte 3, guia de persistència i modelat, [planificació d'aula del Repte 3](planificacio_aula_r3_mvc_i_persistencia.md)
- Evidència mínima del bloc: primer flux end-to-end amb dades reals, vista o plantilla server-rendered si és el flux triat, validació o error mínim i prova o verificació registrada
- Checkpoint docent: el flux ha de vindre de `R2` i no pot ser només una pantalla nova sense persistència
- Pla per a alumnat endarrerit: tancar un únic recorregut complet abans d'afegir camps o relacions
- Pla per a alumnat avançat: reforçar validació, proves o separació de servei sense canviar d'abast

#### Setmana 12

- Focus o repte: segon cas d'ús, estabilització i [microdefensa tècnica de `R3`](programacio_aula_r3sx_microdefenses_tecniques_criteris.md)
- Què fa el professorat: revisa fluxos, força prova de `migrations` i `seeders`, demana seguir una petició ruta-controlador-model/vista i activa defenses breus d'arquitectura aplicada
- Què fa l'alumnat: tanca el segon flux o ampliació útil, actualitza `README`, prepara defensa de separació de responsabilitats, persistència inicial o flux end-to-end
- Materials per a l'alumnat: checklist del Repte 3, itinerari triat, [planificació d'aula del Repte 3](planificacio_aula_r3_mvc_i_persistencia.md), [microdefensa de R3](programacio_aula_r3sx_microdefenses_tecniques_criteris.md)
- Producte mínim: aplicació en framework amb Docker, BBDD reconstruïble, dades inicials i almenys un flux complet server-rendered o equivalent
- Evidència mínima del bloc: demo end-to-end, codi de ruta/controlador/model/vista o servei, prova de dades, commits, `AI log` i justificació tècnica
- Checkpoint docent: validació formal d'entrada a `R4` només si l'alumne pot explicar el recorregut del flux
- Pla per a alumnat endarrerit: reduir el segon flux al mínim i defensar un únic recorregut complet
- Pla per a alumnat avançat: preparar contracte preliminar d'`API` o prova de regressió sense ampliar l'abast nuclear

#### Setmana 13

- Focus o repte: disseny del contracte d'`API`
- Què fa el professorat: modela recursos, endpoints, codis d'estat i errors coherents
- Què fa l'alumnat: decideix quina part rellevant del producte exposarà com a `API`
- Materials per a l'alumnat: materials del Repte 4, guia de contracte i disseny `API`
- Evidència mínima del bloc: contracte mínim d'`API` usable
- Checkpoint docent: comprovar que l'`API` respon a un cas d'ús real
- Pla per a alumnat endarrerit: limitar l'`API` a pocs endpoints nuclears
- Pla per a alumnat avançat: millorar model de resposta i errors o documentar més completament

#### Setmana 14

- Focus o repte: implementació dels endpoints principals
- Què fa el professorat: modela un endpoint complet amb entrada, eixida i error controlat
- Què fa l'alumnat: desenvolupa els endpoints nuclears del producte
- Materials per a l'alumnat: apunt real del Repte 4, itinerari triat reutilitzat en context d'`API`
- Evidència mínima del bloc: endpoints principals funcionals
- Checkpoint docent: revisar coherència de respostes i validacions
- Pla per a alumnat endarrerit: mantindre només operacions bàsiques del flux principal
- Pla per a alumnat avançat: afegir autenticació o permisos més clars a l'`API`

#### Setmana 15

- Focus o repte: documentació, consum i protecció verificable de l'`API`
- Què fa el professorat: modela col·lecció mínima de proves, client de consum, documentació curta i cas denegat o d'error
- Què fa l'alumnat: documenta, prova, consuma i ajusta el servei perquè el contracte siga usable i comprovable
- Materials per a l'alumnat: guia de proves i documentació `API`, apunt real del Repte 4, checklist del Repte 4
- Evidència mínima del bloc: documentació coherent, consum verificat, cas correcte, cas d'error i cas denegat si hi ha protecció
- Checkpoint docent: no reservar la microdefensa per arreglar l'API; la sessió següent és de verificació, no de construcció principal
- Pla per a alumnat endarrerit: documentació mínima i una prova clara del flux principal
- Pla per a alumnat avançat: millorar col·lecció de proves, permisos o qualitat del consumidor

#### Setmana 16

- Focus o repte: [microdefensa tècnica de `R4`](programacio_aula_r4sx_microdefenses_tecniques_criteris.md) i decisió inicial de pas a `R5`
- Què fa el professorat: verifica contracte, endpoint, autenticació o autorització, consum i documentació amb preguntes de contrast; al final mostra què és una integració amb valor real
- Què fa l'alumnat: defensa un servei real amb demo, prova correcta i prova d'error o denegació; després tria una possible integració externa o workflow `n8n` per a `R5`
- Materials per a l'alumnat: [microdefensa de R4](programacio_aula_r4sx_microdefenses_tecniques_criteris.md), guia de contracte i disseny `API`, guia de proves i documentació `API`, materials del Repte 5
- Producte mínim: API o servei usable, documentat, provat i amb control d'accés quan siga necessari
- Evidència mínima del bloc: contracte, demo de petició, codi d'endpoint o control d'accés, prova, commits, `AI log` i justificació
- Checkpoint docent: validació formal d'entrada a `R5`; si el servei no és consumible, la integració queda reduïda fins que el contracte siga estable
- Pla per a alumnat endarrerit: defensar un endpoint crític amb prova positiva i negativa
- Pla per a alumnat avançat: preparar integració amb millor control d'errors o consumidor més complet

#### Setmana 17

- Focus o repte: entrada a `R5`, selecció de font externa i disseny de la integració
- Què fa el professorat: modela criteris per triar una font o servei, un mapa origen-transformació-destí i un flux híbrid mínim
- Què fa l'alumnat: tria integració externa o workflow `n8n` amb sentit per al producte, defineix valor funcional i prepara la primera connexió
- Materials per a l'alumnat: materials del Repte 5, guia d'integració i automatització, guia d'ús verificable de la IA
- Evidència mínima del bloc: font triada, justificació, mapa d'integració, riscos i primer commit de preparació
- Checkpoint docent: evitar una integració ornamental o forçada
- Pla per a alumnat endarrerit: una integració mínima però real amb una sola entrada i eixida
- Pla per a alumnat avançat: definir també errors de flux i traçabilitat més fina

#### Setmana 18

- Focus o repte: implementació, transformació i prova del flux híbrid de `R5`
- Què fa el professorat: modela connexió, transformació de resposta, registre d'incidència i fallback quan el servei extern falla
- Què fa l'alumnat: implementa el flux híbrid, automatització o integració triada, transforma dades i registra proves
- Materials per a l'alumnat: apunt real del Repte 5, guies d'integració, automatització i testing
- Evidència mínima del bloc: flux híbrid executable, mapping o transformació, prova correcta, cas de fallada i traçabilitat
- Checkpoint docent: revisar que la integració aporta valor funcional real i no trenca el producte
- Pla per a alumnat endarrerit: tancar un únic recorregut de punta a punta
- Pla per a alumnat avançat: afegir observabilitat, control d'errors o pas addicional justificat

#### Setmana 19

- Focus o repte: proves, documentació i [microdefensa tècnica de `R5`](programacio_aula_r5sx_microdefenses_tecniques_criteris.md)
- Què fa el professorat: guia revisió de punta a punta, demana registre d'errors, verifica `README`, `AI log` i activa defenses breus de la integració
- Què fa l'alumnat: prova el flux complet, documenta errors, defensa integració, interoperabilitat, transformació, proves o preparació de defensa final
- Materials per a l'alumnat: checklist del Repte 5, [microdefensa de R5](programacio_aula_r5sx_microdefenses_tecniques_criteris.md), instruments de seguiment docent, guió de defensa final
- Producte mínim: integració provada, documentada i connectada amb valor real del producte
- Evidència mínima del bloc: demo del flux complet, codi o workflow rellevant, prova o registre d'incidència, commits, `AI log` i justificació tècnica
- Checkpoint docent: validar que el producte és ja defensable i separar incidències de recuperació de millores opcionals
- Pla per a alumnat endarrerit: renunciar a extensions i estabilitzar el flux complet que realment funciona
- Pla per a alumnat avançat: reforçar proves, observabilitat, desplegament o narrativa de trade-offs

#### Setmana 20

- Focus o repte: tancament del producte i del curs
- Què fa el professorat: fa la defensa final, revisa coherència del repositori, activa recollida de feedback i tanca pilotatge docent del grup
- Què fa l'alumnat: presenta, defensa, entrega evidències finals, declara ús d'IA i aporta feedback del curs
- Materials per a l'alumnat: rúbrica de defensa, sistema d'evidències, plantilla de feedback de pilotatge, documents finals del curs
- Evidència mínima del bloc: producte final defensat, feedback recollit i estat final registrat
- Checkpoint docent: tancament del curs dins de les dues primeres avaluacions, amb microdefenses prèvies ja resoltes o registrades com a recuperació
- Pla per a alumnat endarrerit: defensa ajustada al mínim funcional no trivial assolit
- Pla per a alumnat avançat: proposta de millora o `v2` ben acotada, sense confondre-la amb el lliurable nuclear

## Definition of done del document

Este document es considera completat quan:

- tradueix la seqüència del curs a `20` blocs setmanals o equivalents
- manté el desenvolupament principal del projecte dins de les dues primeres avaluacions
- indica per a cada bloc focus, paper del professorat, paper de l'alumnat, materials, evidència mínima, checkpoint i plans de suport i ampliació
- deixa clar com s'articulen classe guiada, modelatge i autonomia
- incorpora criteri explícit per a alumnat endarrerit i alumnat avançat
- és usable com a guia docent real sense haver de reconstruir el recorregut des de documents dispersos
