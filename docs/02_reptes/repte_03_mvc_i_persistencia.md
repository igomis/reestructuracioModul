# Repte 3. Arquitectura mantenible i persistència segura sobre un cas d’ús real

## 1. Visió general del repte

**Finalitat del repte**

Convertir el backend funcional dels reptes anteriors en una base més mantenible, estructurada i segura, separant responsabilitats i consolidant una persistència suficient sobre un cas d’ús real del producte.

Este repte no s’entén com una reorganització estètica del codi ni com una simple connexió a base de dades. El seu sentit és professionalitzar una funcionalitat existent i deixar-la preparada per créixer sense deute tècnic crític.

**Producte principal del repte**

Una versió refactoritzada d’almenys un cas d’ús real del domini, amb:

- estructura MVC o equivalent aplicada amb sentit
- separació visible de responsabilitats
- capa o mecanisme de persistència dedicat
- accés segur i coherent a dades
- validacions d’entrada
- tractament d’errors
- proves mínimes o verificacions registrades
- documentació tècnica actualitzada

**Context professional simul·lat o realista**

L’equip ja disposa d’una versió inicial funcional, però el codi ha crescut amb dependències acoblades i poca estabilitat per a evolucionar-lo. Abans d’exposar API o integrar tercers, cal reorganitzar la base del producte, assegurar la persistència i demostrar que la funcionalitat clau continua viva després de la refactorització.

**Relació amb el projecte global del curs**

Este repte reutilitza la funcionalitat construïda fins ara i la transforma en una base més professional. A més, prepara el pas al Repte 4, on la publicació de serveis o API necessitarà una arquitectura interna més clara i una persistència més fiable.

---

## 2. Relació amb resultats d’aprenentatge

**Resultat d’aprenentatge principal**

- **RA5**: desenvolupa aplicacions web identificant i aplicant mecanismes per a separar el codi de presentació de la lògica de negoci

**Resultat d’aprenentatge de suport integrat**

- **RA6**: desenvolupa aplicacions web d’accés a magatzems de dades, aplicant mesures per a mantindre la seguretat i la integritat de la informació

**Justificació curricular**

La programació vigent situa l’arquitectura MVC com a **SA3** vinculada principalment a **RA5**, i reserva un pes més fort i específic d’**RA6** per a **SA4**. Per això, en este repte la persistència s’integra per consolidar un cas d’ús real, però el nucli avaluable principal continua sent la separació de responsabilitats i la millora de mantenibilitat.

---

## 3. Canvi metodològic que introdueix la IA

**Paper de la IA en este repte**

La IA es pot usar per a:

- suggerir estratègies de refactorització per iteracions
- proposar estructures de capes o patrons equivalents
- ajudar a detectar acoblaments i duplicacions
- generar esquelets inicials de proves
- suggerir millores en control d’errors
- ajudar a redactar documentació tècnica i decisions

**Què no es delega**

L’alumnat ha de:

- diagnosticar què està mal acoblat
- justificar per què separa unes responsabilitats i no unes altres
- demostrar que el cas d’ús continua funcionant després de la migració
- explicar què fa la capa de dades i què no ha de fer
- verificar la persistència real
- defensar els trade-offs adoptats

**Risc principal d’ús inadequat de la IA**

Acceptar una refactorització aparentment elegant però aliena al problema real del producte, o incorporar persistència sense entendre les implicacions de seguretat, integritat o manteniment.

**Mesures de control**

- AI log quan corresponga
- revisió de commits i issues
- demostració abans i després
- execució en directe de proves mínimes
- preguntes de transferència
- microcanvis en viu
- contrast entre documentació, codi i comportament observat

---

## 4. Estructura del repte

### 4.1 Nucli del repte

**Objectiu del nucli**

Refactoritzar una funcionalitat real del producte perquè passe d’una implementació inicial més acoblada a una estructura més mantenible, amb persistència segura suficient i evidències verificables de qualitat tècnica.

**Lliurable principal**

Mòdul refactoritzat del producte que incloga:

- estructura MVC o equivalent
- separació de capes o responsabilitats
- almenys un cas d’ús prioritari complet migrat
- persistència real en el cas d’ús seleccionat
- validacions i errors coherents
- proves mínimes o verificacions registrades
- documentació tècnica actualitzada

**Criteris d’avaluació principals del nucli**

- CA de **RA5** vinculats a separació de presentació, lògica i estructura de l’aplicació
- CA de **RA6** vinculats a connexió, recuperació, publicació i seguretat bàsica de dades sobre el cas d’ús prioritzat

**Evidències obligatòries del nucli**

- repositori actualitzat
- issue principal del repte i microtasques
- seqüència de commits significativa
- diagnosi inicial del codi
- cas d’ús abans i després de la migració
- persistència funcional i verificable
- validacions i errors observables
- proves mínimes
- documentació tècnica
- AI log quan hi haja ús d’IA

---

## 5. Microprojectes i microtasques del repte

> **Norma del repte**
>
> - Els microprojectes cobrixen sobretot criteris procedimentals i de qualitat tècnica.
> - Cap microprojecte apareix sense el camp **“CA coberts”**.
> - No es considera suficient una reorganització cosmètica ni una persistència només aparent.
> - El repte ha de professionalitzar un cas d’ús real del producte, no crear una arquitectura buida.

### Microprojecte MP1 — Diagnosi del codi actual i pla de migració

**Tipus**

Microtasca d’investigació i decisió tècnica.

**Objectiu**

Analitzar la implementació actual del cas d’ús seleccionat i detectar quins acoblaments, duplicacions o dependències convé corregir abans de migrar-lo a una arquitectura més neta.

**Tasca**

L’equip audita el codi actual i identifica:

- punts de mescla entre presentació i lògica
- dependències excessives
- parts del flux massa acoblades
- punts febles de persistència o traçabilitat
- proposta de migració per iteracions curtes

**Relació amb el producte principal**

Sense una diagnosi real, la refactorització es convertix fàcilment en un canvi superficial o arbitrari.

**CA coberts**

- **RA5.c**
- **RA5.d**

**Descripció dels CA en llenguatge docent**

- L’alumnat identifica mecanismes reals de separació de responsabilitats.
- L’alumnat analitza el punt de partida i detecta per què l’estructura actual és poc mantenible.

**Paper de la IA**

La IA pot suggerir patrons i riscos habituals, però l’alumnat ha de contrastar-los amb el codi real del projecte.

**Evidències obligatòries**

- diagnosi breu del codi
- mapa inicial de dependències o responsabilitats
- pla de migració
- issue principal i microtasques
- defensa oral breu

**Instrument d’avaluació**

Rúbrica de diagnosi i pla tècnic.

**Indicadors d’assoliment**

- diagnosi concreta i no genèrica
- proposta de migració viable
- connexió clara amb el cas d’ús triat

**Riscos habituals**

- diagnosi superficial
- parlar d’MVC en abstracte sense relació amb el producte
- pla massa gran o inviable

**Verificació del treball real**

- pregunta oral sobre quin acoblament concret es vol eliminar i per què
- contrast entre diagnosi i canvis reals fets després

**Pes orientatiu dins del repte**

15%

---

### Microprojecte MP2 — Separació de capes i migració del primer cas d’ús

**Tipus**

Microprojecte procedimental.

**Objectiu**

Migrar un cas d’ús real del domini a una estructura més neta, separant almenys la coordinació del flux de la lògica de negoci i de la interfície o presentació.

**Tasca**

L’equip reorganitza el cas d’ús seleccionat de manera que quede clar:

- qui rep la petició o entrada
- qui coordina el flux
- on queda la lògica de negoci
- com es prepara la resposta o eixida
- quines peces no han de barrejar responsabilitats

**Relació amb el producte principal**

Este microprojecte és el cor de RA5: sense migració real del cas d’ús, no hi ha arquitectura aplicable.

**CA coberts**

- **RA5.e**
- **RA5.f**

**Descripció dels CA en llenguatge docent**

- L’alumnat aplica mecanismes de separació de capes o rols tècnics.
- L’alumnat migra una funcionalitat real sense perdre comportament.

**Paper de la IA**

La IA pot suggerir esquelets de classes, carpetes o mòduls, però l’alumnat ha de demostrar que la separació és coherent i no ornamental.

**Evidències obligatòries**

- cas d’ús migrat
- estructura de carpetes o mòduls revisada
- demo abans/després
- commits de migració incremental
- nota breu de decisions

**Instrument d’avaluació**

Rúbrica de migració arquitectònica.

**Indicadors d’assoliment**

- separació visible i funcional
- millora real de llegibilitat i mantenibilitat
- conservació del comportament del cas d’ús

**Riscos habituals**

- crear capes buides
- moure fitxers sense canviar responsabilitats
- reescriure massa i perdre control del flux

**Verificació del treball real**

- execució del cas d’ús abans/després
- pregunta oral sobre què ha canviat i què s’ha mantingut

**Pes orientatiu dins del repte**

20%

---

### Microprojecte MP3 — Controladors, serveis i components de presentació o equivalent

**Tipus**

Microprojecte procedimental.

**Objectiu**

Consolidar la separació interna del mòdul refactoritzat i assegurar que els diferents rols tècnics tenen fronteres clares.

**Tasca**

L’equip revisa i ajusta el repartiment de responsabilitats entre:

- controladors o equivalent
- serveis, casos d’ús o equivalent
- vistes, plantilles o mecanisme de resposta
- components auxiliars necessaris

No cal que totes les tecnologies usen exactament la mateixa nomenclatura, però sí una separació clara i defensable.

**Relació amb el producte principal**

Este microprojecte evita que la migració es quede a mitges i reforça la mantenibilitat real.

**CA coberts**

- **RA5.g**
- **RA5.h**

**Descripció dels CA en llenguatge docent**

- L’alumnat consolida l’arquitectura de la funcionalitat migrada.
- L’alumnat sap justificar per què cada peça viu on viu.

**Paper de la IA**

La IA pot proposar patrons o convencions, però l’alumnat ha de validar la coherència amb l’stack i amb el producte.

**Evidències obligatòries**

- estructura final del mòdul
- justificació breu de rols tècnics
- demo del flux complet
- registre d’ajustos realitzats

**Instrument d’avaluació**

Checklist d’arquitectura i mantenibilitat.

**Indicadors d’assoliment**

- fronteres clares entre responsabilitats
- coherència interna del mòdul
- capacitat de defensa tècnica

**Riscos habituals**

- nomenclatura correcta però arquitectura confusa
- duplicació entre capes
- serveis o controladors amb massa responsabilitats

**Verificació del treball real**

- pregunta oral sobre què no hauria de fer cada capa
- microcanvi en viu sobre una part concreta del flux

**Pes orientatiu dins del repte**

15%

---

### Microprojecte MP4 — Persistència segura aplicada al cas d’ús prioritari

**Tipus**

Microprojecte procedimental.

**Objectiu**

Consolidar una persistència real i suficient sobre el cas d’ús migrat, evitant accessos improvisats o poc segurs a dades.

**Tasca**

L’equip implementa o reorganitza la persistència del cas d’ús prioritzat, incloent com a mínim:

- connexió o configuració correcta de la capa de dades
- recuperació d’informació
- publicació o ús de les dades dins de l’aplicació
- operació de creació, actualització o equivalent segons el cas d’ús
- tractament coherent de les dades recuperades

**Relació amb el producte principal**

Este microprojecte dona realitat funcional a la refactorització: el cas d’ús no només està millor estructurat, sinó que treballa amb dades de manera estable.

**CA coberts**

- **RA6.a**
- **RA6.b**
- **RA6.c**
- **RA6.d**

**Descripció dels CA en llenguatge docent**

- L’alumnat entén la tecnologia d’accés a dades que està usant.
- L’alumnat connecta, recupera i mostra o utilitza informació persistent.
- L’alumnat integra l’accés a dades dins del cas d’ús real.

**Paper de la IA**

La IA pot suggerir consultes, configuracions o ús d’ORM, però l’alumnat ha de comprovar-ne el funcionament real i la coherència amb el model de dades.

**Evidències obligatòries**

- persistència funcional
- consulta o operació verificable
- demo de lectura i ús de dades
- evidència d’una operació d’escriptura o actualització quan siga pertinent
- commits associats

**Instrument d’avaluació**

Rúbrica de persistència aplicada.

**Indicadors d’assoliment**

- l’accés a dades és real
- la informació persistent forma part del flux del cas d’ús
- la integració és comprensible i defensable

**Riscos habituals**

- persistència simulada
- accés directe i desordenat des de múltiples llocs
- dades sense coherència funcional

**Verificació del treball real**

- execució en directe d’una lectura i d’una operació d’escriptura o actualització
- pregunta oral sobre per què esta acció pertany a la capa de dades i no a una altra

**Pes orientatiu dins del repte**

20%

---

### Microprojecte MP5 — Validacions, errors i regressió mínima

**Tipus**

Microprojecte procedimental.

**Objectiu**

Assegurar que el cas d’ús refactoritzat no sols està més ordenat, sinó també més robust davant dades incorrectes i canvis futurs.

**Tasca**

L’equip incorpora:

- validacions d’entrada
- tractament coherent d’errors
- proves mínimes o verificacions registrades del flux crític
- comprovació que la funcionalitat principal continua viva després de la migració

**Relació amb el producte principal**

Sense esta capa, la refactorització pot ser elegant però fràgil i poc fiable.

**CA coberts**

- **RA6.f**
- **RA6.g**

**Descripció dels CA en llenguatge docent**

- L’alumnat prova i documenta el comportament de l’accés a dades i del cas d’ús.
- L’alumnat reforça la seguretat i la integritat funcional de la informació.

**Paper de la IA**

La IA pot suggerir casos de prova o missatges d’error, però l’alumnat ha de verificar-los amb execució real.

**Evidències obligatòries**

- registre de proves mínimes
- cas positiu i cas negatiu
- tractament visible d’errors
- incidències detectades i corregides
- demo del flux complet verificat

**Instrument d’avaluació**

Checklist de qualitat mínima + revisió de proves.

**Indicadors d’assoliment**

- hi ha prova real del flux
- els errors són observables i coherents
- la funcionalitat no s’ha trencat en la migració

**Riscos habituals**

- proves fictícies
- errors no tractats
- refactorització que trenca el cas d’ús original

**Verificació del treball real**

- execució en directe de proves mínimes
- contrast entre error provocat i resposta del sistema

**Pes orientatiu dins del repte**

15%

---

### Microprojecte MP6 — Documentació tècnica i preparació del Repte 4

**Tipus**

Microprojecte de tancament i verificació.

**Objectiu**

Deixar el cas d’ús refactoritzat documentat i en condicions de servir de base per a la fase següent del projecte.

**Tasca**

L’equip:

- actualitza README o documentació equivalent
- registra decisions arquitectòniques
- anota punts de deute tècnic encara oberts
- explica què queda preparat per al Repte 4
- defensa oralment les decisions adoptades

**Relació amb el producte principal**

Este microprojecte fixa l’aprenentatge i connecta el repte amb la següent fase del projecte evolutiu.

**CA coberts**

- **RA5.f**
- **RA5.g**
- **RA6.g**

**Descripció dels CA en llenguatge docent**

- L’alumnat sap explicar l’arquitectura adoptada.
- L’alumnat documenta decisions i estat real del mòdul.
- L’alumnat deixa traçabilitat i continuïtat d’equip.

**Paper de la IA**

La IA pot ajudar a polir la redacció, però la documentació ha de correspondre al sistema real i la defensa és responsabilitat directa de l’alumnat.

**Evidències obligatòries**

- README tècnic actualitzat
- registre de decisions
- llista de deute tècnic pendent
- defensa tècnica breu

**Instrument d’avaluació**

Rúbrica de defensa + checklist de documentació.

**Indicadors d’assoliment**

- documentació coherent amb el codi
- decisions justificades
- connexió clara amb el pas a API o serveis del repte següent

**Riscos habituals**

- documentació embellida
- decisions redactades a posteriori sense correspondència real
- no saber explicar per què l’arquitectura és millor que abans

**Verificació del treball real**

- contrast entre README, commits i resultat
- pregunta oral sobre què facilita esta arquitectura de cara al Repte 4

**Pes orientatiu dins del repte**

15%

---

## 6. Taula resum de microprojectes i criteris d’avaluació

| Microprojecte | Tipus | Producte o lliurable | CA coberts | Evidències principals | Instrument | Pes orientatiu |
|---|---|---|---|---|---|---|
| MP1 | Investigació / decisió tècnica | Diagnosi i pla de migració | RA5.c, RA5.d | diagnosi, pla, issues, defensa breu | rúbrica | 15% |
| MP2 | Procedimental | Cas d’ús migrat a arquitectura més neta | RA5.e, RA5.f | migració, demo abans/després, commits | rúbrica | 20% |
| MP3 | Procedimental | Consolidació de capes i responsabilitats | RA5.g, RA5.h | estructura final, justificació, demo | checklist | 15% |
| MP4 | Procedimental | Persistència segura aplicada al cas d’ús | RA6.a, RA6.b, RA6.c, RA6.d | lectura/escriptura, demo, commits | rúbrica | 20% |
| MP5 | Procedimental | Validacions, errors i regressió mínima | RA6.f, RA6.g | proves, incidències, demo | checklist | 15% |
| MP6 | Tancament / verificació | Documentació i preparació del Repte 4 | RA5.f, RA5.g, RA6.g | README, decisions, defensa | rúbrica + checklist | 15% |

---

## 7. Evidències globals del repte

**Evidències mínimes comunes**

- issue principal amb microtasques
- seqüència de commits significativa
- diagnosi inicial del codi
- cas d’ús real seleccionat
- demo abans/després
- arquitectura més clara i defensable
- persistència funcional i verificable
- validacions i errors visibles
- proves mínimes o verificacions registrades
- documentació tècnica actualitzada
- AI log quan hi haja ús d’IA

**Evidències opcionals d’ampliació**

- més d’un cas d’ús migrat
- major cobertura de proves
- millor tractament de deute tècnic
- persistència més rica
- observabilitat o logging millorats
- preparació més explícita per a API

---

## 8. Instruments d’avaluació del repte

### 8.1 Instruments principals

- rúbrica base del repte adaptada al pes principal de RA5 i suport de RA6
- rúbriques específiques de migració i persistència
- checklist d’arquitectura i mantenibilitat
- checklist de persistència i seguretat bàsica
- defensa tècnica breu

### 8.2 Instruments de verificació

- demostració del cas d’ús abans i després
- execució real de lectura i escriptura o actualització
- revisió de commits i issues
- execució en directe de proves mínimes
- preguntes tècniques breus
- contrast entre AI log, documentació i resultat observat

---

## 9. Riscos d’ús inadequat de la IA

| Risc | Com es manifesta | Impacte | Mesura de control |
|---|---|---|---|
| Refactorització superficial | arquitectura aparentment ordenada però sense canvi real | Alt | demo abans/després i revisió de commits |
| Capes buides o innecessàries | més complexitat i pitjor manteniment | Alt | defensa tècnica i checklist d’arquitectura |
| Persistència insegura o mal integrada | dades inconsistents o flux fràgil | Alt | demo real i revisió dirigida |
| Proves fictícies | documentació sense correspondència amb el codi | Alt | execució real |
| Dependència excessiva de IA | l’alumne no pot explicar trade-offs | Alt | preguntes orals i microcanvis en viu |

---

## 10. Mesures de control i verificació

**Per comprovar aprenentatge real**

- demostració del cas d’ús abans i després
- execució real de persistència
- revisió de commits i issues
- execució de proves mínimes
- provocació d’errors controlats
- preguntes de transferència
- canvi tècnic menut en directe
- contrast entre documentació i sistema observat

**Per distingir nivells d’autonomia**

- **treball autònom real**: l’alumne diagnostica, refactoritza, prova i defensa
- **treball assistit per IA**: l’alumne usa suport, però valida i pren decisions
- **treball excessivament delegat**: l’alumne no comprén la nova arquitectura ni pot mantindre-la

---

## 11. Adaptació realista a l’aula

**Duració orientativa**

6 a 8 sessions, segons la qualitat de partida del codi del Repte 2 i l’stack triat.

**Moment del curs**

Després del Repte 2 i abans del Repte 4.

**Prerequisits**

- funcionalitat real heretada del Repte 2
- repositori operatiu
- treball mínim amb issues i commits
- base d’accés a dades o necessitat clara d’introduir-la per al cas d’ús

**Possibles variants tecnològiques**

Es pot implementar amb MVC clàssic o arquitectura equivalent, sempre que permeta:

- separació clara de responsabilitats
- migració d’un cas d’ús real
- persistència funcional
- validacions i errors
- documentació i verificació

**Part comuna del grup**

- diagnosi inicial
- migració d’un cas d’ús
- separació de capes
- persistència suficient
- proves mínimes
- documentació i defensa

**Ampliacions realistes**

- més d’un cas d’ús migrat
- millor cobertura de proves
- major qualitat de persistència
- major neteja de deute tècnic
- preparació més avançada del Repte 4

**Recuperació o reforç per CA**

- si fallen CA de **RA5**: nova diagnosi, nova migració parcial i defensa arquitectònica
- si fallen CA de **RA6**: correcció de connexió, recuperació, publicació o tractament de dades amb nova verificació
- si fallen proves o documentació: nova execució guiada, registre d’errors i defensa curta

---

## 12. Tancament del repte

**Pregunta de síntesi per a l’alumnat**

Què hem fet perquè el producte no sols funcione, sinó que siga més mantenible i fiable, i què deixa esta nova base preparada per al Repte 4?

**Criteri de superació del repte**

El repte es considera superat quan:

- existix almenys un cas d’ús real del producte migrat a una arquitectura més neta
- la separació de responsabilitats és visible i defensable
- la persistència és funcional i verificable en el cas d’ús prioritzat
- hi ha validacions i tractament d’errors coherents
- existixen proves mínimes o verificacions reals
- la documentació reflectix l’estat real del sistema
- l’alumnat pot explicar tècnicament les decisions adoptades

**Observacions docents**

Este repte s’ha de llegir principalment com a desplegament de **RA5** amb suport integrat de **RA6**. Si més avant es vol ampliar el pes específic de persistència i seguretat de dades, convindrà fer-ho en el repte o situació equivalent que faça de pont amb l’actual SA4.
