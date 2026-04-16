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
| **Fase 1. Kickoff tècnic** | `3-4` | Repte 1 en `4` sessions de `3h`: base executable i primer punt d'entrada funcional | fitxa del Repte 1, materials comuns, projecte base, model d'itineraris com a marc | entorn funcional, ADR inicial, `README` executable, primer punt d'entrada funcional i primers commits útils | `rubrica_base_reptes.md` | evitar que el kickoff quede en infraestructura buida sense decisió tècnica ni producte recognoscible |
| **Fase 2. Base funcional del producte** | `5-8` | Repte 2: usuaris, sessions, autenticació i validacions | materials del Repte 2, materials comuns, base comuna en `PHP` | registre/login/logout, accés protegit, errors mínims, proves bàsiques, `README` actualitzat | `rubrica_base_reptes.md` | controlar que el flux funcional siga real i no només una demo puntual |
| **Fase 3. Arquitectura i persistència** | `9-12` | Repte 3: capes, persistència i qualitat tècnica | materials del Repte 3, materials comuns, itineraris `Laravel`, `Symfony` i `NestJS` com a suport principal | model de dades, persistència funcional, refactorització per capes o equivalent, regressió mínima | `rubrica_base_reptes.md` | no passar a API sense base persistent i mantenible suficient |
| **Fase 4. Publicació i consum d'API** | `13-16` | Repte 4: contracte API, documentació i consum | materials del Repte 4, materials comuns, itineraris reutilitzats en context d'API | endpoints clau, documentació d'API, col·lecció de proves, consum verificat | `rubrica_base_reptes.md` | assegurar coherència entre contracte, proves, errors i documentació real |
| **Fase 5. Integració híbrida i tancament** | `17-20` | Repte 5: integració externa, automatització i defensa final | materials del Repte 5, materials comuns, reutilització final dels itineraris | flux híbrid complet, prova de punta a punta, documentació final, defensa tècnica | `rubrica_defensa_tecnica.md` | evitar tancaments ornamentals sense valor funcional ni capacitat real de defensa |

## Desenvolupament per blocs temporals

### Fase 0. Arrancada i marc comú

Setmanes orientatives: `1-2`

Focus:

- presentar el projecte base del curs i els dominis admesos
- activar la base comuna de Git, `README/ADR`, testing/debugging i ús verificable de la IA com a repàs metodològic, no com a alfabetització des de zero
- fixar criteris de repositori, evidències i defensa

Resultat esperat del bloc:

- cada equip té repositori, estructura mínima, primer `README` i criteri clar de treball
- el grup entén què comptarà com a evidència durant la resta del curs

### Fase 1. Kickoff tècnic

Setmanes orientatives: `3-4`

Focus:

- resoldre `R1` en `4` sessions de `3` hores
- entendre model client/servidor i concretar la primera decisió tècnica
- preparar l'entorn executable del servei backend
- deixar un primer punt d'entrada funcional i la seua documentació mínima

Resultat esperat del bloc:

- existix una base tècnica executable i defensable
- existix un primer punt d'entrada funcional del backend
- l'equip ja treballa sobre producte, no només sobre marc abstracte

### Fase 2. Base funcional del producte

Setmanes orientatives: `5-8`

Focus:

- activar el flux funcional mínim del producte: usuaris, sessions i control d'accés
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
| **Des de la setmana 1** | materials comuns: Git, `README/ADR`, testing/debugging, ús verificable de la IA |
| **Setmanes 1-4** | projecte base del curs, enunciat base, sistema d'evidències, fitxa del Repte 1 |
| **Setmanes 5-8** | materials del Repte 2 i base comuna en `PHP` |
| **Setmanes 9-12** | materials del Repte 3 i activació principal dels itineraris `Laravel`, `Symfony` i `NestJS` |
| **Setmanes 13-16** | materials del Repte 4, reutilització dels itineraris per contracte API, proves i documentació |
| **Setmanes 17-20** | materials del Repte 5, reutilització final dels itineraris per integració i tancament |

Lectura operativa:

- els materials comuns no desapareixen després de Fase 0; es reusen en totes les fases
- els materials per repte s'activen segons necessitat de producte
- els itineraris entren de manera visible en Fase 3

## Evidències clau per moment

| Moment | Evidències clau |
|---|---|
| **Setmanes 1-2** | repositori creat, estructura mínima, primer `README`, criteri de commits i AI log assumit |
| **Setmanes 3-4** | entorn funcional, domini triat, ADR inicial, `README` executable i primer punt d'entrada funcional |
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
