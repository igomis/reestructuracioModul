# Estat de producció actual

Este document ja no funciona com a llistat d'issues inicials de bootstrap. Ara resumeix l'estat real de producció del repositori i el punt exacte en què es troba la implantació docent del mòdul.

## Situació actual
- la base curricular, el projecte base del curs i els documents centrals de planificació ja existixen i són visibles a `master`
- els materials comuns del mòdul i els paquets nuclears dels Reptes `2`, `3`, `4` i `5` ja estan publicats com a base usable
- els itineraris `Laravel`, `Express/Nest` i `FastAPI` ja existixen com a variacions homologables del mateix producte
- la implantació docent ja està descrita en clau de fases, avaluacions, blocs d'aula i sessions
- el marc temporal de referència queda fixat en unes `20` setmanes aproximades amb `6` hores setmanals, és a dir, unes `120` hores lectives dins de les dues primeres avaluacions
- el model docent assumit és clar: el projecte s'ha de desenvolupar i tancar dins de les dues primeres avaluacions lectives
- la tercera avaluació no es considera període central de desenvolupament, sinó espai residual o de connexió amb empresa o `FCT`
- Git/GitHub es manté com a metodologia de treball i criteri de traçabilitat, no com a bloc d'iniciació bàsica

## Fase actual
- paquet docent en versió `1` funcional
- fase principal del paquet docent tancada a nivell de model, materials, implantació i seguiment
- nova fase oberta: producció d'apunts reals a partir del sistema docent ja consolidat

## Paquets consolidats
- `PB-01` queda consolidat amb l'enunciat base del projecte del curs ja usable i visible.
- `MG-01` queda consolidat com a marc de priorització i seqüència de producció a `docs/04_materials/pla_materials_prioritaris.md`.
- `MG-02` queda consolidat com a base comuna del mòdul amb guies de Git, README/ADR, testing/debugging i ús verificable de la IA.
- `MG-03` queda consolidat com a paquet nuclear del Repte 2 amb materials sobre flux d'usuari, sessions, validació i errors de servidor.
- `MG-04` queda consolidat com a paquet nuclear del Repte 3 amb materials sobre arquitectura per capes o equivalent, persistència i qualitat tècnica.
- `ID-01` queda consolidat com a pla d'implantació docent base del mòdul.
- `ID-02` consolidat amb la calendarització orientativa d'aula.
- `ID-03` consolidat amb la matriu d'evidències i instruments per fase.
- `ID-04` consolidat amb l'adaptació de la planificació a dues avaluacions lectives reals.
- `ID-05` consolidat amb la programació d'aula operativa en dues avaluacions.
- `ID-07` consolidat amb la versió executable del curs en dues avaluacions.
- `ID-08` consolidat amb els instruments finals de seguiment docent.
- `ID-09` consolidat amb el paquet docent exportable del mòdul.
- `ID-10` consolidat amb la revisió editorial i de presentació final del paquet docent.
- `ID-11` consolidat amb el resum executiu i la versió compartible inicial del paquet docent.
- `ID-12` consolidat amb la presentació breu del model DWES per reptes amb IA.
- `ID-13` consolidat amb el tancament formal de la fase principal del paquet docent.
- `AV-01` consolidat amb la revisió de la rúbrica general.
- `PA-01` consolidat amb la programació d'aula per repte.

## Paquets en producció o consolidació final
- `MG-05` continua obert perquè els materials del Repte 4 encara han de passar una ronda final de consolidació pública i revisió de coherència.
- `MG-06` continua obert perquè els materials del Repte 5 encara s'han d'acabar d'alinear amb la seqüència `R3 -> R4 -> R5` i amb el tancament del producte del curs.
- `ID-06` en revisió: ajust temporal a `20` setmanes / `120` hores aproximades a `docs/01_programacio_modul/seqüenciacio_sessions_2_avaluacions.md`.
- `MA-01` en producció: apunts reals del Repte 2 a `docs/04_materials/apunts_reals/repte_02_sessions_i_autenticacio.md`.

## Documents clau de desplegament ja disponibles
- `pla_implantacio_docent.md`: marc global de fases, criteris, evidències i riscos d'implantació
- `calendaritzacio_orientativa_aula.md`: seqüència temporal general del curs per fases
- `calendaritzacio_per_avaluacions.md`: reagrupació del model per avaluacions lectives reals
- `programacio_aula_operativa_2_avaluacions.md`: trasllat del model a blocs d'aula amb activitat docent recognoscible
- `seqüenciacio_sessions_2_avaluacions.md`: detall fi de sessions, checkpoints i seguiment
- `curs_executable_dwes_2_avaluacions.md`: versió unificada i reutilitzable del curs per a desplegament docent real
- `paquet_docent_exportable.md`: lectura unificada del que forma el paquet docent complet i del que es pot transferir a altres contextos
- `resum_executiu_paquet_docent.md`: entrada curta i compartible al model per a professorat que no ha seguit tot el procés
- `presentacio_model_dwes_reptes_ia.md`: peça textual breu per explicar el model a professorat o equips externs
- `revisio_editorial_final.md`: registre de normalització terminològica, coherència editorial i preparació final del paquet
- `tancament_fase_1_paquet_docent.md`: acte formal de tancament de la fase principal i pas a versió `1` funcional
- `programacio_aula_per_repte.md`: lectura docent específica de què convé activar, modelar i revisar en cada repte
- `criteris_ponderacio_reptes_amb_ia.md`: model base de ponderació per avaluar reptes en context de treball amb IA
- `repte_02_sessions_i_autenticacio.md`: primer apunt real de repte, orientat a ús docent i treball autònom

## Itineraris consolidats / en revisió
- `MI-01` `Laravel` queda consolidat com a primer patró reutilitzable de stack.
- `MI-02` `Express/Nest` queda consolidat com a segon patró reutilitzable de stack.
- `MI-03` `FastAPI` queda en revisió transversal junt amb `MI-01` i `MI-02` per assegurar comparabilitat pública.

Criteri comú dels itineraris:
- han de compartir estructura pública, profunditat mínima, tipus de checklist i nivell d'exigència
- han de connectar de manera equivalent amb els Reptes 2, 3, 4 i 5
- han de mantindre el mateix nivell de control sobre auth, persistència, proves, `README` i `AI log`

## Lectura operativa de la fase actual
- el repositori ja no està definint el model del curs; està preparant el seu desplegament real
- el nucli del treball docent ja està documentat i visible: què es fa, quan es fa, amb quins materials i amb quins instruments es revisa
- el nucli del model queda ja tancat i el treball actual entra en producció de materials directament usables en aula

## Següent focus recomanat
- producció dels apunts reals del Repte 3
- continuïtat de la sèrie d'apunts reals dels reptes
- mantenir alineació entre apunts, programació i sistema d'avaluació
