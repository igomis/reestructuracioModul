# Repte 1. Kickoff funcional d’un servei web backend amb microprojectes i criteris d’avaluació explícits

## 1. Visió general del repte

**Finalitat del repte**  
Iniciar un servei web backend en condicions professionals reals i deixar una base tècnica robusta per al conjunt del curs. Este repte fixa la manera de treballar de l’equip (organització, traçabilitat, documentació i validació) i obliga a entregar ja una primera peça funcional real del producte.

**Producte principal del repte**  
Una primera versió funcional i verificable del servei backend, amb:
- repositori inicial funcional
- decisió tecnològica justificada
- punt d’entrada al producte (landing o equivalent)
- formulari funcional per arreplegar una primera dada útil
- validació mínima al servidor
- registre o persistència bàsica de la informació
- README tècnic executable
- ADR curt de decisió d’arquitectura
- traçabilitat de treball amb issues i commits

**Context professional simulat o realista**  
Un equip backend rep l’encàrrec de posar en marxa un nou servei. No es demana encara el producte complet, però sí una base fiable que permeta mostrar una primera interacció real amb el sistema i deixar rastre tècnic verificable del comportament del servei.

**Relació amb el projecte global del curs**  
Este repte crea la base tècnica, metodològica i documental sobre la qual es construiran els reptes següents. No es considera superat només per triar tecnologia o deixar un esquelet executable: ha d’existir una primera peça funcional del producte.

---

## 2. Relació amb resultats d’aprenentatge

**Resultat d’aprenentatge principal**  
- **RA1**: Selecciona les arquitectures i tecnologies de programació web en entorn servidor, analitzant les seues capacitats i característiques pròpies.

**Resultat d’aprenentatge secundari o transversal**  
- **RA5 (no qualificable principalment en este repte, si es manté la matriu actual del mòdul)**: contribució inicial a l’organització del projecte amb criteris de mantenibilitat, estructura i creixement.

**Justificació curricular**  
El repte permet treballar de forma aplicada la comparativa d’arquitectures, els mecanismes d’execució en servidor, la integració amb llenguatges de marques, les funcionalitats dels servidors d’aplicacions i l’avaluació d’eines i frameworks, però ja traslladant-ho a una primera construcció funcional.

---

## 3. Canvi metodològic que introduïx la IA

**Paper de la IA en este repte**  
La IA es pot usar per a:
- explorar alternatives d’arquitectura i stack
- resumir documentació tècnica
- suggerir esquelets inicials
- proposar checklists de validació
- revisar la claredat del README
- detectar errors de configuració inicial

**Què no es delega**  
L’alumnat ha de:
- decidir amb criteri
- adaptar la proposta al context del repte
- verificar que el projecte arranca
- entendre i explicar l’estructura creada
- justificar per què s’ha triat una opció i no una altra
- demostrar el flux funcional inicial

**Risc principal d’ús inadequat de la IA**  
Acceptar configuracions, comparatives o documentació sense entendre-les ni verificar-les.

**Mesures de control**  
- AI log quan hi haja ús d’IA
- issues i commits amb traçabilitat
- prova en directe del README
- defensa tècnica breu
- microcanvis en viu
- preguntes de transferència sobre alternatives descartades

---

## 4. Nucli del repte

**Objectiu del nucli**  
Deixar operativa una primera versió funcional del servei backend que siga executable, justificable i reutilitzable per als reptes següents.

**Lliurable principal**  
Backend inicial funcional amb:
- punt d’entrada al producte
- primer formulari útil
- validació mínima al servidor
- registre o persistència bàsica
- README
- ADR
- historial de treball traçable

**Criteris d’avaluació principals del nucli**  
- RA1b
- RA1c
- RA1e
- RA1f
- RA1g

**Evidències obligatòries del nucli**  
- repositori funcional
- README executable
- ADR curt
- issue mare de kickoff
- commits significatius
- demo del flux inicial
- evidència de validació mínima
- evidència de registre o persistència bàsica
- AI log quan corresponga

---

## 5. Microprojectes i microtasques del repte

> **Norma del repte**
>
> - Els microprojectes cobrixen sobretot criteris procedimentals.
> - Les microtasques d’investigació cobrixen sobretot criteris conceptuals i de decisió.
> - Cap microprojecte apareix sense el camp **CA coberts**.
> - Cada microprojecte genera evidència verificable.

### Microprojecte MP1 — Comparativa d’arquitectures i elecció de stack

**Tipus**  
Microtasca d’investigació i decisió tècnica.

**Objectiu**  
Comparar 2 o 3 alternatives d’arquitectura o stack de backend i justificar quina s’adopta per al projecte base del curs.

**Tasca**  
L’equip prepara una comparativa breu entre alternatives plausibles i redacta una decisió argumentada que incloga:
- model d’execució
- encaix amb el tipus de producte
- corba d’aprenentatge
- documentació disponible
- escalabilitat docent
- viabilitat de desplegament
- impacte en el treball posterior del curs

**Relació amb el producte principal**  
Sense una decisió tècnica inicial coherent, el kickoff funcional queda en un esquelet poc defensable i difícil de continuar.

**CA coberts**  
- **RA1b**: s’han reconegut els avantatges que proporciona la generació dinàmica de pàgines
- **RA1c**: s’han identificat els mecanismes d’execució de codi en els servidors web
- **RA1g**: s’han reconegut i avaluat les eines i frameworks de programació en entorn servidor

**Descripció dels CA en llenguatge docent**  
- L’alumnat sap explicar per què un backend dinàmic aporta valor al producte triat.
- L’alumnat distingix on i com s’executa el codi del servidor.
- L’alumnat compara eines o frameworks amb criteri i no per preferència superficial.

**Paper de la IA**  
La IA pot ajudar a generar una primera comparativa, però la decisió final s’ha de verificar amb documentació i amb el context real del repte.

**Evidències obligatòries**  
- taula comparativa
- ADR curt
- referència a alternatives descartades
- defensa oral breu

**Instrument d’avaluació**  
Rúbrica d’investigació aplicada.

**Indicadors d’assoliment**  
- comparativa no superficial
- criteris de decisió explícits
- elecció coherent amb el producte
- justificació oral convincent

**Riscos habituals**  
- text generat per IA sense criteri
- comparativa massa genèrica
- elecció no alineada amb el curs

**Verificació del treball real**  
- pregunta oral: “què canviaria si el producte haguera d’exposar una API pública des del primer moment?”
- pregunta oral: “quina alternativa has descartat i per què?”

**Pes orientatiu dins del repte**  
20%

### Microprojecte MP2 — Entorn executable i estructura base del servei

**Tipus**  
Microprojecte procedimental.

**Objectiu**  
Inicialitzar el projecte perquè es puga arrancar de manera reproductible en local i quede organitzat amb una estructura coherent des del primer moment.

**Tasca**  
L’equip:
- crea el repositori
- configura l’entorn mínim
- definix estructura de carpetes
- establix convencions bàsiques
- prepara README de posada en marxa
- crea issue mare i primeres microtasques
- valida que un tercer pot arrancar el projecte seguint la documentació

**Relació amb el producte principal**  
Este microprojecte assegura que el servei no és només una idea o una demo local improvisada, sinó una base executable, documentada i reutilitzable.

**CA coberts**  
- **RA1c**: s’han identificat els mecanismes d’execució de codi en els servidors web
- **RA1d**: s’han reconegut les funcionalitats que aporten els servidors d’aplicacions i la seua integració amb els servidors web
- **RA1e**: s’han identificat i caracteritzat els principals llenguatges i tecnologies relacionats amb la programació web en entorn servidor
- **RA1f**: s’han verificat els mecanismes d’integració dels llenguatges de marques amb els llenguatges de programació en entorn servidor

**Descripció dels CA en llenguatge docent**  
- L’alumnat comprén quin component executa què i amb quin paper.
- L’alumnat identifica com s’integra servidor, aplicació i punt d’entrada.
- L’alumnat prepara una base tècnica funcional, no un conjunt d’arxius inconnexos.
- L’alumnat verifica que hi ha una primera integració real entre el backend i la capa de presentació inicial.

**Paper de la IA**  
La IA pot suggerir fitxers inicials, scripts i estructura base, però l’alumnat ha de comprovar que tot allò realment arranca i és coherent amb la seua decisió tècnica.

**Evidències obligatòries**  
- repositori creat
- issue mare de kickoff
- primers commits significatius
- README executable
- estructura base del projecte
- registre de primera validació d’arrancada

**Instrument d’avaluació**  
Checklist tècnica de repositori + revisió docent de README.

**Indicadors d’assoliment**  
- el projecte arranca sense passos ocults
- el README és suficient per a tercers
- l’estructura és coherent
- hi ha traçabilitat mínima del procés

**Riscos habituals**  
- README incomplet
- configuració copiada sense entendre
- commits pobres o inexistents
- arrencada només possible en l’ordinador de l’autor

**Verificació del treball real**  
- prova en directe d’arrancada seguint únicament el README
- revisió de commits i issues
- pregunta tècnica sobre la funció del servidor o runtime triat

**Pes orientatiu dins del repte**  
25%

### Microprojecte MP3 — Primer flux funcional: entrada, formulari, validació i registre mínim

**Tipus**  
Microprojecte procedimental.

**Objectiu**  
Construir una primera interacció real amb el producte, de manera que el repte no quede reduït a infraestructura o muntatge de framework.

**Tasca**  
L’equip implementa:
- una landing page o equivalent d’entrada al producte
- un formulari útil per al domini
- tractament de la petició en servidor
- validació mínima
- resposta controlada davant entrada correcta i incorrecta
- registre o persistència bàsica de la dada arreplegada

**Relació amb el producte principal**  
És la primera peça funcional real del producte i la demostració que la base creada ja servix per a començar a construir valor.

**CA coberts**  
- **RA1b**: s’han reconegut els avantatges que proporciona la generació dinàmica de pàgines
- **RA1e**: s’han identificat i caracteritzat els principals llenguatges i tecnologies relacionats amb la programació web en entorn servidor
- **RA1f**: s’han verificat els mecanismes d’integració dels llenguatges de marques amb els llenguatges de programació en entorn servidor

**Descripció dels CA en llenguatge docent**  
- L’alumnat és capaç de mostrar per què el backend no és un simple servidor d’arxius estàtics.
- L’alumnat integra formulari, processament i resposta del servidor.
- L’alumnat demostra una primera unió funcional entre interfície inicial i lògica executada en servidor.

**Paper de la IA**  
La IA pot ajudar a proposar validacions o esquelets de codi, però l’alumnat ha de provar-los, adaptar-los i explicar-los.

**Evidències obligatòries**  
- landing o equivalent
- formulari funcional
- validació mínima al servidor
- registre o persistència bàsica
- demo del flux complet
- registre de prova funcional
- captura o log de cas vàlid i cas invàlid

**Instrument d’avaluació**  
Rúbrica de microprojecte funcional.

**Indicadors d’assoliment**  
- el flux funciona de principi a fi
- hi ha validació mínima real
- la dada queda registrada o persistida
- la implementació és comprensible i defensable

**Riscos habituals**  
- formulari decoratiu sense processament real
- validació només aparent
- persistència simulada sense rastre verificable
- codi generat però no dominat

**Verificació del treball real**  
- prova en directe del flux
- canvi menor en viu sobre validació o missatge de resposta
- pregunta tècnica sobre què passa en servidor en rebre la petició

**Pes orientatiu dins del repte**  
35%

### Microprojecte MP4 — Documentació tècnica, validació mínima i defensa

**Tipus**  
Microprojecte de tancament i verificació.

**Objectiu**  
Consolidar el repte amb evidència tècnica verificable i demostrar que el treball realitzat és comprés i reutilitzable.

**Tasca**  
L’equip:
- revisa README
- completa ADR
- registra incidències i com les ha resoltes
- documenta la validació mínima feta
- prepara una defensa tècnica de 5-7 minuts

**Relació amb el producte principal**  
Sense documentació i defensa, el repte pot funcionar, però no queda prou verificat ni transferible a l’equip o als reptes següents.

**CA coberts**  
- **RA1d**: s’han reconegut les funcionalitats que aporten els servidors d’aplicacions i la seua integració amb els servidors web
- **RA1g**: s’han reconegut i avaluat les eines i frameworks de programació en entorn servidor

**Descripció dels CA en llenguatge docent**  
- L’alumnat sap explicar el paper de les peces tècniques triades.
- L’alumnat justifica l’eina o framework usat a partir de la seua experiència en el kickoff, no només d’una lectura teòrica.

**Paper de la IA**  
La IA pot ajudar a polir el text del README o de l’ADR, però la defensa i la validació són responsabilitat directa de l’alumnat.

**Evidències obligatòries**  
- README final
- ADR final
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
- ADR redactat a posteriori sense relació real amb el procés
- defensa memorística

**Verificació del treball real**  
- execució del README
- contrast entre ADR, commits i resultat final
- preguntes de transferència sobre com escala esta base al Repte 2

**Pes orientatiu dins del repte**  
20%

---

## 6. Taula resum de microprojectes i criteris d’avaluació

| Microprojecte | Tipus | Producte o lliurable | CA coberts | Evidències principals | Instrument | Pes orientatiu |
|---|---|---|---|---|---|---|
| MP1 | Investigació / decisió tècnica | Comparativa + ADR inicial | RA1b, RA1c, RA1g | Taula comparativa, ADR, defensa breu | Rúbrica | 20% |
| MP2 | Procedimental | Repositori executable i estructura base | RA1c, RA1d, RA1e, RA1f | Repo, README, issues, commits, prova d’arrancada | Checklist + revisió | 25% |
| MP3 | Procedimental | Landing o equivalent + formulari + validació + registre mínim | RA1b, RA1e, RA1f | Demo funcional, logs/captures, evidència de validació i registre | Rúbrica | 35% |
| MP4 | Tancament / verificació | README final + ADR final + defensa tècnica | RA1d, RA1g | Documentació, validació, defensa, AI log | Rúbrica + checklist | 20% |

---

## 7. Evidències globals del repte

**Evidències mínimes comunes**  
- repositori actualitzat i usable
- issue mare de kickoff
- historial de commits significatiu
- README executable per tercers
- ADR curt de decisió arquitectònica
- primera funcionalitat real del producte
- validació mínima al servidor
- registre o persistència bàsica de la dada
- prova funcional registrada
- defensa tècnica breu
- AI log quan hi haja ús d’IA

**Evidències opcionals d’ampliació**  
- checklist d’onboarding per a un tercer
- millor tractament d’errors
- persistència una mica més robusta
- test bàsic automatitzat
- pipeline inicial de qualitat
- millor estructuració de carpetes

---

## 8. Instruments d’avaluació del repte

### 8.1 Instruments principals
- rúbrica del repte
- rúbrica específica dels microprojectes
- checklist de revisió de repositori
- revisió tècnica de README i ADR
- defensa tècnica breu

### 8.2 Instruments de verificació
- prova d’arrancada seguint només el README
- demo del primer flux funcional
- preguntes tècniques sobre alternatives descartades
- revisió d’issues i commits
- microcanvi en viu
- contrast entre AI log, documentació i resultat real

---

## 9. Riscos d’ús inadequat de la IA

| Risc | Com es manifesta | Impacte | Mesura de control |
|---|---|---|---|
| Delegació excessiva | Codi no comprés ni defensable | Alt | Defensa i canvi en viu |
| Comparativa superficial | Decisió tècnica pobra | Mitjà | ADR + preguntes de contrast |
| README fictici | No permet arrancar realment el projecte | Alt | Execució real del README |
| Validació aparent | Formulari sense tractament real o sense control d’errors | Alt | Demo del flux i casos vàlid/invàlid |
| Traçabilitat pobra | Sense rastre del procés ni de les decisions | Mitjà | Revisió d’issues i commits |

---

## 10. Mesures de control i verificació

**Per comprovar aprenentatge real**
- demostració funcional
- execució real del projecte
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
4 a 6 sessions segons el nivell d’entrada del grup i el grau d’autonomia amb Git i entorn de desenvolupament.

**Moment del curs**  
Inici del mòdul o obertura del projecte evolutiu.

**Prerequisits**  
No es pressuposa domini del backend, però sí maneig bàsic d’ordinador, editor i treball tècnic pautat.

**Possibles variants tecnològiques**  
Es pot implementar amb l’stack que el departament considere coherent amb el conjunt del curs, sempre que permeta:
- servei backend executable
- integració amb entrada inicial al producte
- validació en servidor
- traçabilitat i documentació

**Part comuna del grup**  
- issue mare
- README
- ADR
- primer flux funcional mínim
- defensa breu

**Ampliacions realistes**  
- millora de l’estructura
- persistència més robusta
- tractament d’errors més complet
- primer test automatitzat
- mini pipeline de qualitat

**Recuperació o reforç per CA**  
- si fallen RA1b, RA1c o RA1g: nova comparativa i defensa tècnica guiada
- si fallen RA1d, RA1e o RA1f: reconfiguració de l’entorn, millora del README i nova demostració del flux
- si falla l’evidència funcional: reconstrucció del formulari, validació i registre mínim amb verificació en directe

---

## 12. Tancament del repte

**Pregunta de síntesi per a l’alumnat**  
Quina base real hem deixat construïda, per què la podem considerar professionalment viable i què permet fer a continuació en el Repte 2?

**Criteri de superació del repte**  
El repte es considera superat quan:
- el servei arranca en local seguint el README
- hi ha una primera peça funcional real del producte
- existix punt d’entrada, formulari funcional, validació mínima i registre o persistència bàsica
- la decisió d’arquitectura està justificada
- hi ha traçabilitat real de treball
- l’alumnat pot defensar què ha fet, per què i com prepara el pas al repte següent

**Observacions docents**  
Per mantindre coherència amb la programació actual del mòdul, este repte s’ha de llegir principalment com a desplegament aplicat de RA1. Si es vol fer qualificable també una part de RA5, caldrà ajustar abans la distribució SA -> RA i la matriu d’instruments del mòdul.
