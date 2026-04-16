# Repte 1. Kickoff funcional d’un servei web backend amb microprojectes i criteris d’avaluació explícits

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
- punt d’entrada funcional simple
- README tècnic executable
- justificació tècnica breu
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
- demo d’arrancada i execució
- evidència d’un punt d’entrada funcional
- justificació tècnica breu
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
> - En la concreció docent d’aula, cada microrepte es resol en una sessió base de `3` hores.

### Microrepte MP1 — Model client/servidor i elecció guiada de stack

**Tipus**

Microtasca d’investigació i decisió tècnica.

**Objectiu**

Entendre el model client/servidor del producte i fixar una base tècnica guiada que siga coherent amb el recorregut del curs.

**Tasca**

L’equip prepara una comparativa breu dins del marc docent del curs i redacta una decisió tècnica argumentada.

La comparativa ha d’incloure:

- paper del client i del servidor dins del producte
- model d’execució
- tipus de servidor o runtime
- encaix amb el curs i amb el projecte
- encaix amb `Docker`, `PHP` i servidor web
- continuïtat per als reptes següents

**Relació amb el producte principal**

Sense una decisió inicial coherent, el kickoff funcional queda en un esquelet poc defensable i difícil de sostindre durant el curs.

**CA coberts**

- **RA1b**: s’han reconegut els avantatges que proporciona la generació dinàmica de pàgines
- **RA1c**: s’han identificat els mecanismes d’execució de codi en els servidors web
- **RA1g**: s’han reconegut i avaluat les eines i frameworks de programació en entorn servidor

**Descripció dels CA en llenguatge docent**

- L’alumnat sap explicar per què un backend dinàmic aporta valor al projecte.
- L’alumnat distingix on i com s’executa el codi del servidor.
- L’alumnat compara opcions de manera guiada i evita eleccions arbitràries.

**Paper de la IA**

La IA pot ajudar a generar una primera comparativa, però la decisió final s’ha de verificar amb documentació i amb el marc docent del curs.

**Evidències obligatòries**

- taula comparativa breu
- justificació tècnica curta o ADR curt
- referència a alternatives descartades
- defensa oral breu

**Instrument d’avaluació**

Rúbrica d’investigació aplicada.

**Indicadors d’assoliment**

- comparativa no superficial
- marc tecnològic acotat i realista
- elecció coherent amb el curs
- justificació oral convincent

**Riscos habituals**

- comparativa massa genèrica
- elecció per preferència personal sense criteri docent
- dispersió tecnològica difícil de sostindre

**Verificació del treball real**

- pregunta oral: “per què esta opció és assumible per al curs i quina has descartat?”
- pregunta oral: “què fa el runtime o servidor triat dins del flux d’execució?”

**Pes orientatiu dins del repte**

20%

### Microrepte MP2 — Entorn executable amb Docker, PHP i servidor web

**Tipus**

Microprojecte procedimental.

**Objectiu**

Inicialitzar el projecte perquè es puga arrancar de manera reproductible en local sobre una base clara de `Docker`, `PHP` i servidor web.

**Tasca**

L’equip:

- crea el repositori
- configura l’entorn mínim
- prepara arrencada amb `docker compose up` o equivalent
- deixa visible el paper de `PHP` i del servidor web
- definix estructura bàsica de carpetes
- establix convencions inicials
- prepara README de posada en marxa
- crea issue mare i primeres microtasques
- valida que una altra persona pot arrancar el projecte seguint la documentació

**Relació amb el producte principal**

Este microprojecte assegura que el servei no és només una idea o una demo local improvisada, sinó una base executable, documentada i reutilitzable.

**CA coberts**

- **RA1c**: s’han identificat els mecanismes d’execució de codi en els servidors web
- **RA1d**: s’han reconegut les funcionalitats que aporten els servidors d’aplicacions i la seua integració amb els servidors web
- **RA1e**: s’han identificat i caracteritzat els principals llenguatges i tecnologies relacionats amb la programació web en entorn servidor
- **RA1f**: s’han verificat els mecanismes d’integració dels llenguatges de marques amb els llenguatges de programació en entorn servidor

**Descripció dels CA en llenguatge docent**

- L’alumnat comprén quin component executa què i amb quin paper.
- L’alumnat identifica com s’integra servidor, aplicació, contenidors i punt d’entrada.
- L’alumnat prepara una base tècnica funcional, no un conjunt d’arxius inconnexos.
- L’alumnat verifica que el projecte es pot executar de manera reproductible.

**Paper de la IA**

La IA pot suggerir fitxers inicials, estructura base o configuracions de Docker, però l’alumnat ha de comprovar que tot allò realment arranca i és coherent amb la seua decisió tècnica.

**Evidències obligatòries**

- repositori creat
- arrencada amb Docker funcional
- issue mare de kickoff
- primers commits significatius
- README executable
- estructura base del projecte
- registre de primera validació d’arrancada

**Instrument d’avaluació**

Checklist tècnica de repositori + revisió docent de README.

**Indicadors d’assoliment**

- el projecte arranca sense passos ocults
- `docker compose up` o equivalent és funcional
- el README és suficient per a tercers
- l’estructura és coherent
- hi ha traçabilitat mínima del procés

**Riscos habituals**

- README incomplet
- Docker present però no usable
- configuració copiada sense entendre
- arrencada només possible en l’ordinador de l’autor

**Verificació del treball real**

- prova en directe d’arrancada seguint únicament el README
- execució real amb Docker
- revisió de commits i issues
- pregunta tècnica sobre la funció del servidor o runtime triat

**Pes orientatiu dins del repte**

35%

### Microrepte MP3 — Primer punt d’entrada funcional del backend

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

### Microrepte MP4 — Documentació tècnica, verificació i checkpoint

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
| MP1 | Investigació / decisió tècnica | Comparativa guiada + justificació tècnica inicial | RA1b, RA1c, RA1g | Taula comparativa, justificació, defensa breu | Rúbrica | 20% |
| MP2 | Procedimental | Repositori executable amb Docker i estructura base | RA1c, RA1d, RA1e, RA1f | Repo, Docker, README, issues, commits, prova d’arrancada | Checklist + revisió | 35% |
| MP3 | Procedimental | Punt d’entrada funcional simple | RA1b, RA1e, RA1f | Demo funcional, logs o captures, evidència d’execució | Rúbrica | 25% |
| MP4 | Tancament / verificació | README final + justificació tècnica + defensa | RA1d, RA1g | Documentació, validació, defensa, AI log | Rúbrica + checklist | 20% |

### 6.1 Coordinació docent amb sessions de `3` hores

| Sessió | Duració | Microrepte | Focus docent | Producte o evidència clau |
|---|---:|---|---|---|
| `1` | `3h` | MP1 | model client/servidor i decisió tècnica guiada | comparativa breu + justificació inicial |
| `2` | `3h` | MP2 | entorn executable amb Docker, PHP i servidor web | projecte arrancant + `README` inicial |
| `3` | `3h` | MP3 | primer punt d’entrada funcional del backend | ruta, vista, `endpoint` o `healthcheck` funcional |
| `4` | `3h` | MP4 | documentació tècnica, verificació i checkpoint | README executable + defensa breu + pas cap a `R2` |

---

## 7. Evidències globals del repte

**Evidències mínimes comunes**

- repositori actualitzat i usable
- issue mare de kickoff
- historial de commits significatiu
- README executable per tercers
- justificació tècnica breu o ADR curt
- projecte executable amb Docker
- primera peça funcional simple del producte
- prova funcional registrada
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

`12` hores de base, organitzades en `4` sessions de `3` hores.

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
