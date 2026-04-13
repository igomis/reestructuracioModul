# Kit de pilotatge de les setmanes 9-12

## Finalitat del document

Completar un primer bloc pilotable del curs fins al tancament de la primera avaluació, de manera que el professorat puga conduir l'entrada real a `R3`, els primers canvis d'arquitectura i persistència i el checkpoint de tancament sense haver de reconstruir este tram a partir de documents separats.

Este kit prolonga la capa operativa iniciada en els trams `1-4` i `5-8`. La seua funció és traduir les setmanes `9-12` a una pauta de pilotatge real: què convé explicar, què s'ha de modelar, què ha de produir l'alumnat, què s'ha de verificar per alumne i què convé registrar per decidir si la primera avaluació queda realment tancada.

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
- `R3` no es considera obert de manera seriosa si `R2` encara no té un mínim funcional no trivial clarament defensable
- si en una setmana no apareix l'evidència mínima, cal prioritzar reconducció abans d'obrir noves capes de persistència o arquitectura

## Estructura del tram 9-12

- `Setmana 9`: tancament fort del mínim funcional no trivial de `R2` i entrada explícita a `R3`
- `Setmana 10`: separació de responsabilitats i primers canvis d'arquitectura sobre un flux real
- `Setmana 11`: persistència coherent i validació lligada al domini
- `Setmana 12`: checkpoint de tancament de la primera avaluació i decisió de pas

## Peces que s'activen en este tram

- [kit_pilotatge_setmanes_01_04.md](kit_pilotatge_setmanes_01_04.md)
- [kit_pilotatge_setmanes_05_08.md](kit_pilotatge_setmanes_05_08.md)
- [guia_sessio_a_sessio_20_setmanes.md](guia_sessio_a_sessio_20_setmanes.md)
- [annex_suport_i_ampliacio_ritmes.md](annex_suport_i_ampliacio_ritmes.md)
- [pla_execucio_pilotatge_real.md](../00_visio_general/pla_execucio_pilotatge_real.md)
- [repte_02_materials_sessio.md](../04_materials/materials_aula/repte_02_materials_sessio.md)
- [repte_03_materials_sessio.md](../04_materials/materials_aula/repte_03_materials_sessio.md)
- [mini_briefings_setmanals.md](../04_materials/materials_aula/mini_briefings_setmanals.md)
- [checkpoints_curts_aula.md](../04_materials/materials_aula/checkpoints_curts_aula.md)
- [plantilles_feedback_rapid.md](../04_materials/materials_aula/plantilles_feedback_rapid.md)
- [fulls_treball_base.md](../04_materials/materials_aula/fulls_treball_base.md)
- [plantilla_recollida_feedback_pilotatge.md](../03_avaluacio/plantilla_recollida_feedback_pilotatge.md)
- [registre_incidents_i_ajustos_pilotatge.md](../03_avaluacio/registre_incidents_i_ajustos_pilotatge.md)

## Planificació operativa per setmanes

### Setmana 9

- Objectiu docent: tancar amb força el mínim funcional no trivial de `R2` i obrir `R3` sobre una base funcional real
- Focus o repte: tancament fort de `R2` i entrada explícita a `R3`
- Què explica el professorat: què ha de quedar clarament assolit a `R2`, per què no n'hi ha prou amb auth aparent i com seleccionar la funcionalitat del producte que val la pena professionalitzar a `R3`
- Què modela en directe: revisió d'un flux autenticat ja defensable, identificació de parts fràgils i pas del cas d'ús protegit a un candidat real de refactorització
- Què fa l'alumnat: reforça el flux autenticat principal, tanca errors i validacions pendents, identifica el cas d'ús que entrarà a `R3` i deixa rastre individual de què pot explicar i reproduir
- Materials concrets que s'activen: [kit_pilotatge_setmanes_05_08.md](kit_pilotatge_setmanes_05_08.md), [repte_02_materials_sessio.md](../04_materials/materials_aula/repte_02_materials_sessio.md), [repte_03_materials_sessio.md](../04_materials/materials_aula/repte_03_materials_sessio.md), guies comunes de testing/debugging i `README`
- Evidència mínima a arreplegar: flux de `R2` complet, error mínim controlat, cas d'ús de `R3` triat i justificat individualment
- Checkpoint docent: validar si cada alumne pot defensar `R2` com a funcionalitat de negoci real i explicar quina part passarà a `R3`
- Intervenció per alumnat endarrerit: congelar qualsevol ampliació, reduir a un únic flux autenticat i fixar una sola operació a professionalitzar
- Ampliació per alumnat avançat: anticipar un mapa curt de responsabilitats o una primera lectura de model de dades sense obrir encara canvis extensos
- Què s'ha de registrar al pilotatge: si el tancament real de `R2` arriba dins del temps previst, quins alumnes encara es queden en una lectura superficial del repte i quins patrons de bloqueig es repetixen

### Setmana 10

- Objectiu docent: obrir `R3` amb separació de responsabilitats recognoscible i canvi d'arquitectura amb sentit
- Focus o repte: primers canvis d'arquitectura i refactorització útil
- Què explica el professorat: què vol dir separar responsabilitats en cada itinerari, per què el repte no és “fer MVC” i com evitar refactoritzacions cosmètiques
- Què modela en directe: un mapa curt de capes o equivalent, una operació central del domini i la seua redistribució a una estructura més mantingible
- Què fa l'alumnat: reorganitza una funcionalitat real del producte, identifica responsabilitats, reubica lògica i deixa el flux principal encara executable
- Materials concrets que s'activen: [repte_03_materials_sessio.md](../04_materials/materials_aula/repte_03_materials_sessio.md), [fulls_treball_base.md](../04_materials/materials_aula/fulls_treball_base.md), [checkpoints_curts_aula.md](../04_materials/materials_aula/checkpoints_curts_aula.md) i l'itinerari triat
- Evidència mínima a arreplegar: estructura refactoritzada recognoscible, operació principal encara viva i justificació individual del canvi
- Checkpoint docent: comprovar que la nova estructura millora un flux real i que cada alumne pot explicar quina responsabilitat s'ha separat i per què
- Intervenció per alumnat endarrerit: limitar la refactorització a una sola operació i ajornar tota reorganització lateral
- Ampliació per alumnat avançat: afinar noms, serveis o límits entre capes, o deixar una primera prova de regressió millor definida
- Què s'ha de registrar al pilotatge: si el grup entén `R3` com a professionalització del producte o torna a una lectura purament tècnica, i quin itinerari necessita més modelatge docent

### Setmana 11

- Objectiu docent: fer persistent el flux principal de manera coherent amb el domini i amb validació lligada al model
- Focus o repte: persistència coherent i validació lligada al domini
- Què explica el professorat: com passar d'una operació refactoritzada a una operació persistent, quina relació hi ha entre model, validació i cas d'ús, i per què “guardar dades” no és suficient
- Què modela en directe: una primera entitat persistent, una operació de lectura o escriptura coherent i una validació vinculada al model del domini
- Què fa l'alumnat: crea o consolida la primera entitat persistent del flux principal, ajusta validació lligada al domini i prova que el cas d'ús continua funcionant
- Materials concrets que s'activen: [repte_03_materials_sessio.md](../04_materials/materials_aula/repte_03_materials_sessio.md), guia de persistència i modelat, guia de testing/debugging i [plantilles_feedback_rapid.md](../04_materials/materials_aula/plantilles_feedback_rapid.md)
- Evidència mínima a arreplegar: registre persistent del domini, validació coherent i prova reproduïble del flux principal
- Checkpoint docent: validar si cada alumne pot explicar quina entitat, quina operació i quina validació està realment sostenint
- Intervenció per alumnat endarrerit: una sola entitat, una sola operació i una sola validació nuclear; congelar relacions i extensions
- Ampliació per alumnat avançat: afegir una relació del domini, una prova de regressió millor tancada o una lectura més robusta de servei/capa
- Què s'ha de registrar al pilotatge: si la persistència entra amb càrrega raonable, quins errors apareixen per itinerari i si la validació lligada al domini resulta prou comprensible per a l'alumnat

### Setmana 12

- Objectiu docent: tancar la primera avaluació amb un checkpoint fort de `R3` inicial i decisió de pas
- Focus o repte: checkpoint de tancament de la 1a avaluació
- Què explica el professorat: què compta com a tancament suficient del primer bloc, quins mínims s'han d'haver assolit per entrar amb sentit a la segona avaluació i com es diferencia un producte viu d'un producte aparent
- Què modela en directe: lectura de checkpoint amb evidències individuals, revisió d'estat del producte, de traçabilitat i de part defensable del flux persistent
- Què fa l'alumnat: tanca documentació mínima, prepara evidències individuals, mostra el punt real del producte i deixa registrada la part del treball que pot explicar i defensar
- Materials concrets que s'activen: [repte_03_materials_sessio.md](../04_materials/materials_aula/repte_03_materials_sessio.md), [plantilla_recollida_feedback_pilotatge.md](../03_avaluacio/plantilla_recollida_feedback_pilotatge.md), [registre_incidents_i_ajustos_pilotatge.md](../03_avaluacio/registre_incidents_i_ajustos_pilotatge.md) i instruments de seguiment docent
- Evidència mínima a arreplegar: flux principal persistent o clarament encaminat a ser-ho, `README` actualitzat, prova mínima i checkpoint individual tancat
- Checkpoint docent: decidir si cada alumne entra a la 2a avaluació amb base suficient o si necessita reconducció explícita
- Intervenció per alumnat endarrerit: freeze de noves funcionalitats, consolidació d'una sola operació persistent i pla curt de recuperació per a l'entrada a la 2a avaluació
- Ampliació per alumnat avançat: afinar model de dades, claredat d'arquitectura o primera idea de contracte d'`API`, sense obrir encara `R4`
- Què s'ha de registrar al pilotatge: balanç de càrrega de la 1a avaluació, punts d'estrangulament, ajustos immediats per a la segona avaluació i si el bloc inicial del curs ha sigut realment pilotable de punta a punta

## Registre mínim de pilotatge per al tram 9-12

Per a les setmanes `9-12`, convé deixar com a mínim:

- una nota setmanal per alumne amb estat real, bloqueig principal i decisió docent següent
- una síntesi de si `R2` queda realment tancat i de si `R3` s'obri sobre base prou estable
- almenys una entrada de feedback al tancament de la primera avaluació
- una entrada al registre d'incidents si apareixen patrons recurrents en arquitectura, persistència, validació lligada al domini o càrrega temporal

## Criteri de pas a la setmana 13

Només convé entrar al bloc següent si:

- el mínim funcional no trivial de `R2` ha quedat clarament superat
- hi ha una funcionalitat persistent recognoscible o una base molt clara per tancar-la immediatament en l'inici de la 2a avaluació
- cada alumne pot explicar i defensar la seua part del flux refactoritzat o persistent
- el `README`, la traçabilitat i les evidències permeten entendre el punt real del producte al final de la primera avaluació

## Definition of done del document

Este kit es considera completat quan:

- concreta les setmanes `9-12` com a tercer tram operatiu del curs
- indica per a cada setmana objectiu, paper docent, treball de l'alumnat, materials activats, evidència mínima, checkpoint, suport, ampliació i registre de pilotatge
- connecta el tancament fort de `R2`, l'entrada explícita a `R3`, la persistència inicial i el checkpoint final de la primera avaluació
- deixa clar que pot haver-hi cooperació tècnica coordinada, però que l'evidència, la verificació i la defensa són individuals
- deixa la primera avaluació quasi completament pilotable com a bloc docent real
