# Kit de pilotatge de les setmanes 17-20

## Finalitat del document
Completar la seqüència pilotable de les dues primeres avaluacions amb un paquet usable per al tram `17-20`, de manera que el professorat puga obrir `R5` de manera explícita, conduir la integració híbrida o automatització útil, verificar el flux complet, tancar la defensa final individual i deixar també tancat el pilotatge del producte.

Este kit prolonga la capa operativa iniciada en els trams `1-4`, `5-8`, `9-12` i `13-16`. La seua funció és traduir les setmanes `17-20` a una pauta de pilotatge real: què convé explicar, què s'ha de modelar, què ha de produir l'alumnat, què s'ha de verificar per alumne i què convé registrar per decidir si el curs queda realment pilotable de punta a punta dins de les dues avaluacions.

El tram assumix que el bloc `13-16` ha deixat `R4` prou tancat i ha identificat una necessitat real d'integració, però no dona per feta encara la solidesa del flux final; per això la setmana `17` funciona com a entrada explícita a `R5` i com a confirmació que la integració triada té valor real abans de convertir-la en tancament del curs.

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
- pot haver-hi context de producte compartit o moments de treball coordinat, però l'evidència, la verificació, la defensa i la decisió docent s'han de resoldre individualment
- `R5` no s'ha d'entendre com a “fer `n8n`” ni com a demo visual d'automatització; només té sentit si resol una necessitat real del producte reutilitzant l'`API` publicada
- la IA es pot usar com a eina guiada per mapar payloads, diagnosticar errors, preparar proves o documentació, però qualsevol ús ha de quedar verificat, registrat i defensable individualment
- si en una setmana no apareix l'evidència mínima, cal prioritzar reconducció abans d'avançar cap a defensa final o tancament del pilotatge

## Estructura del tram 17-20
- `Setmana 17`: entrada explícita a `R5` i definició final de la necessitat real d'integració
- `Setmana 18`: implementació del flux híbrid o automatització útil
- `Setmana 19`: proves, documentació del flux complet i preparació forta de defensa individual
- `Setmana 20`: defensa final individual i tancament del producte i del pilotatge

## Peces que s'activen en este tram
- [kit_pilotatge_setmanes_13_16.md](kit_pilotatge_setmanes_13_16.md)
- [guia_sessio_a_sessio_20_setmanes.md](guia_sessio_a_sessio_20_setmanes.md)
- [annex_suport_i_ampliacio_ritmes.md](annex_suport_i_ampliacio_ritmes.md)
- [pla_execucio_pilotatge_real.md](../00_visio_general/pla_execucio_pilotatge_real.md)
- [repte_05_materials_sessio.md](../04_materials/materials_aula/repte_05_materials_sessio.md)
- [guia_integracio_externa_i_flux_hibrid.md](../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md)
- [guia_n8n_i_automatitzacio.md](../04_materials/repte_05/guia_n8n_i_automatitzacio.md)
- [checklist_repte_05.md](../04_materials/repte_05/checklist_repte_05.md)
- [repte_05_integracio_hibrida_n8n.md](../04_materials/apunts_reals/repte_05_integracio_hibrida_n8n.md)
- [rubrica_base_reptes.md](../03_avaluacio/rubrica_base_reptes.md)
- [rubrica_defensa_tecnica.md](../03_avaluacio/rubrica_defensa_tecnica.md)
- [instruments_seguiment_docent.md](../03_avaluacio/instruments_seguiment_docent.md)
- [sistema_evidencies.md](../03_avaluacio/sistema_evidencies.md)
- [mini_briefings_setmanals.md](../04_materials/materials_aula/mini_briefings_setmanals.md)
- [checkpoints_curts_aula.md](../04_materials/materials_aula/checkpoints_curts_aula.md)
- [plantilles_feedback_rapid.md](../04_materials/materials_aula/plantilles_feedback_rapid.md)
- [fulls_treball_base.md](../04_materials/materials_aula/fulls_treball_base.md)
- [plantilla_recollida_feedback_pilotatge.md](../03_avaluacio/plantilla_recollida_feedback_pilotatge.md)
- [registre_incidents_i_ajustos_pilotatge.md](../03_avaluacio/registre_incidents_i_ajustos_pilotatge.md)

## Planificació operativa per setmanes
### Setmana 17
- Objectiu docent: obrir `R5` de manera explícita i validar que la integració triada respon a una necessitat real del producte
- Focus o repte: entrada explícita a `R5` i definició final de la necessitat real d'integració
- Què explica el professorat: què compta com a integració amb valor real, per què no n'hi ha prou amb un workflow visible i com reconnectar `R5` amb el contracte d'`API`, el domini i el tancament professional del producte
- Què modela en directe: selecció d'un esdeveniment real del domini, mapatge d'entrada, consum d'`API`, transformació mínima i eixida observable, deixant clar també quin error rellevant convé controlar des del principi
- Què fa l'alumnat: valida individualment la necessitat real que resoldrà, defineix el flux d'entrada i eixida, identifica l'endpoint o recurs d'`API` que reutilitzarà i deixa documentada la decisió d'integració amb criteri defensable
- Materials concrets que s'activen: [kit_pilotatge_setmanes_13_16.md](kit_pilotatge_setmanes_13_16.md), [repte_05_materials_sessio.md](../04_materials/materials_aula/repte_05_materials_sessio.md), [guia_integracio_externa_i_flux_hibrid.md](../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md), [guia_n8n_i_automatitzacio.md](../04_materials/repte_05/guia_n8n_i_automatitzacio.md), [rubrica_base_reptes.md](../03_avaluacio/rubrica_base_reptes.md) i [instruments_seguiment_docent.md](../03_avaluacio/instruments_seguiment_docent.md)
- Evidència mínima a arreplegar: necessitat d'integració justificada, flux híbrid dissenyat amb entrada i eixida clares, i identificació individual del contracte d'`API` que sostindrà `R5`
- Checkpoint docent: validar si cada alumne pot explicar quin problema real del producte tanca amb `R5`, quin flux usarà i per què no és una integració ornamental
- Intervenció per alumnat endarrerit: reduir el repte a un únic recorregut de punta a punta amb un sol desencadenant, una sola crida a l'`API` i una sola eixida observable
- Ampliació per alumnat avançat: anticipar una branca d'incidència, una segona comprovació de qualitat del flux o una justificació més robusta de manteniment sobre la mateixa integració
- Què s'ha de registrar al pilotatge: si el grup entén `R5` com a tancament del producte i no com a ferramenta, quines necessitats reals d'integració apareixen i quin nivell de modelatge docent necessita la definició del flux

### Setmana 18
- Objectiu docent: convertir la decisió d'integració en un flux híbrid o automatització útil ja executable
- Focus o repte: implementació del flux híbrid o automatització útil
- Què explica el professorat: com mantindre la lògica de negoci al backend i usar el workflow només com a orquestració, quins punts crítics s'han de controlar en el camí correcte i en el camí de fallada, i com evitar que la implementació perda traçabilitat
- Què modela en directe: un recorregut mínim amb trigger recognoscible, consum d'`API`, transformació o validació curta, eixida final i un punt de control d'error o diagnòstic
- Què fa l'alumnat: implementa el recorregut principal de la integració, connecta l'`API` pròpia amb el servei extern o workflow, estabilitza el flux nuclear i deixa una primera execució reproduïble del cas principal
- Materials concrets que s'activen: [repte_05_materials_sessio.md](../04_materials/materials_aula/repte_05_materials_sessio.md), [guia_integracio_externa_i_flux_hibrid.md](../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md), [guia_n8n_i_automatitzacio.md](../04_materials/repte_05/guia_n8n_i_automatitzacio.md), [repte_05_integracio_hibrida_n8n.md](../04_materials/apunts_reals/repte_05_integracio_hibrida_n8n.md), [plantilles_feedback_rapid.md](../04_materials/materials_aula/plantilles_feedback_rapid.md) i [checkpoints_curts_aula.md](../04_materials/materials_aula/checkpoints_curts_aula.md)
- Evidència mínima a arreplegar: flux híbrid parcial o complet ja executable, consum real de l'`API` dins del workflow i primera eixida observable del procés
- Checkpoint docent: comprovar que la integració ja fa alguna cosa útil, que reutilitza l'`API` com a contracte central i que cada alumne pot localitzar la seua part del flux dins del producte compartit si n'hi ha
- Intervenció per alumnat endarrerit: congelar passos no nuclears, estabilitzar només el recorregut principal i ajornar qualsevol refinament que no siga imprescindible per executar el flux
- Ampliació per alumnat avançat: afegir millor diagnòstic d'incidències, control d'errors més fi o una eixida addicional justificada dins del mateix flux
- Què s'ha de registrar al pilotatge: si la implementació real de `R5` entra amb la càrrega prevista, quins bloquejos apareixen en consum d'`API`, credencials, workflow o manteniment i quines simplificacions resulten més útils

### Setmana 19
- Objectiu docent: provar el flux complet, tancar documentació operativa i preparar una defensa final individual amb base tècnica real
- Focus o repte: proves i documentació del flux complet, i preparació forta de defensa individual
- Què explica el professorat: per què el repte no queda tancat fins que hi ha prova de punta a punta, documentació usable i capacitat d'explicar tant el cas correcte com la fallada rellevant, i com s'ha de llegir la defensa final des de la rúbrica i el sistema d'evidències
- Què modela en directe: una prova completa del flux híbrid amb cas correcte i cas de fallada, una anotació curta al `README` o documentació tècnica i una defensa breu centrada en autoria, decisions, errors i ús verificable de la IA
- Què fa l'alumnat: executa proves completes, registra incidències, actualitza `README`, AI log i documentació del workflow, i prepara la seua narrativa tècnica individual a partir d'evidències reproduïbles
- Materials concrets que s'activen: [checklist_repte_05.md](../04_materials/repte_05/checklist_repte_05.md), [rubrica_defensa_tecnica.md](../03_avaluacio/rubrica_defensa_tecnica.md), [instruments_seguiment_docent.md](../03_avaluacio/instruments_seguiment_docent.md), [sistema_evidencies.md](../03_avaluacio/sistema_evidencies.md), [repte_05_materials_sessio.md](../04_materials/materials_aula/repte_05_materials_sessio.md) i [repte_05_integracio_hibrida_n8n.md](../04_materials/apunts_reals/repte_05_integracio_hibrida_n8n.md)
- Evidència mínima a arreplegar: prova reproduïble de punta a punta amb cas correcte i fallada rellevant, documentació final del flux, `README` actualitzat i preparació individual de defensa basada en evidències
- Checkpoint docent: validar si cada alumne pot reproduir el flux, explicar què falla quan hi ha incidència, justificar decisions tècniques i defensar l'ús de la IA si n'hi ha hagut
- Intervenció per alumnat endarrerit: renunciar a ampliacions, consolidar un únic flux complet provat, documentar només el nucli imprescindible i preparar una defensa ajustada al mínim funcional no trivial realment assolit
- Ampliació per alumnat avançat: reforçar observabilitat, qualitat de documentació, claredat del troubleshooting o profunditat de la defensa tècnica sense obrir un segon recorregut
- Què s'ha de registrar al pilotatge: si `CP-P5` arriba amb consistència real, quines parts de la defensa continuen sent febles, quins patrons d'ús de IA o manca de traçabilitat reapareixen i si les evidències demanades són assumibles

### Setmana 20
- Objectiu docent: resoldre la defensa final individual i tancar formalment el producte i el pilotatge complet del curs
- Focus o repte: defensa final individual i tancament del producte i del pilotatge
- Què explica el professorat: criteri final de revisió, com es resol la defensa individual encara que hi haja producte compartit, què es considera tancament suficient del curs i com es recull feedback útil per a la iteració següent del paquet docent
- Què modela en directe: lectura final de repositori, `README`, evidències, AI log i flux complet; també una defensa curta amb justificació de decisions, detecció d'errors i capacitat de modificació o contrast
- Què fa l'alumnat: presenta i defensa individualment el seu treball real, entrega evidències finals, deixa el repositori en estat coherent de tancament i aporta feedback sobre càrrega, materials, checkpoints i comprensió dels reptes
- Materials concrets que s'activen: [rubrica_defensa_tecnica.md](../03_avaluacio/rubrica_defensa_tecnica.md), [plantilla_recollida_feedback_pilotatge.md](../03_avaluacio/plantilla_recollida_feedback_pilotatge.md), [registre_incidents_i_ajustos_pilotatge.md](../03_avaluacio/registre_incidents_i_ajustos_pilotatge.md), [instruments_seguiment_docent.md](../03_avaluacio/instruments_seguiment_docent.md), [sistema_evidencies.md](../03_avaluacio/sistema_evidencies.md) i [repte_05_materials_sessio.md](../04_materials/materials_aula/repte_05_materials_sessio.md)
- Evidència mínima a arreplegar: defensa final individual resolta, producte final coherent i reproduïble, feedback recollit i estat final del pilotatge registrat
- Checkpoint docent: tancar `CP-P6`, decidir si el curs queda pilotable de punta a punta dins de les dues avaluacions i deixar distingits ajustos immediats respecte a canvis reservats per a una `v2`
- Intervenció per alumnat endarrerit: centrar la defensa en el flux principal realment assolit, evitar discurs compensatori i deixar tancada una evidència final clara del mínim funcional no trivial
- Ampliació per alumnat avançat: afinar millor la narrativa de trade-offs, manteniment o `v2` del producte, sempre separant clarament el lliurable nuclear del que seria millora futura
- Què s'ha de registrar al pilotatge: balanç global del curs, càrrega real del tram final, qualitat de la defensa individual, patrons de bloqueig, feedback recurrent de l'alumnat i criteri de viabilitat per a ús estable o iteració següent

## Registre mínim de pilotatge per al tram 17-20
Per a les setmanes `17-20`, convé deixar com a mínim:
- una nota setmanal per alumne amb estat real de `R5`, bloqueig principal i decisió docent següent
- una síntesi de si el flux híbrid es convertix realment en tancament del producte o es queda en automatització superficial
- almenys una entrada de feedback al tancament de `R5` i una altra al tancament global del pilotatge
- una entrada al registre d'incidents si apareixen patrons recurrents en integració, proves de punta a punta, defensa individual, autoria o ús verificable de la IA

## Criteri de tancament del curs pilotable
Només convé donar per tancada la seqüència pilotable si:
- existix una integració o flux híbrid lligat a una necessitat real del producte i sostingut sobre l'`API` publicada
- hi ha prova reproduïble del camí correcte i d'almenys una fallada rellevant, amb documentació operativa alineada amb l'estat real
- cada alumne pot explicar, verificar i defensar individualment la seua part del producte, encara que hi haja hagut context de producte compartit o treball coordinat
- el repositori, el `README`, l'AI log i les evidències finals permeten revisar el curs complet com a seqüència tancada dins de les dues primeres avaluacions

## Definition of done del document
Este kit es considera completat quan:
- concreta les setmanes `17-20` com a quint i últim tram operatiu del curs
- indica per a cada setmana objectiu, paper docent, treball de l'alumnat, materials activats, evidència mínima, checkpoint, suport, ampliació i registre de pilotatge
- connecta l'entrada explícita a `R5`, la necessitat real d'integració, la implementació del flux híbrid, les proves, la documentació, la defensa final individual i el tancament del pilotatge
- deixa clar que pot haver-hi context de treball compartit, però que l'evidència, la verificació i la defensa són individuals
- deixa la seqüència pilotable completa del curs tancada com a recorregut docent usable dins de les dues avaluacions
