# Calendarització orientativa d'aula

## Finalitat del document

Baixar el pla d'implantació docent del mòdul a una seqüència temporal executable, de manera que professorat, reptes, materials, evidències i instruments queden ordenats en una progressió d'aula recognoscible.

Esta calendarització no pretén fixar un únic calendari tancat per a tots els contextos. La seua funció és oferir una base reusable perquè el curs es puga desplegar amb ritme coherent, mantenint el treball per reptes, el projecte base com a fil conductor i les evidències autèntiques com a centre de seguiment.

Esta peça s'ha de llegir conjuntament amb `docs/03_avaluacio/matriu_evidencies_i_instruments_per_fase.md`, que concreta quines evidències s'esperen en cada fase i amb quins instruments s'han de revisar.

En contextos on la 3a avaluació queda absorbida per empresa o `FCT`, esta seqüència s'ha d'interpretar com a recorregut lectiu principal concentrat en les dues primeres avaluacions. Això implica que `Fase 4`, `Fase 5` i defensa final no s'han de deixar per a un tercer període residual.

La hipòtesi de treball usada en esta planificació és un curs d'unes `20` setmanes aproximades amb `6` hores setmanals, és a dir, unes `120` hores lectives concentrades principalment en les dues primeres avaluacions.

## Criteris d'ús de la calendarització

- està pensada com a seqüència orientativa d'un bloc lectiu d'unes `20` setmanes amb unes `6` hores setmanals, ampliable o comprimible segons hores reals del centre
- cada fase s'ha d'entendre com a tram de producte i d'evidència, no només com a bloc temàtic
- els materials comuns s'activen des del començament i continuen vigents durant tot el curs
- els materials per repte s'incorporen quan el producte necessita eixa capa tècnica, no abans
- `R2` es resol sobre una base comuna en `PHP`
- els itineraris tecnològics s'introduïxen de manera guiada a partir de `R3`
- el pas d'una fase a la següent ha de dependre d'evidències mínimes verificables, no només del calendari

## Taula global de fases

| Fase | Setmanes orientatives | Repte o focus principal | Materials activats | Evidències principals | Instrument principal | Punt crític de seguiment |
|---|---|---|---|---|---|---|
| **Fase 0. Arrancada i marc comú** | `1-2` | marc de treball, projecte base i criteris comuns | materials comuns de mòdul, sistema d'evidències, enunciat base del projecte | repositori creat, primer `README`, organització mínima, traça inicial | `checklist_revisio_repo.md` | comprovar que el grup usa Git/GitHub com a repàs metodològic i traçabilitat professional, no com a iniciació bàsica |
| **Fase 1. Kickoff tècnic** | `3-4` | Repte 1 en `3` sessions de `3h`: marc comú, decisió tècnica inicial, base executable i landing inicial servida pel backend | fitxa del Repte 1, materials comuns, projecte base, model d'itineraris com a marc | entorn funcional, nota tècnica de decisió inicial, `README` executable, landing inicial i primers commits útils | `rubrica_base_reptes.md` | evitar que el kickoff quede en infraestructura buida sense decisió tècnica ni producte recognoscible |
| **Fase 2. Base funcional del producte** | `5-8` | Repte 2: dades, processament, lògica, estat, autenticació i funcionalitat protegida sobre base comuna en `PHP` | materials del Repte 2, materials comuns, base comuna en `PHP` | flux complet de `R2`, reutilització funcional de dades, accés protegit, errors controlats, proves bàsiques, `README` actualitzat | `rubrica_base_reptes.md` | controlar que el flux funcional siga real i no només una demo puntual |
| **Fase 3. Arquitectura i persistència** | `9-12` | Repte 3: capes, persistència i qualitat tècnica | materials del Repte 3, materials comuns, itineraris `Laravel`, `Symfony` i `NestJS` com a suport principal | model de dades, persistència funcional, refactorització per capes o equivalent, regressió mínima | `rubrica_base_reptes.md` | no passar a API sense base persistent i mantenible suficient |
| **Fase 4. Publicació i consum d'API** | `13-16` | Repte 4: contracte API, documentació i consum | materials del Repte 4, materials comuns, itineraris reutilitzats en context d'API | endpoints clau, documentació d'API, col·lecció de proves, consum verificat | `rubrica_base_reptes.md` | assegurar coherència entre contracte, proves, errors i documentació real |
| **Fase 5. Integració híbrida i tancament** | `17-20` | Repte 5: integració externa, automatització i defensa final | materials del Repte 5, materials comuns, reutilització final dels itineraris | flux híbrid complet, prova de punta a punta, documentació final, defensa tècnica | `rubrica_defensa_tecnica.md` | evitar tancaments ornamentals sense valor funcional ni capacitat real de defensa |

## Desenvolupament per blocs temporals

### Fase 0. Arrancada i marc comú

Setmanes orientatives: `1-2`

Focus:

- presentar el projecte base del curs i els dominis admesos
- activar la base comuna de Git, `README i nota tècnica de decisió`, testing/debugging i ús verificable de la IA com a repàs metodològic, no com a alfabetització des de zero
- fixar criteris de repositori, evidències i defensa

Resultat esperat del bloc:

- cada equip té repositori, estructura mínima, primer `README` i criteri clar de treball
- el grup entén què comptarà com a evidència durant la resta del curs

### Fase 1. Kickoff tècnic

Setmanes orientatives: `3-4`

Focus:

- resoldre `R1` en `3` sessions de `3` hores
- entendre model client/servidor i concretar la primera decisió tècnica
- preparar l'entorn executable del servei backend
- deixar una landing inicial servida pel backend i la seua documentació mínima

Resultat esperat del bloc:

- existix una base tècnica executable i defensable
- existix una landing inicial servida pel backend
- l'equip ja treballa sobre producte, no només sobre marc abstracte

### Fase 2. Base funcional del producte

Setmanes orientatives: `5-8`

Focus:

- activar el flux funcional mínim del producte: dades, lògica, estat i control d'accés sobre una acció real del domini
- introduir validacions, errors mínims i proves bàsiques
- consolidar la base comuna en `PHP` sense obrir encara el contrast de frameworks

Resultat esperat del bloc:

- el producte ja té una primera funcionalitat real usable i verificable
- el grup deixa evidències de procés, no només resultat

### Fase 3. Arquitectura i persistència

Setmanes orientatives: `9-12`

Focus:

- refactoritzar el backend a capes o equivalent
- consolidar model de dades, persistència i validacions lligades al domini
- activar `Laravel`, `Symfony` i `NestJS` com a patró directe de stack per a `R3`

Resultat esperat del bloc:

- el producte deixa de ser només funcional i passa a ser mantenible
- l'equip ja pot explicar l'arquitectura i el model de dades com a base del Repte 4

### Fase 4. Publicació i consum d'API

Setmanes orientatives: `13-16`

Focus:

- exposar funcionalitats com a API amb contracte clar
- documentar endpoints, errors i proves de consum
- reutilitzar itineraris per aplicar auth, estructura i validació en context d'API

Resultat esperat del bloc:

- existix una API publicada, documentada i comprovada
- el producte queda preparat per integrar-se amb fluxos externs

### Fase 5. Integració híbrida i tancament

Setmanes orientatives: `17-20`

Focus:

- connectar el producte amb una automatització, servei extern o flux híbrid
- tancar documentació, proves i defensa tècnica
- revisar mantenibilitat i traçabilitat del conjunt

Resultat esperat del bloc:

- el backend del curs queda tancat com a producte defensable i integrable
- el grup arriba a defensa final amb evidències suficients de procés i de resultat

## Activació de materials per moment

| Moment | Materials activats |
|---|---|
| **Des de la setmana 1** | materials comuns: Git, `README i nota tècnica de decisió`, testing/debugging, ús verificable de la IA |
| **Setmanes 1-4** | projecte base del curs, enunciat base, sistema d'evidències, fitxa del Repte 1 |
| **Setmanes 5-8** | materials del Repte 2 i base comuna en `PHP` |
| **Setmanes 9-12** | materials del Repte 3 i activació principal dels itineraris `Laravel`, `Symfony` i `NestJS` |
| **Setmanes 13-16** | materials del Repte 4, reutilització dels itineraris per contracte API, proves i documentació |
| **Setmanes 17-20** | materials del Repte 5, reutilització final dels itineraris per integració i tancament |

Lectura operativa:

- els materials comuns no desapareixen després de Fase 0; es reusen en totes les fases
- els materials per repte s'activen segons necessitat de producte
- els itineraris entren de manera visible en Fase 3

## Encaix temporal de tallers, teoria i presentacions

La planificació detallada està en [Planificació de microtallers dins dels reptes](planificacio_microtallers_reptes.md). Esta taula només situa cada taller dins del calendari general perquè no aparega com una càrrega afegida fora de la sessió.

| Fase | Sessió preferent | Taller | Temps dins de la sessió | Teoria/material que s'activa | Presentació |
|---|---|---|---:|---|---|
| Fase 0 | `R1S0` | `MT19. IA responsable aplicada al repte` | `25 min` inicials + recordatoris de `10 min` | [Guia d'ús verificable de la IA](../04_materials/materials_comuns/guia_ús_verificable_ia.md) | [MT19](../07_presentacions/microtallers/mt19_ia_responsable_repte.md) |
| Fase 1 | `R1S1` | `MT01. Projecte no CRUD` | `35 min` | [Apunts R1](../04_materials/apunts_reals/repte_01_kickoff_backend.md) | [MT01](../07_presentacions/microtallers/mt01_projecte_no_crud.md) |
| Fase 1 | `R1S2` | `MT02. README executable i commit defensable` | `30 min` | [Guia README i nota tècnica de decisió](../04_materials/materials_comuns/guia_readme_i_adr.md) | [MT02](../07_presentacions/microtallers/mt02_readme_commit_defensable.md) |
| Fase 2 | `R2S1-R2S2` | `MT03. Validació de servidor amb casos roïns` | `45 min` + `10 min` | [Guia de validació i errors](../04_materials/repte_02/guia_validacio_i_errors_servidor.md) | [MT03](../07_presentacions/microtallers/mt03_validacio_servidor_casos_roins.md) |
| Fase 2 | `R2S4` | `MT04. Sessió, cookies i estat` | `35 min` | [Guia de flux d'usuari i sessions](../04_materials/repte_02/guia_flux_usuari_i_sessions.md) | [MT04](../07_presentacions/microtallers/mt04_sessions_cookies_estat.md) |
| Fase 2 | `R2S5-R2S6` | `MT05. Auth mínima defensable` | `50 min` + `10 min` | [Apunts R2](../04_materials/apunts_reals/repte_02_sessions_i_autenticacio.md) | [MT05](../07_presentacions/microtallers/mt05_auth_minima_defensable.md) |
| Fase 2 | `R2S7` | `MT06. Debugging i prova curta` | `35 min` | [Guia testing i debugging](../04_materials/materials_comuns/guia_testing_i_debugging.md) | [MT06](../07_presentacions/microtallers/mt06_debugging_prova_curta.md) |
| Fase 3 | `R3S1` | `MT07. Migrar un cas d'ús a framework` | `40 min` | [Apunts R3](../04_materials/apunts_reals/repte_03_mvc_i_persistencia.md) | [MT07](../07_presentacions/microtallers/mt07_migrar_cas_us_framework.md) |
| Fase 3 | `R3S2` | `MT08. Migracions, seeders i dades de prova` | `50 min` | [Guia de persistència i modelat](../04_materials/repte_03/guia_persistencia_i_modelat_dades.md) | [MT08](../07_presentacions/microtallers/mt08_migracions_seeders_dades_prova.md) |
| Fase 3 | `R3S2B` | `MT16. Portabilitat entre frameworks` | `3h` obligatòries | [Model d'itineraris tecnològics](model_itineraris_tecnologics.md) | [MT16](../07_presentacions/microtallers/mt16_portabilitat_frameworks.md) |
| Fase 3 | `R3S3-R3S4` | `MT09. On pose la lògica` | `35 min` + `10 min` | [Guia de refactorització MVC o equivalent](../04_materials/repte_03/guia_refactoritzacio_mvc_o_equivalent.md) | [MT09](../07_presentacions/microtallers/mt09_on_pose_la_logica.md) |
| Fase 4 | `R4S1` | `MT10. Dissenyar endpoint abans de programar` | `35 min` | [Guia de contracte i disseny API](../04_materials/repte_04/guia_contracte_i_disseny_api.md) | [MT10](../07_presentacions/microtallers/mt10_dissenyar_endpoint_abans_programar.md) |
| Fase 4 | `R4S5` | `MT11. Provar i documentar una API` | `45 min` | [Guia de proves i documentació API](../04_materials/repte_04/guia_proves_i_documentacio_api.md) | [MT11](../07_presentacions/microtallers/mt11_provar_documentar_api.md) |
| Fase 4 | `R4S3` o `R4S6` | `MT17. Tokens funcionals del backend` | `60 min` opcional o sessió ampliada opcional | [Guia de contracte i disseny API](../04_materials/repte_04/guia_contracte_i_disseny_api.md) | [MT17](../07_presentacions/microtallers/mt17_tokens_funcionals_backend.md) |
| Fase 5 | `R5S1` | `MT12. Triar una integració amb valor` | `30 min` | [Guia d'integració externa i flux híbrid](../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md) | [MT12](../07_presentacions/microtallers/mt12_integracio_amb_valor.md) |
| Fase 5 | `R5S2` | `MT13. Secrets, .env i claus` | `35 min` | [Guia d'integració externa i flux híbrid](../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md) | [MT13](../07_presentacions/microtallers/mt13_secrets_env_claus.md) |
| Fase 5 | `R5S3` | `MT14. Mapping de resposta externa` | `45 min` | [Guia d'integració externa i flux híbrid](../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md) | [MT14](../07_presentacions/microtallers/mt14_mapping_resposta_externa.md) |
| Fase 5 | `R5S5` | `MT15. Defensa tècnica curta` | `35 min` | [Guió de defensa individual](../08_materials_compartibles/guio_defensa_individual_breu.md) | [MT15](../07_presentacions/microtallers/mt15_defensa_tecnica_curta.md) |
| Fase 5 | `R5S4` o `R5S6` | `MT18. Actius digitals tokenitzats` | `50 min` opcional o sessió ampliada opcional | [Guia d'orquestració i automatització](../04_materials/repte_05/guia_orquestracio_i_automatitzacio.md) | [MT18](../07_presentacions/microtallers/mt18_actius_digitals_tokenitzats.md) |

## Evidències clau per moment

| Moment | Evidències clau |
|---|---|
| **Setmanes 1-2** | repositori creat, estructura mínima, primer `README`, criteri de commits i AI log assumit |
| **Setmanes 3-4** | entorn funcional, domini triat, nota tècnica de decisió inicial, `README` executable i landing inicial servida pel backend |
| **Setmanes 5-8** | autenticació funcional, estat o sessió equivalent, validacions mínimes, primers casos de prova |
| **Setmanes 9-12** | arquitectura per capes o equivalent, persistència coherent, model de dades, proves de regressió |
| **Setmanes 13-16** | contracte API, documentació d'endpoints, col·lecció de proves, consum verificat |
| **Setmanes 17-20** | flux híbrid complet, prova de punta a punta, documentació final, defensa tècnica i AI log tancat si aplica |

## Punts crítics de seguiment docent

- revisar a les setmanes `2-3` si el grup realment ha assumit Git, evidències i ús verificable de la IA
- revisar a les setmanes `7-8` si el Repte 2 deixa una base funcional real i no només una demostració puntual
- revisar a les setmanes `10-12` si la persistència i l'arquitectura estan prou madures per obrir API
- revisar a les setmanes `15-16` si la documentació i les proves d'API reflectixen l'estat real del codi
- revisar a les setmanes `19-20` si la integració final té valor funcional real i si la defensa és coherent amb el repositori

## Marges d'adaptació

- si el centre treballa amb menys hores setmanals, la calendarització es pot estendre a `22-24` setmanes mantenint la mateixa lògica de fases
- si el centre treballa amb més intensitat horària, Fase 0 i Fase 1 poden compactar-se, però no s'haurien de fusionar si això elimina control sobre repositori i criteris comuns
- si un grup mostra bloqueig tècnic en Fase 2, convé reforçar materials comuns i itinerari abans de passar a persistència
- si la base de Fase 3 és feble, s'hauria de retardar Fase 4 abans que publicar una API sense model ni arquitectura sostenibles
- els itineraris no s'han d'usar com a excusa per descompassar criteris d'avaluació o de seguiment

## Definition of done del document

Este document es considera completat quan:

- definix una calendarització orientativa reusable i no només un recordatori de fases
- organitza el curs en les fases 0-5 acordades
- indica per a cada fase setmanes orientatives, focus principal, materials, evidències, instrument i punt crític de seguiment
- deixa visible quan s'activen materials comuns, materials per repte i itineraris
- manté coherència amb treball per reptes, projecte base, itineraris, evidències autèntiques i IA verificable
