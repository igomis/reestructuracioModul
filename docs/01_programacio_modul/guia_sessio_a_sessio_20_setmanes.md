# Guia sessió a sessió del curs en 20 setmanes

## Finalitat del document

Convertir la implantació del mòdul en una guia docent setmanal usable, pensada perquè el professorat puga saber què convé explicar, què modelar, què deixar a autonomia i com adaptar el ritme segons el progrés real de l'alumnat.

Esta peça complementa [programacio_aula_per_repte.md](programacio_aula_per_repte.md), [seqüenciacio_sessions_2_avaluacions.md](seqüenciacio_sessions_2_avaluacions.md) i [pla_execucio_pilotatge_real.md](../00_visio_general/pla_execucio_pilotatge_real.md). Aquells documents fixen la lògica global i els checkpoints; esta guia baixa el model a una lectura setmanal o de bloc docent real.

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
- el criteri principal no és “arribar a tot”, sinó mantindre la progressió real del producte i la seua defensa tècnica dins de les dues primeres avaluacions

## Estructura general del curs

- `Avaluació 1` (`setmanes 1-10 / ~60h`): marc comú, `R1`, `R2` i entrada real a `R3`
- `Avaluació 2` (`setmanes 11-20 / ~60h`): tancament de `R3`, `R4`, `R5` i defensa final
- `Avaluació 3`: sense desenvolupament central del projecte; només seguiment residual, connexió amb empresa o `FCT`

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
- Què fa el professorat: modela formulari, validació visible i primer tram de processament amb reutilització funcional de la dada correcta
- Què fa l'alumnat: tanca `MP1` i `MP2`, prepara l'acció del domini i deixa la informació correcta disponible dins del projecte
- Materials per a l'alumnat: materials del Repte 2, apunt real del Repte 2, base comuna en `PHP`, guia de validació i errors
- Evidència mínima del bloc: dades recuperades, errors visibles, tractament correcte i primera reutilització funcional
- Checkpoint docent: evitar que `R2` es reduïsca a formularis d'accés o a persistència ornamental
- Pla per a alumnat endarrerit: un únic formulari, una única dada central i una sola reutilització funcional
- Pla per a alumnat avançat: incorporar fitxer o imatge amb control bàsic si el flux ho demana

#### Setmana 6

- Focus o repte: lògica del flux i estat temporal del `R2`
- Què fa el professorat: modela una regla recognoscible del domini i un ús d'estat, sessió o cookies amb sentit funcional
- Què fa l'alumnat: implementa `MP3` i `MP4`, deixa una decisió observable i recupera un pas o dada temporal del flux
- Materials per a l'alumnat: apunt real del Repte 2, guia de flux d'usuari i sessions, materials comuns
- Evidència mínima del bloc: regla del projecte aplicada, estat recuperable i frontera clara entre estat i conservació funcional
- Checkpoint docent: comprovar que el producte ja resol comportament de domini, no només recepció de dades
- Pla per a alumnat endarrerit: reduir la funcionalitat a un sol cas d'ús complet i una única dada temporal útil
- Pla per a alumnat avançat: incorporar segona regla de negoci o millor tractament d'estat

#### Setmana 7

- Focus o repte: autenticació, funcionalitat protegida, prova mínima i checkpoint tècnic de `R2`
- Què fa el professorat: modela una operació protegida amb valor real del domini, un cas denegat i una prova curta del flux complet
- Què fa l'alumnat: implementa `MP5` i `MP6`, protegix una acció real, prova casos correctes i incorrectes i actualitza `README`
- Materials per a l'alumnat: guia de validació i errors del Repte 2, guia de testing i debugging, checklist del Repte 2
- Evidència mínima del bloc: operació del domini protegida, cas autoritzat, cas denegat, prova mínima i documentació reproduïble
- Checkpoint docent: no obrir la sessió final de `R2` sense evidència reproduïble del flux complet
- Pla per a alumnat endarrerit: tancar només el cas d'ús principal i els errors crítics
- Pla per a alumnat avançat: afegir proves més sistemàtiques o millor missatge d'error

#### Setmana 8

- Focus o repte: sessió final de `R2` amb refactorització, organització en fitxers amb `include` / `require`, primer objecte de domini i primer mapa de pas a `R3`
- Què fa el professorat: modela una refactorització curta del codi ja funcional, mostra com separar funcions comunes en fitxers, explica la diferència bàsica entre `include`, `require`, `include_once` i `require_once`, introduïx un objecte simple del domini i delimita què encara queda reservat a `R3`
- Què fa l'alumnat: implementa `MP7`, reorganitza una part del codi en fitxers, usa `include` / `require` amb sentit, incorpora una entitat mínima del domini com a objecte simple, compara abans/després, justifica la millora i identifica el primer punt de pas a arquitectura
- Materials per a l'alumnat: full de treball del Repte 2, checklist del Repte 2, materials del Repte 3 com a lectura de transició
- Evidència mínima del bloc: comparativa breu abans/després, almenys un fitxer comú importat amb criteri, objecte simple del domini, justificació de mantenibilitat i primer mapa de pas a `R3`
- Checkpoint docent: validar que el pas a `R3` es fa sobre un flux real i una revisió final explicable
- Pla per a alumnat endarrerit: centrar-se en una sola entitat i un sol cas d'ús
- Pla per a alumnat avançat: reforçar la separació de responsabilitats sense saltar encara a capes completes ni a persistència com a focus central

#### Setmana 9

- Focus o repte: arquitectura i persistència inicials
- Què fa el professorat: modela una refactorització curta a capes o equivalent i la primera entitat persistent
- Què fa l'alumnat: inicia el pas a arquitectura mantenible i persistència real
- Materials per a l'alumnat: materials del Repte 3, itinerari triat com a suport de persistència
- Evidència mínima del bloc: primera entitat persistent i estructura refactoritzada recognoscible
- Checkpoint docent: comprovar que la persistència no és només decorativa
- Pla per a alumnat endarrerit: prioritzar una única entitat persistent i un servei o equivalent
- Pla per a alumnat avançat: afegir relació simple o capa de servei més robusta

#### Setmana 10

- Focus o repte: tancament de la primera avaluació amb `R3` obert
- Què fa el professorat: revisa estat del producte, persistència mínima i riscos per a l'avaluació 2
- Què fa l'alumnat: tanca el primer tram de `R3`, documenta estat i prepara el pas a la segona avaluació
- Materials per a l'alumnat: checklist del Repte 3, programació per repte
- Evidència mínima del bloc: flux funcional existent ja persistent o clarament encaminat a ser-ho
- Checkpoint docent: decidir si l'equip entra a l'avaluació 2 amb base suficient
- Pla per a alumnat endarrerit: freeze de noves funcionalitats i consolidació d'una sola peça persistent
- Pla per a alumnat avançat: afinar model de dades o començar proves de regressió més clares

### Avaluació 2

#### Setmana 11

- Focus o repte: consolidació de persistència i regressió
- Què fa el professorat: modela comprovació de regressió sobre el flux ja refactoritzat
- Què fa l'alumnat: completa persistència i valida que el flux principal continua viu
- Materials per a l'alumnat: apunt real del Repte 3, guia de persistència i modelat
- Evidència mínima del bloc: cas d'ús principal persistent i verificat
- Checkpoint docent: no obrir `R4` sense base estable
- Pla per a alumnat endarrerit: assegurar només un flux persistent sencer
- Pla per a alumnat avançat: reforçar proves o segona lectura d'arquitectura

#### Setmana 12

- Focus o repte: tancament formal de `R3`
- Què fa el professorat: revisa decisions d'arquitectura i model de dades; acota què farà de nucli d'`API`
- Què fa l'alumnat: tanca capes o equivalent, `README` tècnic i proves mínimes
- Materials per a l'alumnat: checklist del Repte 3, itinerari triat
- Evidència mínima del bloc: `R3` explicable, persistent i defensable
- Checkpoint docent: validació formal d'entrada a `R4`
- Pla per a alumnat endarrerit: tancar un únic flux persistent i ajornar millores no nuclears
- Pla per a alumnat avançat: preparar ja contracte preliminar d'`API`

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

- Focus o repte: documentació i consum de l'`API`
- Què fa el professorat: modela col·lecció mínima de proves o client de consum i una documentació curta però usable
- Què fa l'alumnat: documenta, prova i consuma la seua `API`
- Materials per a l'alumnat: guia de proves i documentació `API`, apunt real del Repte 4
- Evidència mínima del bloc: documentació coherent i consum verificat
- Checkpoint docent: tancament de `R4` només si hi ha contracte usable per tercers
- Pla per a alumnat endarrerit: documentació mínima i una prova clara del flux principal
- Pla per a alumnat avançat: millorar col·lecció de proves o qualitat del consumidor

#### Setmana 16

- Focus o repte: entrada a `R5`, decisió d'integració
- Què fa el professorat: explica què és una integració amb valor real i modela un flux híbrid mínim
- Què fa l'alumnat: tria integració externa o workflow `n8n` amb sentit per al producte
- Materials per a l'alumnat: materials del Repte 5, guia d'integració i automatització
- Evidència mínima del bloc: flux híbrid dissenyat i justificat
- Checkpoint docent: evitar una integració ornamental o forçada
- Pla per a alumnat endarrerit: una integració mínima però real amb una sola entrada i eixida
- Pla per a alumnat avançat: tractar també errors de flux i traçabilitat més fina

#### Setmana 17

- Focus o repte: implementació del flux híbrid
- Què fa el professorat: modela un workflow bàsic i recorda criteri d'incident i mantenibilitat
- Què fa l'alumnat: implementa el flux híbrid, automatització o integració triada
- Materials per a l'alumnat: apunt real del Repte 5, guia `n8n` i automatització
- Evidència mínima del bloc: flux híbrid parcial ja executable
- Checkpoint docent: revisar que la integració aporta valor funcional real
- Pla per a alumnat endarrerit: tancar un únic recorregut de punta a punta
- Pla per a alumnat avançat: afegir control d'errors o pas addicional justificat

#### Setmana 18

- Focus o repte: proves, incidències i tancament de `R5`
- Què fa el professorat: guia revisió de punta a punta, demana registre d'errors i ajusta tancament
- Què fa l'alumnat: prova el flux complet, documenta errors i tanca documentació final
- Materials per a l'alumnat: checklist del Repte 5, instruments de seguiment docent
- Evidència mínima del bloc: integració provada i documentada
- Checkpoint docent: validar que el producte és ja defensable
- Pla per a alumnat endarrerit: renunciar a extensions i estabilitzar el flux complet
- Pla per a alumnat avançat: reforçar proves, observabilitat o defensa tècnica

#### Setmana 19

- Focus o repte: preparació de defensa final
- Què fa el professorat: modela defensa curta, recorregut del repositori i ús verificable de la IA
- Què fa l'alumnat: prepara narrativa tècnica, revisa `README`, `AI log` i evidències finals
- Materials per a l'alumnat: rúbrica de defensa tècnica, sistema d'evidències
- Evidència mínima del bloc: defensa assajada i repositori final coherent
- Checkpoint docent: detectar punts dèbils abans del tancament definitiu
- Pla per a alumnat endarrerit: centrar-se en el flux principal i en la defensa del que realment funciona
- Pla per a alumnat avançat: millorar narrativa de trade-offs i justificació de decisions

#### Setmana 20

- Focus o repte: tancament del producte i del curs
- Què fa el professorat: fa la revisió final, activa recollida de feedback i tanca pilotatge docent del grup
- Què fa l'alumnat: presenta, defensa, entrega evidències finals i aporta feedback del curs
- Materials per a l'alumnat: rúbrica de defensa, plantilla de feedback de pilotatge, documents finals del curs
- Evidència mínima del bloc: producte final defensat, feedback recollit i estat final registrat
- Checkpoint docent: tancament del curs dins de les dues primeres avaluacions
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
