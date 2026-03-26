# Repte 2. Sessions, autenticació i primera funcionalitat de negoci amb microprojectes i criteris d’avaluació explícits

## 1. Visió general del repte

**Finalitat del repte**

Construir la primera funcionalitat de negoci real del producte backend del curs a partir d’una progressió més ampla que la simple autenticació. Este repte obri `SA2` des de la recepció i el tractament bàsic de dades, passa per la lògica del flux i l’estat, i només després arriba a l’autenticació i a la protecció d’una operació real del domini.

**Producte principal del repte**

Una primera funcionalitat de domini real, treballada de manera progressiva, amb:

- formulari base útil per al producte
- recuperació de dades enviades al servidor
- processament bàsic de la petició
- ús de decisions, arrays i funcions aplicades al flux
- estat mantingut amb sessió, cookies o mecanisme equivalent
- autenticació funcional
- almenys una operació de negoci protegida
- validació i tractament mínim d’errors
- proves o verificacions registrades
- documentació tècnica actualitzada

**Context professional simulat o realista**

Després del kickoff, l’equip ja disposa d’un repositori funcional, però encara no ha convertit la base tècnica en un flux usable del producte. En un backend professional, abans d’escapar cap a arquitectura més complexa o cap a `API`, cal demostrar que el sistema rep dades, les processa amb criteri, manté estat quan cal, identifica l’usuari i protegix una operació real del domini.

**Relació amb el projecte global del curs**

Este repte reutilitza la base creada en el Repte 1 i prepara explícitament el pas al Repte 3. No és una activitat aïllada: és la primera seqüència funcional completa del producte, des del formulari i la petició fins a l’estat, l’autenticació i una operació protegida amb valor real.

---

## 2. Relació amb resultats d’aprenentatge

**Resultats d’aprenentatge principals**

- **RA2**: tractament de peticions, dades d’entrada, validació, resposta i control bàsic d’errors del costat servidor
- **RA3**: construcció de lògica de flux amb formularis, recuperació de dades, decisions, arrays i funcions aplicades al producte
- **RA4**: gestió d’estat, sessió o equivalent, autenticació i funcionalitat protegida orientada a un cas d’ús real

**Justificació curricular**

La `SA2` de la programació vigent treballa `RA2`, `RA3` i `RA4` com un bloc funcional continu. Per això, este repte no entra directament en login i control d’accés, sinó que els prepara amb una progressió curricular més coherent:

- primer formulari i recuperació de dades
- després processament bàsic i lògica del flux
- després estat, sessió o cookies
- i finalment autenticació i primera operació protegida

Esta seqüència manté el sentit professional del repte actual: login i logout a soles no són suficients; han d’acabar donant suport a una funcionalitat de domini real i verificable.

---

## 3. Canvi metodològic que introduïx la IA

**Paper de la IA en este repte**

La IA es pot usar per a:

- proposar estructures de formulari i recepció de dades
- suggerir validacions bàsiques i missatges d’error
- ajudar a ordenar decisions, arrays i funcions del flux
- orientar en l’ús de sessió, cookies o mecanisme equivalent
- plantejar casos de prova positius i negatius
- ajudar a interpretar errors de depuració i a documentar incidències

**Què no es delega**

L’alumnat ha de:

- entendre quines dades rep el servidor i com les tracta
- explicar la lògica del flux abans d’arribar a autenticació
- justificar com es manté l’estat i què es comprova en cada pas
- demostrar que l’operació protegida és real i no decorativa
- provar els casos correctes i incorrectes
- identificar què haurà de reorganitzar-se en el Repte 3

**Risc principal d’ús inadequat de la IA**

Copiar formularis, fluxos de tractament o autenticació sense entendre què s’està rebent, què s’està validant, com es manté l’estat o per què una acció queda protegida.

**Mesures de control**

- AI log quan corresponga
- revisió de commits i issues
- execució en directe de casos positius i negatius
- preguntes tècniques breus sobre petició, lògica, estat i autenticació
- modificació menuda en viu
- contrast entre documentació, codi i comportament observat

---

## 4. Nucli del repte

**Objectiu del nucli**

Deixar operativa una primera seqüència funcional completa del producte que recórrega formulari, tractament de dades, lògica, estat i autenticació, i que acabe en una operació real del domini protegida i verificable.

**Lliurable principal**

Mòdul funcional integrat en el producte backend del curs que incloga:

- formulari base i recuperació de dades
- processament bàsic de la petició
- lògica del flux resolta amb decisions, arrays i funcions
- estat o context mantingut entre peticions
- login i logout o mecanisme equivalent coherent amb l’stack
- una operació real del domini protegida
- validació i errors mínims visibles
- proves bàsiques o registre de verificació
- documentació tècnica actualitzada

**Criteris d’avaluació principals del nucli**

- `RA2.c`, `RA2.d`, `RA2.e`, `RA2.f`, `RA2.g`, `RA2.h`
- `RA3.a`, `RA3.b`, `RA3.c`, `RA3.d`, `RA3.e`, `RA3.f`, `RA3.g`
- `RA4.a`, `RA4.b`, `RA4.c`, `RA4.d`, `RA4.e`, `RA4.f`

**Evidències obligatòries del nucli**

- repositori actualitzat
- issue principal del repte i microtasques
- seqüència de commits significativa
- formulari base i recuperació de dades verificables
- processament bàsic amb resposta del servidor
- ús observable de lògica amb decisions, arrays i funcions
- estat o sessió comprovable
- demo funcional d’autenticació i cas d’ús protegit
- casos positius i negatius verificats
- documentació tècnica actualitzada
- AI log quan hi haja ús d’IA

---

## 5. Microprojectes i microtasques del repte

**Norma del repte**

- Els microprojectes cobrixen la progressió real de `SA2` i no només el tram final d’autenticació.
- Cap microprojecte apareix sense el camp **CA coberts**.
- El repte no es considera resolt si hi ha login o logout però no hi ha un cas d’ús real protegit.
- El pas al Repte 3 només té sentit si el flux actual ja funciona de manera reproduïble i mínimament explicable.

### Microprojecte MP1 — Formulari base i recuperació de dades

**Tipus**

Microprojecte procedimental d’entrada al flux.

**Objectiu**

Obrir el repte des d’un formulari base útil per al producte i demostrar que el servidor rep i recupera les dades enviades de manera controlada.

**Tasca**

L’equip ha de:

- definir un formulari base coherent amb el domini
- enviar una primera dada útil al servidor
- recuperar els valors rebuts
- identificar camps, mètode i estructura mínima de la petició
- mostrar una resposta inicial controlada a partir de les dades recuperades

**Relació amb el producte principal**

Este microprojecte impedix començar `SA2` directament en autenticació sense haver consolidat abans l’entrada bàsica de dades del producte.

**CA coberts**

- `RA3.e`
- `RA3.f`
- `RA3.g`

**Descripció dels CA en llenguatge docent**

- L’alumnat sap construir un formulari amb sentit dins del producte.
- L’alumnat sap identificar què arriba al servidor i en quin format mínim.
- L’alumnat recupera i usa les dades rebudes sense reduir el formulari a una peça decorativa.

**Paper de la IA**

La IA pot ajudar a proposar l’estructura del formulari o els camps mínims, però l’equip ha de validar que la recuperació de dades és real i explicable.

**Evidències obligatòries**

- formulari base operatiu
- evidència de dades recuperades
- captura o registre del primer enviament correcte
- breu explicació del camp o dada triada

**Instrument d’avaluació**

Checklist de formulari i recuperació de dades.

**Indicadors d’assoliment**

- el formulari té sentit dins del domini
- les dades arriben i es recuperen correctament
- l’alumnat sap explicar què s’ha rebut i què no

**Riscos habituals**

- formulari dibuixat però no connectat al servidor
- recuperació aparent sense entendre què arriba
- camps sense relació amb el producte

**Verificació del treball real**

- enviament en directe del formulari base
- pregunta tècnica sobre camps, mètode i dades recuperades

**Pes orientatiu dins del repte**

10%

### Microprojecte MP2 — Processament bàsic de la petició i lògica del formulari

**Tipus**

Microprojecte procedimental.

**Objectiu**

Processar la petició del formulari amb criteri de servidor, aplicar validacions bàsiques i produir respostes coherents en cas correcte i incorrecte.

**Tasca**

L’equip ha de:

- tractar la petició rebuda al servidor
- comprovar camps obligatoris o restriccions bàsiques
- generar resposta coherent en cas correcte
- generar resposta d’error mínima en cas incorrecte
- deixar clar quina part del flux és validació i quina és resposta

**Relació amb el producte principal**

Sense este pas, el repte quedaria en recepció aparent de dades però no en tractament real de peticions, que és el nucli d’entrada de `RA2`.

**CA coberts**

- `RA2.c`
- `RA2.d`
- `RA2.e`
- `RA2.f`
- `RA2.g`
- `RA2.h`

**Descripció dels CA en llenguatge docent**

- L’alumnat sap processar la petició en servidor.
- L’alumnat valida dades bàsiques abans de donar-les per bones.
- L’alumnat diferencia el cas correcte del cas incorrecte.
- L’alumnat produïx respostes mínimament comprensibles i verificables.

**Paper de la IA**

La IA pot suggerir validacions o esquelets de processament, però l’equip ha de comprovar què s’accepta, què es rebutja i què es retorna.

**Evidències obligatòries**

- processament funcional de la petició
- cas correcte i cas incorrecte
- evidència de validació bàsica del costat servidor
- missatges d’error mínims visibles
- commits i issue relacionades

**Instrument d’avaluació**

Rúbrica de processament de petició + checklist de validació.

**Indicadors d’assoliment**

- la petició es tracta realment al servidor
- hi ha validació mínima observable
- la resposta canvia segons el cas
- els errors no són merament ornamentals

**Riscos habituals**

- validar només el cas feliç
- barrejar lògica i resposta sense criteri mínim
- error genèric que no deixa clar què falla

**Verificació del treball real**

- execució en directe d’un cas correcte
- execució en directe d’un cas incorrecte
- pregunta tècnica sobre què es comprova abans de continuar el flux

**Pes orientatiu dins del repte**

20%

### Microprojecte MP3 — Decisions, arrays i funcions aplicades al flux

**Tipus**

Microprojecte procedimental de consolidació lògica.

**Objectiu**

Aplicar decisions, arrays i funcions al flux del repte perquè la resolució no quede reduïda a codi lineal, repetit o difícil d’explicar.

**Tasca**

L’equip ha de:

- usar decisions per separar casos del flux
- utilitzar arrays per agrupar dades, regles o missatges
- encapsular parts repetides o significatives en funcions
- fer que esta lògica done suport al formulari i al tractament bàsic de la petició

**Relació amb el producte principal**

Este microprojecte dona coherència interna al flux abans d’arribar a l’estat i a l’autenticació. Sense esta capa, el repte quedaria funcional però massa fràgil i poc explicable.

**CA coberts**

- `RA3.a`
- `RA3.b`
- `RA3.c`
- `RA3.d`

**Descripció dels CA en llenguatge docent**

- L’alumnat usa decisions amb sentit dins del flux.
- L’alumnat aprofita arrays per ordenar informació del procés.
- L’alumnat crea funcions quan ajuden a fer el codi més clar i reutilitzable.
- L’alumnat sap explicar per què la lògica no està tota repetida o dispersa.

**Paper de la IA**

La IA pot proposar refactors menuts o estructures de suport, però l’equip ha de justificar per què usa una funció, un array o una decisió en eixe punt concret.

**Evidències obligatòries**

- ús visible de decisions en el flux
- ús visible d’arrays
- almenys una funció rellevant per al cas d’ús
- explicació breu de la lògica aplicada

**Instrument d’avaluació**

Revisió de codi docent + rúbrica de lògica aplicada.

**Indicadors d’assoliment**

- la lògica està organitzada amb criteri mínim
- arrays i funcions tenen sentit funcional
- l’alumnat pot explicar el recorregut del flux

**Riscos habituals**

- codi lineal i repetit
- funcions afegides només per decoració
- arrays sense paper real en la resolució

**Verificació del treball real**

- explicació en directe del flux amb els seus punts de decisió
- pregunta tècnica sobre què conté un array o què resol una funció concreta

**Pes orientatiu dins del repte**

15%

### Microprojecte MP4 — Estat, sessió i/o cookies

**Tipus**

Microprojecte procedimental.

**Objectiu**

Introduir i demostrar el manteniment mínim d’estat entre peticions abans d’arribar a autenticació completa.

**Tasca**

L’equip ha de:

- mantindre una dada o context mínim entre peticions
- usar sessió, cookies o mecanisme equivalent segons l’stack
- comprovar el comportament abans, durant i després del manteniment d’estat
- deixar clar què guarda el sistema i amb quin propòsit

**Relació amb el producte principal**

Este microprojecte prepara l’entrada a autenticació des d’una base més curricular i comprensible. Primer es treballa l’estat; després s’usa eixe coneixement per protegir una operació real.

**CA coberts**

- `RA4.a`
- `RA4.b`
- `RA4.c`

**Descripció dels CA en llenguatge docent**

- L’alumnat sap mantindre estat mínim entre peticions.
- L’alumnat sap comprovar quan eixe estat existix o deixa d’existir.
- L’alumnat distingix entre tindre dades puntuals i mantindre context funcional.

**Paper de la IA**

La IA pot suggerir patrons de sessió o cookies, però l’equip ha de saber què es guarda i com es comprova en temps d’execució.

**Evidències obligatòries**

- estat mínim funcional
- comprovació de lectura de l’estat
- comprovació de canvi o invalidació de l’estat
- explicació breu del mecanisme triat

**Instrument d’avaluació**

Checklist de sessió o estat equivalent.

**Indicadors d’assoliment**

- l’estat és observable
- hi ha comprovació abans i després del canvi
- el mecanisme triat és explicable

**Riscos habituals**

- estat aparent però no verificable
- guardar dades sense saber per a què servixen
- confondre sessió, cookie i autenticació

**Verificació del treball real**

- execució en directe de lectura i canvi d’estat
- pregunta tècnica sobre què queda guardat i quan s’elimina

**Pes orientatiu dins del repte**

15%

### Microprojecte MP5 — Autenticació i primera operació protegida

**Tipus**

Microprojecte procedimental.

**Objectiu**

Convertir l’estat treballat en un flux d’autenticació funcional i usar-lo per protegir almenys una operació real del domini.

**Tasca**

L’equip ha de:

- implementar login i logout o mecanisme equivalent coherent amb l’stack
- comprovar usuari autenticat
- protegir almenys una operació de negoci del producte
- demostrar un cas autoritzat i un cas denegat
- evitar que el repte quede reduït a pantalla d’accés sense valor funcional

**Relació amb el producte principal**

És el tram que manté la idea central del repte: login i logout a soles no són suficients; han de sostindre una operació de negoci real i protegida.

**CA coberts**

- `RA4.d`
- `RA4.e`

**Descripció dels CA en llenguatge docent**

- L’alumnat sap usar l’autenticació per controlar una acció real del producte.
- L’alumnat demostra què es permet i què es denega.
- L’alumnat diferencia infraestructura d’accés i funcionalitat de negoci protegida.

**Paper de la IA**

La IA pot ajudar a plantejar el flux o els casos de prova, però l’equip ha de demostrar que la protecció és real i no només aparent.

**Evidències obligatòries**

- login funcional
- logout funcional
- comprovació d’usuari autenticat
- operació protegida real
- cas autoritzat
- cas denegat
- evidència de restricció o control aplicat

**Instrument d’avaluació**

Rúbrica de funcionalitat autenticada i protegida.

**Indicadors d’assoliment**

- l’autenticació funciona
- l’operació protegida té valor real
- el cas denegat és observable
- el flux complet és defensable

**Riscos habituals**

- login funcional però sense operació protegida real
- protecció decorativa
- cas denegat no provat

**Verificació del treball real**

- execució en directe del cas autoritzat
- execució en directe del cas denegat
- pregunta oral sobre què es comprova abans de permetre l’acció

**Pes orientatiu dins del repte**

25%

### Microprojecte MP6 — Prova, depuració, documentació i preparació del Repte 3

**Tipus**

Microprojecte de tancament i verificació.

**Objectiu**

Consolidar el repte amb proves mínimes, depuració documentada i una lectura clara del que haurà de passar a reorganització arquitectònica en el Repte 3.

**Tasca**

L’equip ha de:

- provar casos correctes i incorrectes
- registrar errors o incidències trobades
- documentar instruccions mínimes de prova
- actualitzar `README` o documentació equivalent
- identificar punts de deute tècnic que passaran al Repte 3

**Relació amb el producte principal**

Sense esta capa final, el repte pot funcionar en demo, però no queda prou verificat ni deixa clara la transició cap a una arquitectura més neta i mantenible.

**CA coberts**

- `RA4.f`

**Descripció dels CA en llenguatge docent**

- L’alumnat no només implementa: també prova, depura i documenta.
- L’alumnat sap distingir entre funcionalitat resolta i arquitectura encara provisional.
- L’alumnat deixa preparada la continuïtat cap al Repte 3.

**Paper de la IA**

La IA pot ajudar a generar casos de prova o a redactar text tècnic, però l’equip ha de verificar que la documentació i les proves coincidixen amb el comportament real.

**Evidències obligatòries**

- registre de proves mínimes
- casos positius i negatius
- incidències detectades i correccions
- documentació tècnica actualitzada
- llista de punts a reorganitzar al Repte 3
- defensa tècnica breu

**Instrument d’avaluació**

Checklist de verificació + defensa tècnica breu.

**Indicadors d’assoliment**

- proves mínimes reals
- errors documentats i tractats
- coherència entre documentació i demo
- transició al Repte 3 identificada amb claredat

**Riscos habituals**

- proves inventades
- documentació embellida però no executable
- no saber explicar què passarà a capes, servicis o persistència

**Verificació del treball real**

- execució dels casos documentats
- contrast entre documentació, repositori i demo
- pregunta oral sobre què s’haurà de reorganitzar en el Repte 3

**Pes orientatiu dins del repte**

15%

---

## 6. Taula resum de microprojectes i criteris d’avaluació

| Microprojecte | Tipus | Producte o lliurable | CA coberts | Evidències principals | Instrument | Pes orientatiu |
|---|---|---|---|---|---|---|
| MP1 | Procedimental | Formulari base i recuperació de dades | RA3.e, RA3.f, RA3.g | formulari, dades recuperades, primer enviament | Checklist | 10% |
| MP2 | Procedimental | Processament bàsic de la petició i resposta | RA2.c, RA2.d, RA2.e, RA2.f, RA2.g, RA2.h | cas correcte, cas incorrecte, validació, errors | Rúbrica + checklist | 20% |
| MP3 | Procedimental | Decisions, arrays i funcions aplicades al flux | RA3.a, RA3.b, RA3.c, RA3.d | lògica aplicada, arrays, funcions, explicació | Revisió + rúbrica | 15% |
| MP4 | Procedimental | Estat, sessió i/o cookies | RA4.a, RA4.b, RA4.c | estat observable, lectura, canvi o invalidació | Checklist | 15% |
| MP5 | Procedimental | Autenticació i primera operació protegida | RA4.d, RA4.e | login, logout, cas autoritzat, cas denegat | Rúbrica | 25% |
| MP6 | Tancament / verificació | Proves, depuració, documentació i pas a R3 | RA4.f | registre de proves, incidències, documentació, defensa | Checklist + defensa | 15% |

---

## 7. Evidències globals del repte

**Evidències mínimes comunes**

- issue principal amb microtasques
- seqüència de commits significativa
- formulari base operatiu
- recuperació de dades en servidor
- processament bàsic amb validació mínima
- ús de decisions, arrays i funcions dins del flux
- estat, sessió o mecanisme equivalent comprovable
- login i logout o mecanisme equivalent funcional
- almenys una operació real del domini protegida
- casos positius i negatius registrats
- documentació tècnica actualitzada
- AI log quan hi haja ús d’IA

**Evidències opcionals d’ampliació**

- més d’un formulari o cas d’ús coherent
- més d’una operació protegida
- casos de prova extra
- millor tractament de missatges d’error
- test automatitzat mínim
- anàlisi més fina del deute tècnic

---

## 8. Instruments d’avaluació del repte

### 8.1 Instruments principals

- rúbrica base de reptes adaptada al pes de `RA2`, `RA3` i `RA4`
- rúbrica específica de funcionalitat protegida
- checklist de formulari, petició i validació
- checklist d’estat, sessió o equivalent
- revisió de repositori
- defensa tècnica breu

### 8.2 Instruments de verificació

- execució en directe del formulari i de la recuperació de dades
- comprovació de casos correctes i incorrectes
- revisió de lògica amb decisions, arrays i funcions
- comprovació d’estat abans i després del canvi o logout
- demostració del cas autoritzat i del cas denegat
- contrast entre AI log, commits i resultat observat
- preguntes tècniques breus

---

## 9. Riscos del repte

| Risc | Com es manifesta | Impacte | Mesura de control |
|---|---|---|---|
| Saltar massa prompte a autenticació | Hi ha login però no hi ha base funcional prèvia | Alt | Exigir MP1-MP4 abans de donar valor a MP5 |
| Formulari ornamental | El formulari existix però no recupera ni tracta dades reals | Alt | Execució en directe i revisió del flux |
| Validació aparent | Només funciona el cas feliç | Alt | Casos negatius obligatoris |
| Confusió entre estat i autenticació | Es guarda context però no se sap què significa | Alt | Preguntes tècniques i comprovació abans/després |
| Delegació excessiva en IA | Codi o flux no compresos | Alt | Defensa, canvi en viu i contrast amb AI log |
| Funcionalitat protegida decorativa | Hi ha login/logout però no hi ha producte real protegit | Alt | Exigir cas d’ús funcional amb valor de domini |

---

## 10. Mesures de control i verificació

**Per comprovar aprenentatge real**

- execució real del formulari i de la recuperació de dades
- comprovació del processament bàsic en servidor
- explicació de la lògica amb decisions, arrays i funcions
- demostració d’estat o sessió observable
- execució real de login i logout o equivalent
- demo de cas autoritzat i cas denegat
- revisió de commits i issues
- contrast entre validacions definides i errors retornats
- pregunta de transferència
- revisió dels punts que passen al Repte 3

**Per distingir nivells d’autonomia**

- **treball autònom real**: l’alumne explica, adapta, prova i defensa
- **treball assistit per IA**: l’alumne usa suport, però valida i pren decisions
- **treball excessivament delegat**: l’alumne no comprén, no manté i no pot corregir

---

## 11. Adaptació realista a l’aula

**Duració orientativa**

6 a 8 sessions, segons l’stack triat i el grau de maduresa del repositori heretat del Repte 1.

**Moment del curs**

Després del Repte 1 i abans del Repte 3.

**Prerequisits**

- repositori funcional del Repte 1
- `README` operatiu
- primera base backend executable
- criteri mínim de treball amb issues i commits

**Possibles variants tecnològiques**

Es pot implementar amb l’stack adoptat per al curs, sempre que permeta:

- formularis o peticions equivalents
- tractament de dades en servidor
- validació bàsica
- estat, sessió o mecanisme equivalent
- autenticació i control d’accés
- documentació i prova funcional

**Part comuna del grup**

- formulari base
- processament bàsic de la petició
- lògica amb decisions, arrays i funcions
- estat o sessió comprovable
- autenticació funcional
- almenys una operació protegida
- proves mínimes
- documentació i defensa

**Ampliacions realistes**

- més d’un formulari útil
- més d’una operació protegida
- millor tractament d’errors
- casos límit addicionals
- test automatitzat mínim
- més preparació arquitectònica de cara al Repte 3

**Recuperació o reforç per CA**

- si fallen `RA3.e`, `RA3.f` o `RA3.g`: reconstrucció del formulari i de la recuperació de dades
- si fallen `RA2.c` a `RA2.h`: reimplementació del tractament de petició, validació i resposta
- si fallen `RA3.a` a `RA3.d`: reorganització del flux amb decisions, arrays i funcions
- si fallen `RA4.a` a `RA4.c`: revisió d’estat, sessió o cookies
- si fallen `RA4.d` o `RA4.e`: reconstrucció del flux autenticat i del cas protegit
- si falla `RA4.f`: nova ronda de proves, documentació i defensa

---

## 12. Tancament del repte

**Pregunta de síntesi per a l’alumnat**

Quin recorregut funcional complet hem aconseguit construir des del formulari fins a l’operació protegida, què demostra que és real i verificable, i què haurà de reorganitzar-se en el Repte 3?

**Criteri de superació del repte**

El repte es considera superat quan:

- existix un formulari base útil i les dades es recuperen realment en servidor
- la petició es processa amb validació i resposta mínima coherent
- el flux usa decisions, arrays i funcions amb sentit
- existix estat, sessió o mecanisme equivalent observable
- hi ha login i logout o equivalent funcional
- almenys una operació del producte queda protegida i és real
- existixen casos positius i negatius comprovables
- el repositori aporta evidències autèntiques de treball
- l’ús d’IA, si n’hi ha, queda registrat i validat
- el resultat deixa preparada la transició al Repte 3 sense haver de reconstruir la funcionalitat des de zero

**Observacions docents**

Este repte s’ha de llegir com a desplegament complet de `SA2` dins del producte evolutiu. No anticipa `RA5` com a resultat principal. La reorganització arquitectònica profunda queda reservada per al Repte 3, però només té sentit si en este punt ja existix un flux funcional real que va més enllà de login i logout.
