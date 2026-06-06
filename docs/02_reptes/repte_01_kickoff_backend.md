# Repte 1. Kickoff funcional d’un servei web backend amb microprojectes i criteris d’avaluació explícits

## Fitxa canònica del repte

- **Funció didàctica principal**: iniciació / arranque.
- **Objectiu**: deixar arrencat el projecte base amb entorn executable, traçabilitat, punt d'entrada funcional i decisió tècnica inicial.
- **Producte esperat**: backend inicial funcional, executable en local, amb Docker, README, documentació en repositori i primera peça real del producte.
- **Evidències**: repositori traçable, README executable, documentació del repte enllaçada, issue mare, commit rellevant comentat, execució real, ADR o justificació tècnica breu i mini defensa de kickoff.
- **Paper de la IA**: ús assistit per IA permés per configuració, comparativa i depuració inicial; els límits i la delegació excessiva depenen de [us-ia-professorat-i-alumnat.md](../us-ia-professorat-i-alumnat.md).
- **Relació amb el projecte base**: este repte obri el projecte base i fixa la seua base metodològica, tècnica i documental.
- **Checkpoint de control**: arrencada reproduïble amb lectura del `README`, justificació del stack triat i microcanvi tècnic simple sobre l'entorn.
- **Instrument dominant**: checklist d'arrencada i repositori executable.
- **Instrument de comprensió**: mini defensa tècnica de kickoff.
- **Instrument de control de delegació excessiva**: revisió de commit rellevant comentat, contrast amb `AI log` i prova en directe.
- **Instrument de recuperació o millora**: nova demostració d'arrencada amb ajust de `README`, Docker i justificació tècnica.

## Justificació docent

- **Evidència principal**: repositori executable amb `README`, punt d'entrada funcional i justificació tècnica breu.
- **Evidències secundàries**: fitxa d'exploració, issue mare, commit rellevant comentat, incidència o dubte registrat i mini defensa.
- **Mínim suficient**: el projecte arranca des del `README`, mostra un backend mínim real i l'alumnat explica client/servidor, serveis i decisió tècnica.
- **Feedback previst**: checkpoint de kickoff amb prova d'arrencada, revisió ràpida del repositori i pregunta de transferència.

## 1. Visió general del repte

**Finalitat del repte**

Iniciar un servei web backend en condicions professionals bàsiques i deixar una base tècnica robusta per al conjunt del curs.

Este repte fixa la manera de treballar de l’equip des del primer moment: entorn reproductible, traçabilitat, documentació mínima, decisió tecnològica guiada i una primera peça funcional simple però real.

No es considera suficient triar tecnologia o generar un esquelet buit. Tampoc es demana encara una funcionalitat de domini més rica. El sentit del repte és arrancar bé, entendre l’entorn servidor i deixar una base executable i defensable.

**Producte principal del repte**

Una primera versió funcional i verificable del servei backend, amb:

- repositori inicial funcional
- base comuna en `PHP` assumida dins d’un marc docent acotat
- projecte executable en local de manera reproductible
- ús de Docker
- servidor web, servei de base de dades i phpMyAdmin incorporats en l'entorn inicial
- punt d’entrada funcional simple
- README tècnic executable
- documentació del repte dins del repositori i enllaçada des d'un índex o pàgina visible
- justificació tècnica breu
- registre d'una decisió tècnica menuda i d'una incidència, dubte o bloqueig real
- traçabilitat de treball amb issues i commits

**Context professional simul·lat o realista**

Un equip backend rep l’encàrrec de posar en marxa un nou servei. No es demana encara el producte complet, però sí una base fiable que permeta entendre com arranca el sistema, com s’executa l’entorn servidor i com es pot continuar el projecte sense improvisació tècnica.

**Relació amb el projecte global del curs**

Este repte crea la base tècnica, metodològica i documental sobre la qual es construiran els reptes següents.

No es considera superat només per tindre un esquelet de framework. Ha d’existir una primera peça funcional real del producte, però esta peça mínima no implica necessàriament formulari, validació o persistència.

---

## 2. Relació amb resultats d’aprenentatge

**Resultat d’aprenentatge principal**

- **RA1**: selecciona les arquitectures i tecnologies de programació web en entorn servidor, analitzant les seues capacitats i característiques pròpies

**Resultat d’aprenentatge secundari o transversal**

- **RA5 (no qualificable principalment en este repte, si es manté la matriu actual del mòdul)**: contribució inicial a l’organització del projecte amb criteris de mantenibilitat, estructura i creixement

**Justificació curricular**

El repte permet treballar de forma aplicada la comparativa guiada d’arquitectures i tecnologies de servidor, els mecanismes d’execució del codi, la relació entre servidor d’aplicacions i servidor web, i la integració bàsica amb llenguatges de marques o respostes equivalents.

La primera organització del projecte prepara el treball posterior de mantenibilitat, però no substituïx el treball específic de separació de responsabilitats i arquitectura del Repte 3.

---

## 3. Canvi metodològic que introduïx la IA

**Paper de la IA en este repte**

La IA es pot usar per a:

- explorar opcions tecnològiques dins del marc docent establit
- resumir documentació tècnica inicial
- suggerir esquelets de projecte
- ajudar a preparar Docker i scripts d’arrancada
- revisar la claredat del README
- detectar errors de configuració inicial

**Què no es delega**

L’alumnat ha de:

- entendre el paper de l’entorn servidor
- justificar la tecnologia triada dins de les opcions guiades
- verificar que el projecte arranca realment
- entendre què fa Docker i què posa en marxa
- explicar l’estructura creada
- demostrar que existix un punt d’entrada funcional del producte

**Risc principal d’ús inadequat de la IA**

Acceptar configuracions, comparatives o documentació sense entendre-les ni verificar-les, o confondre un esquelet generat amb un projecte realment executable i defensable.

**Mesures de control**

- AI log quan hi haja ús d’IA
- issues i commits amb traçabilitat
- prova en directe del README
- execució real amb `docker compose up` o equivalent
- defensa tècnica breu
- microcanvis en viu
- preguntes de transferència sobre alternatives descartades

---

## 4. Estructura del repte

### 4.1 Nucli del repte

**Objectiu del nucli**

Deixar operativa una primera versió funcional del servei backend que siga executable, justificable i reutilitzable per als reptes següents.

**Lliurable principal**

Backend inicial funcional amb:

- punt d’entrada simple al producte
- entorn executable amb Docker
- estructura base coherent
- README clar d’arrancada
- justificació tècnica breu
- historial de treball traçable

**Criteris d’avaluació principals del nucli**

- RA1b
- RA1c
- RA1d
- RA1e
- RA1f
- RA1g

**Evidències obligatòries del nucli**

- repositori funcional
- README executable
- Docker Compose o equivalent funcional
- issue mare de kickoff
- commits significatius
- un commit rellevant comentat o referenciat pel mateix alumne
- demo d’arrancada i execució
- evidència d’un punt d’entrada funcional
- ADR o justificació tècnica breu
- mini defensa tècnica al checkpoint de tancament
- AI log quan corresponga

---

## 5. Microreptes, microprojectes i microtasques del repte

> **Norma del repte**
>
> - Els microprojectes cobrixen sobretot criteris procedimentals.
> - Les microtasques d’investigació cobrixen sobretot criteris conceptuals i de decisió.
> - Cap microprojecte apareix sense el camp **CA coberts**.
> - Cada microprojecte ha de generar almenys una evidència verificable.
> - El mínim funcional del repte no obliga a incloure formulari, validació ni persistència.
> - Estos elements poden aparéixer com a ampliació opcional o com a pas natural del Repte 2.
> - Els microreptes són unitats de progrés, no unitats fixes de temps docent.
> - En la concreció docent d’aula, els `4` microreptes es compacten en `2` sessions principals de treball i una tercera sessió opcional de checkpoint o defensa formal.

### Microrepte R1M1 — Model client/servidor i elecció guiada de stack

**Tipus**

Microtasca d’investigació i decisió tècnica.

**Objectiu**

Entendre el model client/servidor del producte, caracteritzar els models d'execució de codi en client i servidor, i fixar una base tècnica guiada que siga coherent amb el recorregut del curs.

**Tasca**

L’equip completa una [fitxa breu d’exploració tècnica inicial](../08_materials_compartibles/fitxa_exploracio_tecnica_inicial.md) i la convertix en una primera decisió tècnica orientativa dins del marc docent del curs.

Esta exploració es pot fer amb ajuda d’IA i amb consulta de materials del curs.

No busca una comparativa exhaustiva ni un informe llarg. Busca sobretot comprensió inicial, criteri tècnic i capacitat d’explicar amb què començaríem i quins dubtes continuen oberts.

No cal adjuntar captures de totes les converses amb IA.

La fitxa ha d’incloure:

- paper del client i del servidor dins del producte
- diferència entre què s'executa al client web i què s'executa al servidor
- explicació del model d'execució aplicat al producte propi
- identificació de tecnologies de client i de servidor
- exploració breu de possibles stacks o frameworks
- diferències inicials entre exemples com `Laravel`, `Symfony` i `NestJS`
- primera decisió tècnica orientativa
- justificació del paper que tindrà el backend dins d'eixe model
- dubtes tècnics detectats

**Relació amb el producte principal**

Sense una decisió inicial coherent, el kickoff funcional queda en un esquelet poc defensable i difícil de sostindre durant el curs.

**CA coberts**

- **RA1a**: s’han caracteritzat i diferenciat els models d’execució de codi en el servidor i en el client web
- **RA1b**: s’han reconegut els avantatges que proporciona la generació dinàmica de pàgines
- **RA1c**: s’han identificat els mecanismes d’execució de codi en els servidors web
- **RA1g**: s’han reconegut i avaluat les eines i frameworks de programació en entorn servidor

**Descripció dels CA en llenguatge docent**

- L’alumnat diferencia què s’executa al navegador i què s’executa al servidor.
- L’alumnat relaciona eixa diferència amb el seu producte concret.
- L’alumnat sap explicar per què un backend dinàmic aporta valor al projecte.
- L’alumnat distingix on i com s’executa el codi del servidor.
- L’alumnat compara opcions de manera guiada i evita eleccions arbitràries.

**Paper de la IA**

La IA pot ajudar a localitzar exemples de stack, frameworks, tecnologies de client i servidor o diferències inicials entre `Laravel`, `Symfony` i `NestJS`, però el resultat final ha de reflectir què s’ha entés, què s’ha contrastat i quina orientació provisional es pren dins del marc docent del curs.

**Evidències obligatòries**

- fitxa breu d’exploració tècnica inicial
- explicació breu del model d'execució client vs servidor aplicat al producte
- primera decisió tècnica orientativa
- referència breu a alternatives i dubtes oberts
- posada en comú o defensa oral breu

**Instrument d’avaluació**

Rúbrica d’investigació aplicada.

**Indicadors d’assoliment**

- fitxa breu amb criteri, no superficial
- marc tecnològic acotat i realista
- orientació coherent amb el curs
- justificació oral convincent

**Riscos habituals**

- fitxa convertida en comparativa massa llarga o genèrica
- voler substituir la fitxa per captures de converses amb IA
- elecció per preferència personal sense criteri docent
- dispersió tecnològica difícil de sostindre

**Verificació del treball real**

- revisió de la fitxa breu entregada per la parella o alumne
- posada en comú oral breu al final de la sessió o a l’inici de la següent
- pregunta oral: “quina part del teu producte s'executa al client i quina al servidor?”
- pregunta oral: “per què esta opció és assumible per al curs i quina has descartat?”
- pregunta oral: “què fa el runtime o servidor triat dins del flux d’execució?”

**Pes orientatiu dins del repte**

20%

### Microrepte R1M2 — Base executable en PHP amb Docker i completació de l’entorn

**Tipus**

Microprojecte procedimental.

**Objectiu**

A partir d’un model mínim mostrat pel professorat, configurar una base executable pròpia per al projecte i completar-la afegint persistència i gestió bàsica de l’entorn.

**Tasca**

El professorat modela una base mínima executable amb `PHP`, servidor web i `Docker`, suficient per veure l'arrencada i entendre el paper de cada peça, però no dona l'entorn complet tancat.

A partir d'eixe model, l'equip:

- crea el repositori
- adapta l'entorn mínim al seu projecte
- ajusta elements propis com nom del projecte, estructura mínima, port o resposta inicial
- prepara arrencada amb `docker compose up` o equivalent
- deixa visible el paper de `PHP` i del servidor web
- completa l'entorn afegint servei de base de dades i phpMyAdmin
- definix estructura bàsica de carpetes
- establix convencions inicials
- prepara un README curt de posada en marxa i comprovació
- crea issue mare i primeres microtasques
- valida que una altra persona pot arrancar el projecte seguint la documentació
- registra una incidència, dubte o decisió tècnica real detectada durant la configuració

**Relació amb el producte principal**

Este microprojecte assegura que el servei no és només una idea, una demo local improvisada o una còpia plana d'una configuració docent, sinó una base executable, adaptada, documentada i reutilitzable.

**CA coberts**

- **RA1c**: s’han identificat els mecanismes d’execució de codi en els servidors web
- **RA1d**: s’han reconegut les funcionalitats que aporten els servidors d’aplicacions i la seua integració amb els servidors web
- **RA1e**: s’han identificat i caracteritzat els principals llenguatges i tecnologies relacionats amb la programació web en entorn servidor
- **RA1f**: s’han verificat els mecanismes d’integració dels llenguatges de marques amb els llenguatges de programació en entorn servidor

**Descripció dels CA en llenguatge docent**

- L’alumnat comprén quin component executa què i amb quin paper.
- L’alumnat identifica com s’integra servidor, aplicació, contenidors, base de dades, phpMyAdmin i punt d’entrada.
- L’alumnat prepara una base tècnica funcional, no un conjunt d’arxius inconnexos.
- L’alumnat verifica que el projecte es pot executar de manera reproductible.
- L'alumnat pot explicar què ha adaptat respecte del model del professorat i per què.

**Paper de la IA**

La IA pot suggerir fitxers inicials, estructura base, configuracions de Docker o pistes per depurar errors, però l’alumnat ha de comprovar que tot allò realment arranca, adaptar-ho al seu projecte i poder explicar el paper de cada servei. No és acceptable entregar una configuració completa generada o copiada sense verificació i defensa.

**Evidències obligatòries**

- repositori creat
- arrencada amb Docker funcional
- `docker-compose.yml` o equivalent adaptat al projecte
- serveis mínims de `PHP`, servidor web, base de dades i phpMyAdmin definits i arrancables
- issue mare de kickoff
- primers commits significatius
- README curt i executable
- estructura base del projecte
- registre de primera validació d’arrancada
- justificació curta d'una decisió tècnica
- incidència, dubte o bloqueig detectat o resolt

**Instrument d’avaluació**

Checklist tècnica de repositori + revisió docent de README.

**Indicadors d’assoliment**

- el projecte arranca sense passos ocults
- `docker compose up` o equivalent és funcional
- el README és suficient per a tercers
- l’estructura és coherent
- hi ha traçabilitat mínima del procés
- es pot explicar què fa cada servei
- hi ha una adaptació pròpia respecte del model inicial

**Riscos habituals**

- README incomplet
- Docker present però no usable
- configuració copiada sense entendre
- arrencada només possible en l’ordinador de l’autor
- phpMyAdmin o la base de dades afegits com a decoració sense saber comprovar-los

**Verificació del treball real**

- prova en directe d’arrancada seguint únicament el README
- execució real amb Docker
- revisió de commits i issues
- pregunta tècnica sobre la funció del servidor, `PHP`, Docker, base de dades i phpMyAdmin
- explicació de què s'ha adaptat respecte del model del professorat
- revisió d'una decisió tècnica menuda i d'una incidència o dubte real

**Pes orientatiu dins del repte**

35%

### Microrepte R1M3 — Primer punt d’entrada funcional del backend

**Tipus**

Microprojecte procedimental.

**Objectiu**

Construir una primera peça funcional simple del producte perquè el repte no quede reduït a infraestructura o muntatge de framework.

**Tasca**

L’equip implementa almenys una d’estes opcions, o una alternativa equivalent coherent amb la base comuna del curs:

- una landing page
- una ruta inicial
- una vista renderitzada
- un endpoint bàsic
- un healthcheck

La implementació ha de permetre demostrar que el backend ja respon de manera real i verificable.

**Relació amb el producte principal**

És la primera peça funcional real del producte i la demostració que la base creada ja servix per a començar a construir valor.

**CA coberts**

- **RA1b**: s’han reconegut els avantatges que proporciona la generació dinàmica de pàgines
- **RA1e**: s’han identificat i caracteritzat els principals llenguatges i tecnologies relacionats amb la programació web en entorn servidor
- **RA1f**: s’han verificat els mecanismes d’integració dels llenguatges de marques amb els llenguatges de programació en entorn servidor

**Descripció dels CA en llenguatge docent**

- L’alumnat és capaç de mostrar per què el backend no és un simple conjunt d’arxius sense execució real.
- L’alumnat integra punt d’entrada, execució i resposta del servidor.
- L’alumnat demostra una primera unió funcional entre entorn desplegat i comportament observable.

**Paper de la IA**

La IA pot ajudar a proposar esquelets de ruta, vista o endpoint, però l’alumnat ha de provar-los, adaptar-los i explicar-los.

**Evidències obligatòries**

- landing, ruta, vista, endpoint o healthcheck funcional
- demo del comportament
- registre de prova funcional mínima
- captura o log d’execució
- commits associats

**Instrument d’avaluació**

Rúbrica de microprojecte funcional.

**Indicadors d’assoliment**

- hi ha una resposta real del sistema
- la implementació és simple però funcional
- el punt d’entrada és comprensible i defensable
- el repte no queda reduït a esquelet buit

**Riscos habituals**

- resposta purament decorativa sense connexió amb el servei
- demo aparent però no reproduïble
- confondre “mínim funcional” amb “res de producte”

**Verificació del treball real**

- prova en directe del punt d’entrada funcional
- canvi menor en viu sobre ruta, missatge o resposta
- pregunta tècnica sobre què passa en servidor quan s’accedix a este punt d’entrada

**Pes orientatiu dins del repte**

25%

### Microrepte R1M4 — Documentació tècnica, verificació i checkpoint

**Tipus**

Microprojecte de tancament i verificació.

**Objectiu**

Consolidar el repte amb evidència tècnica verificable i demostrar que el treball realitzat és comprés i reutilitzable.

**Tasca**

L’equip:

- revisa README
- completa la justificació tècnica o ADR curt
- registra incidències inicials i com les ha resoltes
- documenta l’arrancada i la validació mínima fetes
- crea un directori de documentació dins del repositori
- penja les fitxes o documents del repte al repositori
- crea una pàgina o índex visible que enllace eixa documentació
- prepara una defensa tècnica breu

**Relació amb el producte principal**

Sense documentació i defensa, el repte pot arrancar, però no queda prou verificat ni transferible a l’equip o als reptes següents.

**CA coberts**

- **RA1d**: s’han reconegut les funcionalitats que aporten els servidors d’aplicacions i la seua integració amb els servidors web
- **RA1g**: s’han reconegut i avaluat les eines i frameworks de programació en entorn servidor

**Descripció dels CA en llenguatge docent**

- L’alumnat sap explicar el paper de les peces tècniques triades.
- L’alumnat justifica l’eina o framework usat a partir de la seua experiència en el kickoff, no només d’una lectura teòrica.
- L’alumnat demostra que la documentació correspon al sistema real.

**Paper de la IA**

La IA pot ajudar a polir el text del README o de la justificació tècnica, però la defensa i la verificació són responsabilitat directa de l’alumnat.

**Evidències obligatòries**

- README final
- justificació tècnica final o ADR curt
- registre d’incidències inicials i correccions
- evidència de validació tècnica mínima
- directori de documentació en el repositori
- fitxes o documents del repte incorporats al repositori
- pàgina o índex visible que enllaça la documentació del repte
- defensa oral
- AI log si n’hi ha hagut ús

**Instrument d’avaluació**

Rúbrica de defensa tècnica + checklist de documentació.

**Indicadors d’assoliment**

- documentació coherent amb el producte real
- defensa clara i solvent
- capacitat de justificar decisions
- capacitat de connectar el repte amb el següent

**Riscos habituals**

- README embellit però no executable
- documentació redactada a posteriori sense relació real amb el procés
- defensa memorística

**Verificació del treball real**

- execució del README
- contrast entre justificació, commits i resultat final
- preguntes de transferència sobre com escala esta base al Repte 2

**Pes orientatiu dins del repte**

20%

---

## 6. Taula resum de microreptes i criteris d’avaluació

| Microrepte | Tipus | Producte o lliurable | CA coberts | Evidències principals | Instrument | Pes orientatiu |
|---|---|---|---|---|---|---|
| R1M1 | Investigació / decisió tècnica | Fitxa breu d’exploració tècnica + model d'execució client/servidor + decisió orientativa | RA1a, RA1b, RA1c, RA1g | Fitxa, model d'execució, dubtes detectats, posada en comú | Rúbrica | 20% |
| R1M2 | Procedimental | Repositori executable amb Docker i estructura base | RA1c, RA1d, RA1e, RA1f | Repo, Docker, README, issues, commits, prova d’arrancada | Checklist + revisió | 35% |
| R1M3 | Procedimental | Punt d’entrada funcional simple | RA1b, RA1e, RA1f | Demo funcional, logs o captures, evidència d’execució | Rúbrica | 25% |
| R1M4 | Tancament / verificació | README final + documentació en repositori + justificació tècnica + defensa | RA1d, RA1g | Documentació, validació, defensa, AI log | Rúbrica + checklist | 20% |

### 6.1 Coordinació docent amb sessions de `3` hores

El Repte 1 es compon de `4` microreptes, però la seua execució docent es compacta en `2` sessions principals de treball i una tercera sessió opcional de checkpoint o defensa.

| Sessió | Duració | Microreptes | Focus docent | Producte o evidència clau |
|---|---:|---|---|---|
| `1` | `3h` | R1M1 + inici R1M2 | model client/servidor, decisió inicial i arrencada de l'entorn | fitxa breu + decisió orientativa + base mínima iniciada |
| `2` | `3h` | tancament R1M2 + R1M3 + R1M4 | entorn complet, primer punt d'entrada funcional i documentació | projecte arrancant + punt funcional + README + documentació en repositori |
| `3` | opcional | checkpoint formal | defensa, execució real i revisió de traçabilitat | defensa tècnica o acta de checkpoint |

---

## 7. Evidències globals del repte

**Evidències mínimes comunes**

- repositori actualitzat i usable
- issue mare de kickoff
- historial de commits significatiu
- README executable per tercers
- fitxa breu d’exploració tècnica inicial del `R1M1`
- justificació tècnica breu o ADR curt
- projecte executable amb Docker
- base de dades i phpMyAdmin incorporats a l'entorn inicial quan corresponga al `R1M2`
- primera peça funcional simple del producte
- directori de documentació dins del repositori
- fitxes o documents del repte incorporats al repositori
- índex o pàgina visible que enllaça la documentació
- prova funcional registrada
- explicació del paper de cada servei, decisió tècnica menuda i incidència o dubte real
- defensa tècnica breu
- AI log quan hi haja ús d’IA

**Evidències opcionals d’ampliació**

- formulari inicial
- validació bàsica
- registre o persistència mínima de dades
- checklist d’onboarding per a un tercer
- millor tractament d’errors
- test bàsic automatitzat
- pipeline inicial de qualitat
- millor estructuració de carpetes

---

## 8. Instruments d’avaluació del repte

### 8.1 Instruments principals

- rúbrica del repte
- rúbrica específica dels microprojectes
- checklist de revisió de repositori
- revisió tècnica de README i justificació tècnica
- defensa tècnica breu

### 8.2 Instruments de verificació

- prova d’arrancada seguint només el README
- execució real amb Docker
- demo del punt d’entrada funcional
- preguntes tècniques sobre alternatives descartades
- revisió d’issues i commits
- microcanvi en viu
- contrast entre AI log, documentació i resultat real

---

## 9. Riscos d’ús inadequat de la IA

| Risc | Com es manifesta | Impacte | Mesura de control |
|---|---|---|---|
| Delegació excessiva | codi no comprés ni defensable | Alt | defensa i canvi en viu |
| Comparativa superficial | decisió tècnica pobra | Mitjà | justificació tècnica + preguntes de contrast |
| README fictici | no permet arrancar realment el projecte | Alt | execució real del README |
| Docker aparent | existeix però no permet reproduir l’entorn | Alt | arrencada real amb `docker compose up` o equivalent |
| Traçabilitat pobra | sense rastre del procés ni de les decisions | Mitjà | revisió d’issues i commits |

---

## 10. Mesures de control i verificació

**Per comprovar aprenentatge real**

- demostració funcional
- execució real del projecte
- execució real amb Docker
- defensa tècnica
- revisió de commits
- revisió d’issues
- preguntes de transferència
- canvi tècnic menor en directe
- contrast entre versió inicial, suport d’IA i resultat final validat

**Per distingir nivells d’autonomia**

- **treball autònom real**: l’alumne explica, adapta, corregix i defensa
- **treball assistit per IA**: l’alumne usa suport, però valida i pren decisions
- **treball excessivament delegat**: l’alumne no comprén, no transferix i no pot corregir

---

## 11. Adaptació realista a l’aula

**Duració orientativa**

`6` hores de base, organitzades en `2` sessions principals de `3` hores. Es pot afegir una tercera sessió opcional de `3` hores si cal una defensa o checkpoint formal més pausat.

**Moment del curs**

Inici del mòdul o obertura del projecte evolutiu.

**Prerequisits**

No es pressuposa domini del backend, però sí maneig bàsic d’ordinador, editor i treball tècnic pautat.

**Marc docent acotat de tecnologies**

La tria tècnica de `R1` no hauria de quedar completament oberta.

Per a la implementació base d’aula, convé treballar dins d’un marc clar i comú:

- `Docker`
- `PHP`
- servidor web
- estructura mínima de projecte executable

La decisió guiada de stack en este repte afecta sobretot com s’explica, s’ordena i s’arranca esta base, no encara quin framework gran s’incorporarà després.

**Part comuna del grup**

- issue mare
- README
- justificació tècnica breu
- Docker funcional
- primer punt d’entrada simple
- defensa breu

**Ampliacions realistes**

- millora del `README` i de l’onboarding tècnic
- una segona resposta simple del backend coherent amb el domini
- millor estructuració de carpetes o scripts d’arrancada
- millor tractament d’errors d’arrancada
- primer test o comprovació automatitzada molt simple
- mini checklist tècnic d’obertura per a tercers

**Recuperació o reforç per CA**

- si fallen RA1b, RA1c o RA1g: nova comparativa guiada i defensa tècnica breu
- si fallen RA1d, RA1e o RA1f: reconfiguració de l’entorn, millora del README, ajust de Docker i nova demostració d’arrancada
- si falla l’evidència funcional: reconstrucció del punt d’entrada simple amb verificació en directe

---

## 12. Tancament del repte

**Pregunta de síntesi per a l’alumnat**

Quina base real hem deixat construïda, per què la podem considerar tècnicament viable i què permet fer a continuació en el Repte 2?

**Criteri de superació del repte**

El repte es considera superat quan:

- el servei arranca en local seguint el README
- el projecte és executable de manera reproductible amb Docker
- hi ha una primera peça funcional real del producte
- existix un punt d’entrada funcional simple
- la decisió tecnològica està justificada dins d’un marc docent acotat
- hi ha traçabilitat real de treball
- l’alumnat pot defensar què ha fet, per què i com prepara el pas al repte següent

**Observacions docents**

Per mantindre coherència amb la programació actual del mòdul, este repte s’ha de llegir principalment com a desplegament aplicat de RA1.

El formulari, la validació de dades, el registre d’informació o la persistència poden aparéixer com a extensió puntual, però no haurien de formar part del mínim obligatori del kickoff.

Si es vol fer qualificable també una part de RA5, caldrà ajustar abans la distribució SA → RA i la matriu d’instruments del mòdul.

---

## 13. Ampliació 9→10

**Finalitat**

Aprofundir el kickoff amb una millora tècnica real sobre reproduïbilitat, traçabilitat o criteri d'arrancada, de manera que l'alumnat puga demostrar excel·lència des del primer repte.

**Condició prèvia**

El nucli obligatori del repte ha d'estar complet, funcional i validat.

**Opcions d’ampliació**

- reforçar l'entorn reproductible amb automatització bàsica d'arrancada, comprovació simple d'estat o millor contenidorització
- convertir la justificació tècnica inicial en una ADR més sòlida, amb alternatives descartades i impacte sobre el projecte base

**Ampliació proposada per l’alumne/a**

També es pot proposar una ampliació pròpia si està alineada amb el repte i es valida prèviament amb el professorat.

**Paper de la IA**

La IA es pot usar per contrastar opcions de contenidorització, documentació d'entorn o estructura d'una ADR, però l'alumnat ha d'aportar decisió, validació i defensa pròpia.

**Evidències**

- commit o branca identificable
- justificació tècnica breu o ADR
- prova funcional o demo d'arrancada millorada
- rastre de l'ús de la IA, si n'hi ha hagut
- mini defensa tècnica o preguntes de contrast

**Instruments de verificació**

- checklist curta d'ampliació
- revisió de repositori
- demo funcional
- mini defensa tècnica al tancament del repte

**Perquè compute com a 9→10**

- el nucli està ben resolt
- l’ampliació aporta valor real a l’entorn o a la traçabilitat
- es pot explicar i defensar
- no és ornamental
- no hi ha delegació excessiva en IA
