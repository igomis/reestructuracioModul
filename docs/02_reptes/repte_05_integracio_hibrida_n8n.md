# Repte 5. Aplicació web híbrida i integració de serveis externs

## 1. Visió general del repte

**Finalitat del repte**

Construir una funcionalitat híbrida del projecte que combine recursos propis amb serveis, dades o codi de tercers per generar valor nou i útil dins del producte.

Este repte no s’entén com una simple connexió a una API externa ni com una demostració superficial de consum de dades alienes. El seu sentit és integrar informació o serveis heterogenis de manera crítica, transformada i documentada, perquè el sistema faça alguna cosa nova que abans no podia fer.

**Producte principal del repte**

Una funcionalitat híbrida integrada en el projecte, amb:

- consum real d’una o més fonts externes
- tractament o transformació de la informació rebuda
- combinació amb dades o serveis propis del projecte quan siga pertinent
- generació d’una funcionalitat nova amb valor real
- tractament mínim d’errors i incidències d’integració
- proves mínimes o verificacions registrades
- documentació tècnica de la integració

**Context professional simul·lat o realista**

L’equip ja disposa d’un backend funcional, estructurat i capaç d’exposar serveis propis.

Ara ha de demostrar una competència molt habitual en entorns professionals: reutilitzar serveis, fonts de dades o components externs per ampliar el valor del sistema sense reconstruir-ho tot des de zero.

**Relació amb el projecte global del curs**

Este repte reutilitza el sistema construït fins ara i l’obri a l’exterior.

En el Repte 4, el sistema aprenia a exposar serveis propis.

En el Repte 5, el sistema aprén a consumir, integrar, transformar i reaprofitar informació o serveis externs per generar una aplicació híbrida amb sentit.

---

## 2. Relació amb resultats d’aprenentatge

**Resultat d’aprenentatge principal**

- **RA9**: desenvolupament d’aplicacions web híbrides seleccionant i utilitzant tecnologies, frameworks servidor i repositoris heterogenis d’informació

**Resultats d’aprenentatge de suport integrat**

- **RA7**: només com a base del servei propi ja construït, si el projecte el reutilitza en la integració
- **RA6**: només quan calga guardar, transformar o reutilitzar dades procedents de fonts externes dins del sistema

**Justificació curricular**

Este repte permet passar d’un sistema que ja té lògica pròpia, persistència i serveis exposats a un sistema capaç d’interoperar amb recursos externs de forma crítica i útil.

La dificultat no està sols en connectar-se a una font externa, sinó en decidir què aporta realment, com es transforma i com s’integra dins del producte.

En este punt del curs, el repte reutilitza l'API publicada i consumida al Repte 4, posa a prova la robustesa real del backend més enllà del seu ús intern i permet usar `n8n` o una eina equivalent d'orquestració, automatització o integració si s'ajusta millor al cas d'ús.

És compatible amb `Laravel`, `Symfony` i `NestJS` i manté el criteri del repositori: canvien les eines concretes, però no els objectius, les evidències ni la verificació exigida. Quan es treballe `FastAPI`, s'ha d'entendre com a via avançada o excepcional, no com a itinerari base general.

---

## 3. Canvi metodològic que introdueix la IA

**Paper de la IA en este repte**

La IA es pot usar per a:

- explorar possibles APIs, repositoris o serveis externs
- comparar fonts de dades o contractes de serveis
- generar esquelets inicials de connectors o adapters
- proposar estratègies de mapping o transformació
- detectar inconsistències entre formats
- ajudar a redactar documentació tècnica
- suggerir casos de prova sobre la integració

**Què no es delega**

L’alumnat ha de:

- seleccionar críticament la font externa
- justificar per què aporta valor real al producte
- entendre què rep i què transforma
- explicar com es combina la informació externa amb el sistema propi
- provar què passa quan la font externa falla o respon mal
- documentar el flux real de dades i les limitacions de la integració

**Risc principal d’ús inadequat de la IA**

Fer una integració superficial, sense entendre el contracte extern ni la transformació aplicada, o limitar-se a mostrar dades externes sense valor afegit real.

**Mesures de control**

- AI log quan corresponga
- revisió de commits i issues
- demo del flux complet
- casos positius i d’error
- preguntes tècniques sobre la font externa i el mapping
- contrast entre documentació, codi i resultat observat

---

## 4. Estructura del repte

### 4.1 Nucli del repte

**Objectiu del nucli**

Integrar una font externa real dins del projecte i transformar-la en una funcionalitat híbrida amb valor per al producte.

**Lliurable principal**

Mòdul o funcionalitat híbrida integrada en el sistema, amb:

- selecció justificada de la font externa
- connector o mecanisme de consum funcional
- transformació o adaptació de dades
- integració amb una necessitat real del projecte
- tractament mínim d’errors
- proves mínimes o verificacions registrades
- documentació tècnica de la integració

**Criteris d’avaluació principals del nucli**

- CA de **RA9** vinculats a reutilització de codi i informació, integració de fonts externes, creació d’aplicacions híbrides, verificació i documentació
- CA de suport de **RA6** només si la integració exigix guardar, transformar o reutilitzar dades dins del sistema

**Evidències obligatòries del nucli**

- repositori actualitzat
- issue principal del repte i microtasques
- seqüència de commits significativa
- comparativa o justificació de la font externa
- connector funcional
- dades o servei extern recuperat realment
- transformació o integració observable
- demo del cas d’ús híbrid
- tractament mínim d’errors
- documentació tècnica
- AI log quan hi haja ús d’IA

---

## 5. Microprojectes i microtasques del repte

> **Norma del repte**
>
> - Els microprojectes cobrixen sobretot criteris procedimentals d’integració, transformació i reutilització.
> - Cap microprojecte apareix sense el camp **“CA coberts”**.
> - No es considera suficient una simple crida a un servei extern si no hi ha integració amb valor real dins del producte.
> - El repte ha de generar una funcionalitat híbrida, no una demo ornamental de consum de dades.

### Microprojecte MP1 — Selecció de fonts externes i disseny de la integració

**Tipus**

Microtasca d’investigació i decisió tècnica.

**Objectiu**

Seleccionar una o més fonts externes útils i justificar per què tenen sentit dins del producte del curs.

**Tasca**

L’equip analitza alternatives externes, per exemple:

- serveis web públics o privats
- repositoris heterogenis d’informació
- llibreries o components de tercers
- serveis de consulta, validació o enriquiment

L’equip ha de concretar:

- quina font o fonts utilitzarà
- quin contracte extern aprofitarà
- quin valor aportarà la integració
- quin flux de dades seguirà la funcionalitat híbrida

**Relació amb el producte principal**

Sense una selecció crítica de la font externa, el repte corre el risc de convertir-se en una integració arbitrària i sense valor.

**CA coberts**

- **RA9.a**
- **RA9.b**

**Descripció dels CA en llenguatge docent**

- L’alumnat reconeix els avantatges de reutilitzar codi i informació procedent d’altres serveis o repositoris.
- L’alumnat identifica tecnologies, frameworks o fonts aplicables a una integració híbrida.

**Paper de la IA**

La IA pot ajudar a localitzar alternatives i resumir-ne característiques, però l’alumnat ha de justificar la decisió final.

**Evidències obligatòries**

- comparativa breu de fonts externes
- decisió justificada
- esquema del flux d’integració
- defensa oral breu

**Instrument d’avaluació**

Rúbrica de selecció i disseny de la integració.

**Indicadors d’assoliment**

- la font externa està ben triada
- la integració té valor clar per al producte
- el flux previst és viable i comprensible

**Riscos habituals**

- font externa triada per moda o comoditat
- manca de valor real per al producte
- contracte extern mal entés

**Verificació del treball real**

- pregunta oral sobre per què s’ha triat esta font i no una altra
- contrast entre disseny previst i implementació posterior

**Pes orientatiu dins del repte**

15%

---

### Microprojecte MP2 — Connexió amb la font externa i recuperació real d’informació

**Tipus**

Microprojecte procedimental.

**Objectiu**

Consumir realment una font externa i recuperar informació o funcionalitat útil.

**Tasca**

L’equip implementa un connector, client o mecanisme equivalent que permeta:

- connectar-se a la font externa
- recuperar informació o servei real
- gestionar com a mínim un cas correcte
- mostrar almenys un cas d’error o resposta no prevista

**Relació amb el producte principal**

Este microprojecte és el punt on la integració deixa de ser disseny i passa a ser consum real.

**CA coberts**

- **RA9.c**
- **RA9.f**

**Descripció dels CA en llenguatge docent**

- L’alumnat crea una aplicació que recupera i processa informació d’una font existent.
- L’alumnat utilitza informació o codi generats per tercers dins d’una peça funcional real.

**Paper de la IA**

La IA pot suggerir connectors inicials, però l’alumnat ha de demostrar que el consum és real i que entén el format de resposta.

**Evidències obligatòries**

- connector o client funcional
- evidència de dades externes reals
- demo del cas correcte
- demo d’un cas d’error o incidència
- commits associats

**Instrument d’avaluació**

Rúbrica de consum de font externa.

**Indicadors d’assoliment**

- la connexió funciona realment
- la resposta externa és comprensible i usable
- hi ha un mínim de control d’errors

**Riscos habituals**

- simulació de dades externes sense necessitat
- connector que funciona només en un cas molt controlat
- no entendre l’origen ni el format de la resposta

**Verificació del treball real**

- execució en directe del connector
- pregunta oral sobre estructura i significat de la resposta externa

**Pes orientatiu dins del repte**

20%

---

### Microprojecte MP3 — Transformació, mapping i valor afegit

**Tipus**

Microprojecte procedimental.

**Objectiu**

Transformar la informació externa perquè genere valor real dins del producte.

**Tasca**

L’equip implementa una capa de transformació, mapping o tractament que permeta:

- adaptar el format extern al model intern
- combinar dades externes amb dades pròpies quan siga pertinent
- filtrar, enriquir, agrupar o normalitzar informació
- evitar que la integració es limite a mostrar dades crues sense tractament

**Relació amb el producte principal**

És el microprojecte que convertix la integració en aplicació híbrida real.

**CA coberts**

- **RA9.d**
- **RA9.e**

**Descripció dels CA en llenguatge docent**

- L’alumnat crea repositoris o estructures específiques a partir d’informació heterogènia.
- L’alumnat construeix una funcionalitat híbrida amb valor nou i no merament decoratiu.

**Paper de la IA**

La IA pot suggerir estratègies de mapping o transformació, però l’alumnat ha de justificar el model adoptat.

**Evidències obligatòries**

- transformació observable de dades
- explicació del mapping
- demo del valor afegit
- justificació tècnica breu

**Instrument d’avaluació**

Rúbrica de transformació i integració híbrida.

**Indicadors d’assoliment**

- hi ha valor nou respecte a la font externa original
- la transformació és coherent
- la funcionalitat híbrida està clarament integrada al producte

**Riscos habituals**

- mostrar dades externes sense treball propi
- mapping improvisat o poc explicable
- integració ornamental

**Verificació del treball real**

- execució en directe del flux de transformació
- pregunta oral sobre com passa una dada de la font externa al model intern

**Pes orientatiu dins del repte**

25%

---

### Microprojecte MP4 — Integració de la funcionalitat híbrida en el projecte

**Tipus**

Microprojecte procedimental.

**Objectiu**

Incorporar la nova funcionalitat híbrida al producte principal de manera usable i coherent.

**Tasca**

L’equip integra la funcionalitat híbrida dins del projecte de forma que es puga veure:

- on s’activa o s’utilitza
- quina necessitat del producte resol
- com interactua amb funcionalitats ja existents
- quin comportament oferix a l’usuari o al sistema

**Relació amb el producte principal**

Sense esta integració final, el repte podria quedar com una prova aïllada sense impacte real en el producte.

**CA coberts**

- **RA9.e**
- **RA9.f**

**Descripció dels CA en llenguatge docent**

- L’alumnat integra la funcionalitat híbrida dins d’un sistema real.
- L’alumnat reutilitza de manera coherent serveis o repositoris externs per resoldre una necessitat pròpia del projecte.

**Paper de la IA**

La IA pot ajudar a detectar punts d’integració, però l’alumnat ha de demostrar que la funcionalitat híbrida forma part real del producte.

**Evidències obligatòries**

- funcionalitat híbrida integrada
- demo del cas d’ús complet
- ús combinat de font externa i sistema propi
- commits i issue relacionades

**Instrument d’avaluació**

Rúbrica de funcionalitat híbrida integrada.

**Indicadors d’assoliment**

- la funcionalitat no és una demo aïllada
- la integració resol una necessitat real
- el flux complet és comprensible i usable

**Riscos habituals**

- integració superficial
- funcionalitat desconnectada del producte
- reutilització poc justificada

**Verificació del treball real**

- execució en directe del cas d’ús complet
- pregunta oral sobre què aporta la integració que abans el producte no podia fer

**Pes orientatiu dins del repte**

20%

---

### Microprojecte MP5 — Prova, depuració i documentació del flux híbrid

**Tipus**

Microprojecte de tancament i verificació.

**Objectiu**

Deixar clar que la integració és verificable, mantenible i comprensible per tercers.

**Tasca**

L’equip documenta i verifica:

- la font externa usada
- el contracte o tipus de resposta aprofitat
- els punts de transformació
- els casos de prova mínims
- els errors o limitacions principals
- les incidències detectades i correccions aplicades

**Relació amb el producte principal**

Este microprojecte consolida la integració i deixa rastre tècnic suficient perquè es puga mantindre o revisar.

**CA coberts**

- **RA9.g**
- **RA9.h**

**Descripció dels CA en llenguatge docent**

- L’alumnat utilitza llibreries o entorns complementaris quan són útils per a treballar la integració.
- L’alumnat prova, depura i documenta la funcionalitat híbrida amb criteri tècnic.

**Paper de la IA**

La IA pot ajudar a polir documentació o a generar casos de prova inicials, però l’alumnat ha de verificar que tot correspon al sistema real.

**Evidències obligatòries**

- registre de proves mínimes
- casos positius i d’error
- documentació tècnica de la integració
- incidències i correccions
- defensa tècnica breu

**Instrument d’avaluació**

Rúbrica de prova i documentació del flux híbrid.

**Indicadors d’assoliment**

- la integració està provada realment
- la documentació és coherent amb el codi
- es poden identificar límits i riscos de la font externa

**Riscos habituals**

- proves fictícies
- documentació embellida
- no saber explicar què falla o què depén del tercer servei

**Verificació del treball real**

- execució en directe d’un cas positiu i d’un cas d’error
- contrast entre documentació, codi i resultat observat

**Pes orientatiu dins del repte**

20%

---

## 6. Taula resum de microprojectes i criteris d’avaluació

| Microprojecte | Tipus | Producte o lliurable | CA coberts | Evidències principals | Instrument | Pes orientatiu |
|---|---|---|---|---|---|---|
| MP1 | Investigació / decisió tècnica | Selecció de fonts externes i disseny del flux | RA9.a, RA9.b | comparativa, esquema, defensa | rúbrica | 15% |
| MP2 | Procedimental | Connector o consum real de font externa | RA9.c, RA9.f | connector, dades reals, demo, error | rúbrica | 20% |
| MP3 | Procedimental | Transformació, mapping i valor afegit | RA9.d, RA9.e | transformació observable, mapping, demo | rúbrica | 25% |
| MP4 | Procedimental | Funcionalitat híbrida integrada | RA9.e, RA9.f | demo completa, integració, commits | rúbrica | 20% |
| MP5 | Tancament / verificació | Proves i documentació del flux híbrid | RA9.g, RA9.h | proves, errors, documentació, defensa | rúbrica | 20% |

---

## 7. Evidències globals del repte

**Evidències mínimes comunes**

- issue principal amb microtasques
- seqüència de commits significativa
- selecció justificada d’una font externa
- consum real de la font externa
- transformació o reutilització observable
- funcionalitat híbrida integrada al projecte
- cas positiu i cas d’error
- proves mínimes registrades
- documentació tècnica de la integració
- AI log quan hi haja ús d’IA

**Evidències opcionals d’ampliació**

- integració de més d’una font externa
- cachejat o gestió més avançada de la font externa
- repositori derivat o estructura intermèdia pròpia
- analítica o quadre de comandament simple
- automatització periòdica
- tractament d’errors més ric

---

## 8. Instruments d’avaluació del repte

### 8.1 Instruments principals

- rúbrica base del repte
- rúbriques específiques d’integració i transformació
- revisió de repositori
- checklist de qualitat de la integració
- defensa tècnica breu

### 8.2 Instruments de verificació

- execució en directe del flux híbrid
- prova de cas positiu i d’error
- revisió de commits i issues
- preguntes tècniques sobre la font externa i el mapping
- contrast entre documentació, AI log i resultat observat

---

## 9. Riscos d’ús inadequat de la IA

| Risc | Com es manifesta | Impacte | Mesura de control |
|---|---|---|---|
| Integració superficial | es mostren dades externes sense valor nou | Alt | exigir transformació o reutilització amb sentit |
| Contracte extern mal comprés | l’alumne no sap explicar la resposta rebuda | Alt | preguntes tècniques i demo |
| Dependència excessiva del tercer servei | el flux es trenca i no se sap per què | Mitjà-alt | casos d’error obligatoris |
| Documentació fictícia | no correspon al comportament real | Alt | execució dels casos documentats |
| Dependència excessiva de IA | l’alumne no pot explicar la integració | Alt | defensa tècnica i preguntes de transferència |

---

## 10. Mesures de control i verificació

**Per comprovar aprenentatge real**

- execució real del connector
- demostració de la transformació aplicada
- execució del cas d’ús híbrid complet
- prova d’almenys un error o incidència d’integració
- revisió de commits i issues
- pregunta de transferència
- canvi tècnic menut en directe
- contrast entre documentació i comportament observat

**Per distingir nivells d’autonomia**

- **treball autònom real**: l’alumne selecciona, integra, transforma, prova i defensa
- **treball assistit per IA**: l’alumne usa suport, però valida i pren decisions
- **treball excessivament delegat**: l’alumne no entén la font externa ni el mapping aplicat

---

## 11. Adaptació realista a l’aula

**Duració orientativa**

5 a 7 sessions, segons la complexitat de la font externa triada i el nivell del grup.

**Moment del curs**

Després del Repte 4.

**Prerequisits**

- projecte funcional i estructurat
- servei propi o base de serveis ja disponible
- treball mínim amb Git, issues i commits
- criteri bàsic de prova i documentació

**Possibles variants tecnològiques**

Es pot implementar amb l’stack triat pel projecte o departament, sempre que permeta:

- consum de fonts externes
- transformació o mapping de dades
- integració real amb el producte
- prova i documentació del flux híbrid

**Part comuna del grup**

- una font externa real
- un connector funcional
- una transformació amb sentit
- una funcionalitat híbrida integrada
- prova i documentació

**Ampliacions realistes**

- diverses fonts externes
- integració més rica
- transformació més complexa
- repositori derivat propi
- automatització periòdica
- analítica o quadre de comandament simple

**Recuperació o reforç per CA**

- si fallen CA de **RA9.a** o **RA9.b**: nova selecció i justificació de la font externa
- si fallen CA de **RA9.c** o **RA9.f**: correcció del connector i nova demo del consum
- si fallen CA de **RA9.d** o **RA9.e**: revisió del mapping i de la funcionalitat híbrida integrada
- si fallen CA de **RA9.g** o **RA9.h**: nova prova guiada, documentació i defensa tècnica

---

## 12. Tancament del repte

**Pregunta de síntesi per a l’alumnat**

Quina funcionalitat nova hem creat gràcies a la integració amb una font externa i què la fa realment útil dins del producte?

**Criteri de superació del repte**

El repte es considera superat quan:

- existix una integració externa real i justificable
- la font externa es consumix realment
- hi ha transformació, reutilització o valor afegit observables
- la funcionalitat híbrida forma part del producte
- es documenten i proven tant el cas positiu com almenys un cas d’error
- l’alumnat pot explicar tècnicament què rep, què transforma i què aporta la integració

**Observacions docents**

Este repte s’ha de llegir principalment com a desplegament de **RA9**. No hauria de convertir-se ni en una repetició del Repte 4 ni en una simple demostració de consum d’APIs externes sense valor de producte.
