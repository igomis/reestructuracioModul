# Repte 4. API i serveis reutilitzables sobre una funcionalitat real del projecte

## 1. Visió general del repte

**Finalitat del repte**

Convertir una funcionalitat ja estabilitzada del projecte en un servei web reusable, consumible i verificable.

Este repte no s’entén com una simple capa addicional d’endpoints ni com una extensió del treball de persistència. El seu sentit és exposar una part real del producte com a servei útil per a altres clients, components o sistemes, amb un contracte clar i una documentació usable.

**Producte principal del repte**

Una API funcional del projecte, amb:

- almenys un recurs o cas d’ús real exposat com a servei
- contracte clar de peticions i respostes
- endpoints coherents
- autenticació o control d’accés adequat per al servei
- consum verificat del servei
- proves mínimes o verificacions registrades
- documentació tècnica usable per tercers

**Context professional simul·lat o realista**

L’equip ja disposa d’una funcionalitat estructurada i persistent. Ara necessita obrir-la perquè puga ser reutilitzada per una interfície diferent, una integració externa, un client lleuger o un altre servei.

En context professional, este pas exigix definir bé el contracte del servei, el format de dades, les regles d’accés i la manera de provar-lo i documentar-lo.

**Relació amb el projecte global del curs**

Este repte reutilitza el cas d’ús professionalitzat en el Repte 3, però canvia clarament l’objecte principal d’avaluació.

En el Repte 3 es valorava sobretot la qualitat de l’arquitectura interna i la persistència suficient.

En el Repte 4 es valora principalment la capacitat d’exposar eixa funcionalitat com a servei web reusable, consumible i documentat.

---

## 2. Relació amb resultats d’aprenentatge

**Resultat d’aprenentatge principal**

- **RA7**: desenvolupament de serveis web reutilitzables i accessibles mitjançant protocols web, verificant-ne el funcionament

**Resultat d’aprenentatge de suport integrat**

- **RA6**: només en la part necessària per recuperar, publicar i documentar dades reals del sistema a través del servei

**Justificació curricular**

Este repte permet passar d’un backend estructurat a un backend interoperable.

La funcionalitat ja no es mira només des del punt de vista del manteniment intern, sinó des del punt de vista de la seua exposició com a servei per a consum extern o intercomponent.

En este punt del curs, el repte reutilitza la base arquitectònica i de persistència consolidada al Repte 3, transforma funcionalitats internes del producte en una interfície externa clara i versionable, i deixa preparada la infraestructura conceptual i tècnica per al Repte 5.

És compatible amb `Laravel`, `Symfony` i `NestJS` i manté equivalència docent entre stacks: canvia la implementació concreta, no els objectius ni les evidències exigides. Quan es treballe `FastAPI`, s'ha d'entendre com a via avançada o excepcional, no com a itinerari base general.

---

## 3. Canvi metodològic que introdueix la IA

**Paper de la IA en este repte**

La IA es pot usar per a:

- proposar contractes inicials d’API
- generar esquelets d’endpoints
- suggerir estructures de request i response
- ajudar a interpretar errors d’integració
- proposar proves de servei
- ajudar a redactar documentació tècnica
- suggerir exemples d’ús del servei

**Què no es delega**

L’alumnat ha de:

- decidir quina funcionalitat val la pena exposar
- justificar els recursos i endpoints triats
- verificar que el servei retorna dades reals i correctes
- explicar l’autenticació aplicada al context d’API
- demostrar que el servei es pot consumir realment
- documentar allò que efectivament funciona

**Risc principal d’ús inadequat de la IA**

Construir una API aparentment completa però sense criteri de contracte, amb endpoints arbitraris, documentació decorativa o sense consum real verificat.

**Mesures de control**

- AI log quan corresponga
- revisió de commits i issues
- execució en directe d’endpoints
- consum real obligatori del servei
- casos positius i negatius
- preguntes tècniques de contracte i interoperabilitat
- contrast entre documentació, codi i resultat observat

---

## 4. Estructura del repte

### 4.1 Nucli del repte

**Objectiu del nucli**

Publicar una primera API útil i defensable sobre un cas d’ús real del projecte, de manera que una altra peça de programari puga consumir-la en condicions mínimes de claredat, seguretat i verificació.

**Lliurable principal**

Servei web funcional integrat en el projecte, amb:

- un contracte bàsic clar
- un o més endpoints coherents
- dades reals del sistema
- autenticació o control d’accés
- consum verificat
- documentació usable
- proves mínimes o verificacions registrades

**Criteris d’avaluació principals del nucli**

- CA de **RA7** vinculats a caracterització, desenvolupament, verificació, consum i documentació del servei web
- CA de **RA6** vinculats a recuperació, publicació i verificació de dades reals dins del servei

**Evidències obligatòries del nucli**

- repositori actualitzat
- issue principal del repte i microtasques
- seqüència de commits significativa
- mapa d’endpoints
- servei funcional
- dades reals servides
- autenticació o control d’accés en context d’API
- consumidor mínim o prova equivalent
- documentació tècnica
- registre de proves
- AI log quan hi haja ús d’IA

---

## 5. Microprojectes i microtasques del repte

> **Norma del repte**
>
> - Els microprojectes cobrixen sobretot criteris procedimentals i d’interoperabilitat.
> - Cap microprojecte apareix sense el camp **“CA coberts”**.
> - No es considera suficient una col·lecció d’endpoints sense contracte clar, consum real i documentació usable.
> - El repte ha d’exposar una funcionalitat real del projecte, no una API de joguet desconnectada del domini.

### Microprojecte MP1 — Disseny del contracte del servei

**Tipus**

Microtasca d’investigació i decisió tècnica.

**Objectiu**

Decidir quina part del producte s’exposa com a servei i definir un contracte mínim clar per al seu ús.

**Tasca**

L’equip concreta:

- quin recurs o cas d’ús s’exposarà
- quins endpoints tenen sentit
- quin format de dades s’usarà
- quines peticions i respostes s’esperen
- quins errors mínims s’han de contemplar
- quin valor aporta exposar eixa funcionalitat com a servei

**Relació amb el producte principal**

Sense un contracte clar, l’API queda reduïda a una implementació tècnica sense sentit d’interoperabilitat.

**CA coberts**

- **RA7.a**
- **RA7.b**
- **RA7.c**
- **RA7.d**

**Descripció dels CA en llenguatge docent**

- L’alumnat reconeix què és un servei web i per a què és útil.
- L’alumnat identifica tecnologies, protocols o estils adequats.
- L’alumnat justifica el recurs i el contracte del servei.
- L’alumnat dissenya l’exposició del servei amb criteri funcional.

**Paper de la IA**

La IA pot suggerir estructures de contracte o d’endpoints, però l’alumnat ha de validar que encaixen amb el producte real.

**Evidències obligatòries**

- mapa inicial d’endpoints
- taula de peticions i respostes
- justificació del recurs o cas d’ús exposat
- defensa oral breu

**Instrument d’avaluació**

Rúbrica de contracte de servei.

**Indicadors d’assoliment**

- contracte coherent amb el domini
- endpoints amb sentit
- definició clara de request, response i errors bàsics

**Riscos habituals**

- endpoints arbitraris
- contracte poc clar
- exposició d’un recurs sense valor real

**Verificació del treball real**

- pregunta oral sobre per què eixe recurs s’exposa i no un altre
- contrast entre contracte definit i implementació posterior

**Pes orientatiu dins del repte**

15%

---

### Microprojecte MP2 — Implementació del primer endpoint funcional

**Tipus**

Microprojecte procedimental.

**Objectiu**

Publicar un primer endpoint real i verificable sobre el cas d’ús o recurs triat.

**Tasca**

L’equip implementa un primer endpoint que:

- rep una petició coherent amb el contracte
- recupera dades reals del sistema o executa una acció real
- retorna una resposta estructurada
- mostra un comportament observable i verificable

**Relació amb el producte principal**

Este microprojecte és el pas en què el producte deixa de ser només backend intern i passa a oferir funcionalitat reusable.

**CA coberts**

- **RA7.d**
- **RA7.e**
- **RA6.c**
- **RA6.d**

**Descripció dels CA en llenguatge docent**

- L’alumnat implementa el servei segons el contracte triat.
- L’alumnat publica dades reals o resultats reals del sistema.
- L’alumnat integra el servei amb la funcionalitat ja construïda.

**Paper de la IA**

La IA pot ajudar amb esquelets de codi, però l’alumnat ha de provar que el servei funciona realment.

**Evidències obligatòries**

- endpoint funcional
- resposta estructurada
- evidència de dades reals
- demo del cas correcte
- commits associats

**Instrument d’avaluació**

Rúbrica d’endpoint funcional.

**Indicadors d’assoliment**

- el servei respon segons el contracte
- les dades o accions són reals
- la resposta és clara i verificable

**Riscos habituals**

- endpoint decoratiu
- dades simulades sense necessitat
- contracte implementat de manera inconsistent

**Verificació del treball real**

- execució en directe de l’endpoint
- pregunta oral sobre l’origen de les dades servides

**Pes orientatiu dins del repte**

20%

---

### Microprojecte MP3 — Autenticació i control d’accés de l’API

**Tipus**

Microprojecte procedimental.

**Objectiu**

Protegir el servei perquè l’accés als endpoints estiga controlat segons el tipus de recurs o acció publicada.

**Tasca**

L’equip incorpora autenticació o control d’accés adequat al context de servei, per exemple:

- token
- capçalera d’autenticació
- clau d’accés
- altre mecanisme coherent amb l’stack i el nivell del curs

També ha de demostrar:

- cas autoritzat
- cas denegat
- comportament coherent davant absència o error d’autenticació

**Relació amb el producte principal**

Este microprojecte diferencia una API usable i mínimament professional d’un servei obert sense control.

**CA coberts**

- **RA7.e**
- **RA7.f**

**Descripció dels CA en llenguatge docent**

- L’alumnat integra protecció d’accés en un servei web.
- L’alumnat comprova el funcionament correcte i incorrecte del servei protegit.

**Paper de la IA**

La IA pot suggerir patrons d’autenticació, però l’alumnat ha de justificar el mecanisme triat i demostrar-lo.

**Evidències obligatòries**

- mecanisme d’autenticació o control d’accés
- cas autoritzat
- cas denegat
- resposta coherent davant error
- demo d’accés protegit

**Instrument d’avaluació**

Rúbrica de servei protegit.

**Indicadors d’assoliment**

- el control d’accés és real
- la restricció és observable
- el servei respon coherentment en cas positiu i negatiu

**Riscos habituals**

- protecció aparent
- repetir acríticament el model d’autenticació del Repte 2
- no adaptar el control al context d’API

**Verificació del treball real**

- execució en directe de peticions autoritzades i denegades
- pregunta oral sobre en quin punt del flux es comprova l’accés

**Pes orientatiu dins del repte**

20%

---

### Microprojecte MP4 — Consum del servei

**Tipus**

Microprojecte procedimental.

**Objectiu**

Demostrar que el servei es pot reutilitzar realment des d’un client, una eina de proves o una altra peça del sistema.

**Tasca**

L’equip prepara un consumidor mínim del servei, que pot ser:

- una col·lecció de proves amb una eina d’API
- un client simple
- una vista o component consumidor
- un script de consum
- una altra peça equivalent coherent amb el nivell del curs

El consum ha de mostrar:

- ús correcte del servei
- lectura de la resposta
- tractament mínim d’errors o resultats inesperats

**Relació amb el producte principal**

Sense consum verificat, l’API queda definida però no validada com a servei reutilitzable.

**CA coberts**

- **RA7.f**
- **RA7.g**

**Descripció dels CA en llenguatge docent**

- L’alumnat prova el servei en condicions d’ús real.
- L’alumnat consumix el servei des d’un client o eina adequada.
- L’alumnat verifica que l’API és realment reutilitzable.

**Paper de la IA**

La IA pot suggerir exemples de consum, però l’alumnat ha de demostrar-ne el funcionament real.

**Evidències obligatòries**

- consumidor mínim o eina configurada
- demo del consum correcte
- cas d’error o consum invàlid
- registre de prova del servei

**Instrument d’avaluació**

Checklist de consum del servei.

**Indicadors d’assoliment**

- el servei és consumible
- la resposta és usable
- el consumidor no és només ornamental

**Riscos habituals**

- provar només el servidor sense consumidor real
- consum massa trivial
- no tractar cap cas d’error

**Verificació del treball real**

- execució en directe del consumidor
- pregunta oral sobre què necessita un tercer per usar l’API

**Pes orientatiu dins del repte**

20%

---

### Microprojecte MP5 — Documentació i prova del servei

**Tipus**

Microprojecte de tancament i verificació.

**Objectiu**

Deixar el servei documentat i verificable per una altra persona o equip.

**Tasca**

L’equip documenta:

- endpoints disponibles
- format de peticions i respostes
- requisits d’autenticació
- casos de prova mínims
- errors principals
- passos bàsics d’ús

També registra incidències detectades i correccions aplicades.

**Relació amb el producte principal**

Este microprojecte consolida el valor professional del servei i el deixa preparat per a reutilització real.

**CA coberts**

- **RA7.f**
- **RA7.h**
- **RA6.g**

**Descripció dels CA en llenguatge docent**

- L’alumnat prova el servei de manera explícita.
- L’alumnat documenta l’API de forma usable per tercers.
- L’alumnat deixa traçabilitat del comportament real del servei.

**Paper de la IA**

La IA pot ajudar a polir la documentació, però esta ha de correspondre exactament al servei real.

**Evidències obligatòries**

- documentació d’endpoints
- exemples de request i response
- casos de prova mínims
- incidències i correccions
- defensa tècnica breu

**Instrument d’avaluació**

Rúbrica de documentació i verificació del servei.

**Indicadors d’assoliment**

- documentació coherent amb el servei
- proves verificables
- claredat d’ús per tercers

**Riscos habituals**

- documentació embellida
- captures sense correspondència amb l’endpoint real
- proves fictícies

**Verificació del treball real**

- contrast entre documentació, demo i codi
- execució en directe d’un cas documentat
- pregunta oral sobre com consumiria el servei un altre equip

**Pes orientatiu dins del repte**

25%

---

## 6. Taula resum de microprojectes i criteris d’avaluació

| Microprojecte | Tipus | Producte o lliurable | CA coberts | Evidències principals | Instrument | Pes orientatiu |
|---|---|---|---|---|---|---|
| MP1 | Investigació / decisió tècnica | Contracte inicial del servei | RA7.a, RA7.b, RA7.c, RA7.d | mapa d’endpoints, taula request/response, defensa | rúbrica | 15% |
| MP2 | Procedimental | Primer endpoint funcional | RA7.d, RA7.e, RA6.c, RA6.d | endpoint, resposta, demo, dades reals | rúbrica | 20% |
| MP3 | Procedimental | Servei protegit | RA7.e, RA7.f | autenticació, cas autoritzat i denegat | rúbrica | 20% |
| MP4 | Procedimental | Consum real del servei | RA7.f, RA7.g | consumidor, demo, prova d’error | checklist | 20% |
| MP5 | Tancament / verificació | Documentació i prova del servei | RA7.f, RA7.h, RA6.g | documentació, proves, incidències, defensa | rúbrica | 25% |

---

## 7. Evidències globals del repte

**Evidències mínimes comunes**

- issue principal amb microtasques
- seqüència de commits significativa
- contracte bàsic del servei
- almenys un endpoint funcional
- ús de dades reals del sistema
- autenticació o control d’accés del servei
- consumidor mínim o prova equivalent
- casos positius i negatius
- documentació tècnica usable
- registre de proves
- AI log quan hi haja ús d’IA

**Evidències opcionals d’ampliació**

- més d’un endpoint
- més d’un recurs exposat
- consumidor més complet
- proves automatitzades
- control d’errors més ric
- documentació més formalitzada
- integració amb un servei extern

---

## 8. Instruments d’avaluació del repte

### 8.1 Instruments principals

- rúbrica base del repte
- rúbrica específica de servei i interoperabilitat
- checklist de consum del servei
- revisió de repositori
- defensa tècnica breu

### 8.2 Instruments de verificació

- execució en directe d’endpoints
- prova de casos positius i negatius
- consum real del servei
- revisió de commits i issues
- preguntes tècniques sobre contracte, autenticació i reutilització
- contrast entre documentació, AI log i comportament observat

---

## 9. Riscos d’ús inadequat de la IA

| Risc | Com es manifesta | Impacte | Mesura de control |
|---|---|---|---|
| API decorativa | endpoints sense valor real de domini | Alt | exigir servei sobre funcionalitat real |
| Contracte pobre | request/response inconsistents | Alt | revisió del contracte i demo |
| Documentació fictícia | no correspon al comportament real | Alt | execució real dels casos documentats |
| Consum aparent | no hi ha consumidor o és ornamental | Alt | consumidor obligatori o prova equivalent |
| Dependència excessiva de IA | l’alumne no pot justificar el servei | Alt | defensa tècnica i preguntes de transferència |

---

## 10. Mesures de control i verificació

**Per comprovar aprenentatge real**

- execució real del servei
- consum real de l’API
- demostració de cas autoritzat i denegat
- revisió de commits i issues
- contrast entre contracte, implementació i documentació
- pregunta de transferència
- canvi tècnic menut en directe
- comprovació de dades reals servides

**Per distingir nivells d’autonomia**

- **treball autònom real**: l’alumne defineix, publica, prova, consumix i defensa el servei
- **treball assistit per IA**: l’alumne usa suport, però valida i pren decisions
- **treball excessivament delegat**: l’alumne no pot explicar el contracte, el consum ni l’autenticació del servei

---

## 11. Adaptació realista a l’aula

**Duració orientativa**

5 a 7 sessions, segons l’stack triat, el punt de partida del Repte 3 i el nivell del grup en prova de serveis.

**Moment del curs**

Després del Repte 3.

**Prerequisits**

- cas d’ús real ja estructurat
- persistència suficient
- repositori operatiu
- treball mínim amb Git, issues i commits

**Possibles variants tecnològiques**

Es pot implementar amb l’stack triat pel projecte o departament, sempre que permeta:

- exposar endpoints o servicis equivalents
- servir dades reals
- aplicar autenticació o control d’accés
- consumir el servei des d’una eina o client
- documentar i provar el servei

**Part comuna del grup**

- contracte bàsic del servei
- primer endpoint funcional
- protecció d’accés
- consum mínim
- documentació i prova

**Ampliacions realistes**

- diversos recursos
- integració amb front o client separat
- control d’errors més ric
- proves automatitzades de servei
- documentació més formal
- integració externa

**Recuperació o reforç per CA**

- si fallen CA de **RA7**: redisseny del contracte, correcció d’endpoints, nou consum i nova documentació
- si fallen CA de **RA6** de suport: correcció de recuperació o publicació de dades reals i nova verificació
- si fallen proves o consum: nova execució guiada i defensa tècnica breu

---

## 12. Tancament del repte

**Pregunta de síntesi per a l’alumnat**

Quina part real del producte hem aconseguit exposar com a servei reusable, com sabem que es pot consumir i què la fa usable per tercers?

**Criteri de superació del repte**

El repte es considera superat quan:

- existix almenys un servei funcional sobre una funcionalitat real del projecte
- el contracte bàsic del servei és clar i defensable
- el servei retorna dades reals o executa una acció real
- hi ha autenticació o control d’accés coherent
- el servei es pot consumir de manera verificable
- la documentació reflectix el comportament real
- l’alumnat pot explicar tècnicament per què esta API és usable i com es podria integrar

**Observacions docents**

Este repte s’ha de llegir principalment com a desplegament de **RA7** amb suport concret de **RA6**. No hauria de convertir-se en un nou repte general de persistència ni en una simple col·lecció d’endpoints CRUD sense contracte, consum i documentació.
