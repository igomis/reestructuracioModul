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
- el treball compartit pot existir, però cada alumne ha de mantindre rastre propi, evidència pròpia i capacitat de defensa individual

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
- Pla per a alumnat avançat: justificar dues alternatives de domini o stack abans de decidir

#### Setmana 2

- Focus o repte: domini, stack i decisió tècnica inicial
- Què fa el professorat: modela una decisió tècnica breu, exemplifica un `ADR` curt i acota què no és suficient en `R1`
- Què fa l'alumnat: tria domini, itinerari i primer cas d'ús mínim del producte
- Materials per a l'alumnat: fitxa del Repte 1, itineraris tecnològics, guia `README` i `ADR`
- Evidència mínima del bloc: domini triat, decisió tècnica justificada i traçabilitat inicial
- Checkpoint docent: validar que hi ha producte pensat, no només framework triat
- Pla per a alumnat endarrerit: domini més acotat i un sol cas d'ús d'entrada
- Pla per a alumnat avançat: explorar riscos i trade-offs de la decisió tècnica

#### Setmana 3

- Focus o repte: `R1` com a primera peça funcional real
- Què fa el professorat: modela una landing page o equivalent i un formulari mínim amb validació bàsica
- Què fa l'alumnat: implementa la primera entrada funcional del producte
- Materials per a l'alumnat: apunt real del Repte 1, materials comuns i suport de l'itinerari triat
- Evidència mínima del bloc: pàgina inicial funcional i formulari bàsic operatiu
- Checkpoint docent: revisar que hi ha interacció real del producte
- Pla per a alumnat endarrerit: formulari amb menys camps i un flux més curt
- Pla per a alumnat avançat: afegir validació més robusta o millor feedback d'errors

#### Setmana 4

- Focus o repte: validació de servidor i primer registre de dades
- Què fa el professorat: modela resposta correcta i incorrecta, i exemplifica com deixar rastre al `README`
- Què fa l'alumnat: completa validació mínima al servidor i registra o persistix la primera dada útil del domini
- Materials per a l'alumnat: apunt real del Repte 1, guia de testing i debugging
- Evidència mínima del bloc: flux `R1` reproduïble amb validació i primer registre verificable
- Checkpoint docent: tancament de `R1` només si no és un esquelet buit
- Pla per a alumnat endarrerit: una sola validació obligatòria i un únic camí de registre
- Pla per a alumnat avançat: reforçar persistència bàsica o documentació tècnica del bloc

#### Setmana 5

- Focus o repte: arranque de `R2`, autenticació com a infraestructura
- Què fa el professorat: explica diferència entre auth, autorització i flux funcional del domini; modela alta o login mínim
- Què fa l'alumnat: prepara usuaris, estat equivalent i punt d'entrada al primer flux autenticat
- Materials per a l'alumnat: materials del Repte 2, apunt real del Repte 2, itinerari triat
- Evidència mínima del bloc: registre o login operatiu i cas d'ús de domini identificat
- Checkpoint docent: evitar que `R2` es reduïsca a formularis d'accés
- Pla per a alumnat endarrerit: un únic actor i una única operació protegida
- Pla per a alumnat avançat: definir també una primera restricció de rol o regla de negoci

#### Setmana 6

- Focus o repte: funcionalitat de negoci autenticada
- Què fa el professorat: modela una operació protegida amb valor real del domini i una restricció recognoscible
- Què fa l'alumnat: implementa el primer flux funcional autenticat del producte
- Materials per a l'alumnat: apunt real del Repte 2, materials comuns
- Evidència mínima del bloc: operació del domini protegida i usable
- Checkpoint docent: comprovar que el producte ja resol una acció real, no només auth
- Pla per a alumnat endarrerit: reduir la funcionalitat a un sol cas d'ús complet
- Pla per a alumnat avançat: incorporar segona regla de negoci o millor control d'accés

#### Setmana 7

- Focus o repte: validacions, errors i proves mínimes de `R2`
- Què fa el professorat: modela tractament d'errors i una prova mínima del flux complet
- Què fa l'alumnat: reforça validacions, prova casos correctes i casos límit, actualitza `README`
- Materials per a l'alumnat: guia de validació i errors del Repte 2, guia de testing i debugging
- Evidència mínima del bloc: flux de `R2` verificat amb errors controlats
- Checkpoint docent: no obrir `R3` sense evidència reproduïble
- Pla per a alumnat endarrerit: tancar només el cas d'ús principal i els errors crítics
- Pla per a alumnat avançat: afegir proves més sistemàtiques o millor missatge d'error

#### Setmana 8

- Focus o repte: tancament de `R2` i entrada a `R3`
- Què fa el professorat: explica què s'ha de refactoritzar primer i per què `R3` no és “fer MVC”
- Què fa l'alumnat: identifica punt de refactorització, entitats i model mínim del domini
- Materials per a l'alumnat: materials del Repte 3, apunt real del Repte 3
- Evidència mínima del bloc: mapa de refactorització i primer model de dades
- Checkpoint docent: validar que el pas a `R3` es fa sobre un flux real
- Pla per a alumnat endarrerit: centrar-se en una sola entitat i un sol cas d'ús
- Pla per a alumnat avançat: preparar relació addicional o separació més clara de capes

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
