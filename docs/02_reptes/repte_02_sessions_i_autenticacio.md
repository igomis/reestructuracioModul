# Repte 2. Processament bàsic, estat, autenticació i primera funcionalitat protegida

## 1. Visió general del repte

**Finalitat del repte**

Construir la primera funcionalitat de negoci real del projecte a partir d’una progressió completa: recepció de dades, processament en servidor, ús de lògica bàsica, manteniment d’estat, autenticació i protecció d’una operació del domini.

Este repte no s’entén com un bloc reduït a registre, login i logout. El seu sentit és més ampli: consolidar els fonaments tècnics bàsics del treball en entorn servidor i fer-los desembocar en una funcionalitat autenticada amb valor real dins del producte del curs.

Este repte es resol sobre una **base comuna en `PHP`** per a tot l’alumnat. El contrast de frameworks no entra ací com a norma general.

**Producte principal del repte**

Una primera funcionalitat de domini protegida, construïda sobre una seqüència progressiva que inclou:

- formulari funcional o entrada equivalent de dades
- validació visible, errors interpretables i possibilitat de correcció
- recuperació i tractament de dades en servidor
- conservació funcional de la informació correcta perquè es puga reutilitzar
- ús de decisions, estructures de dades i funcions
- tractament bàsic d’imatge o fitxer quan tinga sentit dins del flux
- gestió bàsica d’estat
- mecanisme d’autenticació
- operació de domini restringida
- validació i tractament d’errors
- proves mínimes o verificacions registrades
- documentació tècnica actualitzada

**Context professional simul·lat o realista**

Després del kickoff inicial del projecte, l’equip necessita deixar arrere la simple posada en marxa del backend i començar a construir comportament real del sistema. Açò implica rebre dades, processar-les correctament, mostrar errors útils, conservar la informació que té valor funcional, mantindre informació d’estat quan cal, gestionar usuaris i assegurar que una primera operació del domini només es pot executar en les condicions adequades.

Per això, en este punt del curs es manté una base més controlada i comuna. El contrast fort de `Laravel`, `Symfony` o `NestJS` s’obri després, quan el flux ja està consolidat.

**Relació amb el projecte global del curs**

Este repte reutilitza la base tècnica creada en el Repte 1 i la transforma en una primera peça funcional realment usable. A més, prepara el pas al Repte 3, on la funcionalitat construïda ací s’haurà de reorganitzar, mantindre i professionalitzar millor.

El canvi metodològic del curs es concreta així:

- `R2` és base comuna en `PHP`
- `R3` és el punt d’entrada del contrast de frameworks
- el mateix projecte continua després amb itineraris diferents

---

## 2. Relació amb resultats d’aprenentatge

**Resultats d’aprenentatge principals**

- **RA2**: desenvolupament de blocs bàsics de codi en entorn servidor, amb mecanismes de generació de pàgines o respostes amb codi embegut, tecnologies associades, inclusió de codi, sintaxi, variables, operadors, directives i processament elemental
- **RA3**: construcció de fluxos amb decisions, repeticions, arrays, funcions i interacció amb formularis
- **RA4**: manteniment d’estat, autenticació d’usuaris, control d’accés i ús d’eines de prova i depuració

**Justificació curricular**

Este repte no ha de començar directament per l’autenticació com si fora un bloc aïllat. Perquè siga curricularment sòlid, ha de recórrer abans els elements bàsics de processament de dades en servidor i de programació necessaris per a entendre què es rep, què es valida, què es conserva de manera funcional, què es protegix i per què.

---

## 3. Canvi metodològic que introdueix la IA

**Paper de la IA en este repte**

La IA es pot usar per a:

- generar esquelets inicials de formularis i processament
- suggerir validacions
- proposar exemples de decisions, arrays i funcions
- ajudar a interpretar errors
- generar casos de prova positius i negatius
- ajudar a redactar documentació tècnica i registre d’incidències

**Què no es delega**

L’alumnat ha de:

- entendre què fa cada part del flux
- saber d’on ix cada dada i on es tracta
- justificar la necessitat de cada decisió o funció
- distingir entre estat, autenticació i autorització
- provar i defensar el comportament real del sistema

**Risc principal d’ús inadequat de la IA**

Construir un flux aparentment funcional però sense comprensió real del tractament de dades, de la lògica bàsica, del manteniment d’estat o de la restricció de l’operació protegida.

**Mesures de control**

- AI log quan corresponga
- revisió de commits i issues
- execució en directe
- casos positius i negatius obligatoris
- preguntes de transferència
- microcanvis en viu
- contrast entre documentació, codi i comportament observat

---

## 4. Estructura del repte

### 4.1 Nucli del repte

**Objectiu del nucli**

Construir una primera funcionalitat de negoci real que recórrega de manera coherent el camí complet des de l’entrada de dades fins a una acció protegida per autenticació o restricció funcional.

**Lliurable principal**

Mòdul funcional integrat en el projecte que incloga:

- formulari o entrada de dades equivalent
- visualització d’errors de validació i possibilitat de correcció
- recuperació de dades en servidor
- lògica bàsica amb decisions, arrays o funcions
- conservació funcional simple de la informació correcta
- estat o sessió quan siga necessari
- tractament d’imatge o fitxer quan tinga sentit dins del cas d’ús
- alta o identificació d’usuari
- autenticació
- una operació de domini protegida
- tractament d’errors
- proves mínimes o verificacions registrades
- documentació tècnica actualitzada

**Criteris d’avaluació principals del nucli**

- CA de **RA2** vinculats a inclusió de codi, sintaxi, variables, operadors, directives i àmbits
- CA de **RA3** vinculats a decisions, bucles, arrays, funcions, formularis i recuperació de dades
- CA de **RA4** vinculats a estat, mecanismes d’autenticació, control d’accés i prova/depuració

**Evidències obligatòries del nucli**

- repositori actualitzat
- issue principal del repte i microtasques
- seqüència de commits significativa
- formulari funcional o equivalent
- evidència de processament correcte i incorrecte
- evidència de validació visible i correcció del flux
- ús visible de lògica bàsica
- evidència de conservació funcional o reutilització de la informació correcta
- evidència d’estat, sessió o cookies
- flux d’autenticació funcional
- operació de domini protegida
- proves mínimes
- documentació tècnica
- AI log quan hi haja ús d’IA

### 4.2 Límit metodològic sobre persistència

En este repte, la informació correcta del formulari o de l’entrada equivalent ha de poder continuar viva dins del projecte.

Això pot significar:

- recuperar un usuari o un element creat
- tornar a mostrar un producte, una reserva o un recurs
- llistar dades que ja formen part del flux funcional

Ara bé, esta conservació no convertix encara `R2` en un repte centrat en accés a dades o arquitectura de persistència.

El que importa ací és:

- tractament de dades
- lògica bàsica
- estat o sessió
- autenticació
- funcionalitat protegida

La conservació es pot resoldre amb mecanismes simples i controlats. La base de dades pot aparéixer si el projecte o el professorat ho demanen, però en este punt no és el focus principal del repte. Eixa professionalització metodològica i arquitectònica guanya pes en `R3`.

---

## 5. Microprojectes i microtasques del repte

> **Norma del repte**
>
> - Els microprojectes cobrixen la progressió real de `SA2` i no només el tram final d’autenticació.
> - Les microtasques d’investigació o decisió cobrixen sobretot criteris conceptuals o de modelització.
> - Cap microprojecte apareix sense el camp **“CA coberts”**.
> - El repte no es considera suficient si només hi ha login/logout sense un recorregut previ de processament i sense una operació real protegida.
> - El pas al Repte 3 només té sentit si el flux actual ja funciona de manera reproduïble i mínimament explicable.
> - El contrast de frameworks encara no és el centre del repte.

### Microprojecte MP1 — Formulari base, validació visible i recuperació de dades

**Tipus**

Microprojecte procedimental.

**Objectiu**

Construir un punt d’entrada de dades usable i demostrar que el sistema és capaç de recuperar la informació aportada per l’usuari, validar-la i mostrar errors interpretables.

**Tasca**

L’equip crea un formulari funcional, o una entrada equivalent coherent amb la base comuna en `PHP`, i implementa la recuperació de les dades enviades per l’usuari.

S’ha de veure amb claredat:

- quins camps es reben
- com es recuperen
- com es mostren els errors quan alguna dada no és vàlida
- quin tractament inicial se’ls dona
- quina resposta bàsica retorna el sistema
- quins comentaris breus ajuden a entendre el flux quan el codi ho necessita

**Relació amb el producte principal**

És el primer pas del flux real de la funcionalitat. Sense esta capa, la resta del repte queda desconnectada de l’entrada d’informació.

**CA coberts**

- **RA3.e**
- **RA3.f**
- **RA3.g**

**Descripció dels CA en llenguatge docent**

- L’alumnat usa formularis o mecanismes equivalents per interactuar amb l’usuari.
- L’alumnat recupera correctament les dades introduïdes.
- L’alumnat documenta el codi amb comentaris útils i claredat mínima.

**Paper de la IA**

La IA pot suggerir l’estructura inicial del formulari o exemples de tractament bàsic, però l’alumnat ha de comprovar que la recuperació de dades és real i que entén el flux.

**Evidències obligatòries**

- formulari funcional o entrada equivalent
- recuperació correcta de dades
- error de validació visible i possibilitat de reintent
- captura o demo del cas correcte
- codi comentat mínimament
- commits associats

**Instrument d’avaluació**

Checklist de formulari i recuperació de dades.

**Indicadors d’assoliment**

- les dades es reben realment
- el codi és comprensible
- hi ha correspondència entre camps, recuperació i resposta

**Riscos habituals**

- formulari només decoratiu
- recuperació aparent però no verificable
- comentaris inexistents o inútils

**Verificació del treball real**

- execució en directe del formulari
- pregunta oral sobre d’on ix cada dada i com arriba al servidor

**Pes orientatiu dins del repte**

15%

---

### Microprojecte MP2 — Processament bàsic de la petició i conservació funcional simple

**Tipus**

Microprojecte procedimental.

**Objectiu**

Fer visible el treball elemental de programació en servidor que permet processar les dades rebudes, modificar el comportament del sistema i deixar la informació correcta en un estat reutilitzable.

**Tasca**

L’equip implementa tractament bàsic de la petició, incloent:

- mecanisme bàsic de generació de pàgina o resposta amb codi embegut o equivalent sobre la base comuna en `PHP`
- identificació de les tecnologies mínimes associades al flux: servidor, fitxer o plantilla, petició i resposta
- inclusió de codi en el llenguatge de marques o equivalent
- ús correcte de sintaxi
- sentències simples
- directives o configuracions bàsiques
- variables
- operadors
- àmbits de variables quan siga rellevant

**Relació amb el producte principal**

Este microprojecte dona la base de processament necessari perquè després el sistema puga prendre decisions, validar i actuar sobre l’estat de l’usuari.
També ha de deixar clar com la informació correcta es conserva de manera funcional sense convertir encara el repte en un exercici centrat en accés a dades.

**CA coberts**

- **RA2.a**
- **RA2.b**
- **RA2.c**
- **RA2.d**
- **RA2.e**
- **RA2.f**
- **RA2.g**
- **RA2.h**

**Descripció dels CA en llenguatge docent**

- L’alumnat entén el mecanisme bàsic de generació de pàgines o respostes amb codi embegut.
- L’alumnat identifica les tecnologies associades mínimes del flux sobre la base comuna en `PHP`.
- L’alumnat integra codi de servidor dins del context de l’aplicació.
- L’alumnat usa sintaxi i sentències amb correcció.
- L’alumnat treballa amb variables, operadors i directives de manera funcional.
- L’alumnat sap explicar on és visible cada variable i per què.

**Paper de la IA**

La IA pot proposar fragments inicials, però l’alumnat ha de depurar-los, adaptar-los i explicar-los.

**Evidències obligatòries**

- tram recognoscible de codi embegut o equivalent
- codi executable de processament
- evidència de variables i operadors en ús
- comportament modificat per alguna directiva o configuració bàsica
- demo de processament correcte
- demo d’una conservació funcional simple o reutilització posterior
- commits i issue relacionades

**Instrument d’avaluació**

Rúbrica breu de processament bàsic en servidor.

**Indicadors d’assoliment**

- el tractament és executable
- el codi no és merament copiat
- hi ha correspondència entre dades rebudes i resposta generada

**Riscos habituals**

- fragments inconnexos
- variables sense sentit funcional
- tractament superficial només per complir

**Verificació del treball real**

- pregunta oral sobre com es genera la pàgina o resposta i quines peces tècniques hi intervenen
- pregunta oral sobre variables i àmbits
- canvi menut en viu sobre una operació o una directiva

**Pes orientatiu dins del repte**

15%

---

### Microprojecte MP3 — Decisions, arrays i funcions aplicades al flux

**Tipus**

Microprojecte procedimental.

**Objectiu**

Aplicar lògica bàsica de programació per controlar el comportament del sistema a partir de les dades rebudes.

**Tasca**

L’equip amplia el flux amb:

- almenys una decisió significativa
- ús d’una estructura iterativa quan siga pertinent
- ús d’un array o estructura equivalent
- una o més funcions per encapsular comportament

No es tracta d’afegir estos elements de manera artificial, sinó d’utilitzar-los per donar forma al comportament del flux.

**Relació amb el producte principal**

Este microprojecte convertix el tractament bàsic en una lògica més rica i més pròxima a una funcionalitat real.

**CA coberts**

- **RA3.a**
- **RA3.b**
- **RA3.c**
- **RA3.d**

**Descripció dels CA en llenguatge docent**

- L’alumnat sap decidir què fa el sistema segons la informació rebuda.
- L’alumnat utilitza estructures bàsiques per organitzar el comportament.
- L’alumnat encapsula operacions en funcions amb sentit.

**Paper de la IA**

La IA pot suggerir exemples de decisions o funcions, però l’alumnat ha de justificar per què són necessàries dins del flux del repte.

**Evidències obligatòries**

- cas de decisió observable
- array o estructura equivalent usada amb sentit
- funció o funcions útils
- demo del comportament resultant
- explicació breu de la lògica aplicada

**Instrument d’avaluació**

Rúbrica de lògica bàsica aplicada.

**Indicadors d’assoliment**

- les estructures usades tenen sentit
- la funció no és ornamental
- el comportament resultant és observable

**Riscos habituals**

- afegir arrays o funcions només per cobrir criteris
- lògica confusa o no connectada al producte

**Verificació del treball real**

- pregunta oral sobre per què la decisió, l’array o la funció són necessaris
- microcanvi en viu sobre una condició o una funció

**Pes orientatiu dins del repte**

15%

---

### Microprojecte MP4 — Estat, sessió i/o cookies

**Tipus**

Microprojecte procedimental.

**Objectiu**

Fer visible que el sistema pot conservar informació rellevant entre interaccions i diferenciar el comportament segons l’estat de l’usuari o del client, sense confondre això amb la conservació funcional de dades del domini.

**Tasca**

L’equip implementa una evidència bàsica de manteniment d’estat, per exemple amb:

- sessió
- cookies
- o mecanisme equivalent coherent amb la base comuna en `PHP`

S’ha de veure:

- quina informació es conserva
- per a què es conserva
- quan es recupera
- quan deixa de ser vàlida o es neteja
- si hi ha informació guardada en client, com es recupera
- quina diferència hi ha entre estat de sessió i informació del projecte que després s’ha de reutilitzar

**Relació amb el producte principal**

Sense estat no hi ha base sòlida per entendre després l’autenticació ni per protegir una operació de domini.

**CA coberts**

- **RA4.a**
- **RA4.b**
- **RA4.c**

**Descripció dels CA en llenguatge docent**

- L’alumnat identifica els mecanismes disponibles per mantindre informació d’un client concret.
- L’alumnat usa un mecanisme real d’estat.
- L’alumnat sap guardar i recuperar informació del client quan toca, i distingir-la del que es manté al servidor.

**Paper de la IA**

La IA pot ajudar a recordar sintaxi o patrons, però l’alumnat ha d’explicar exactament què es guarda i amb quina finalitat.

**Evidències obligatòries**

- mecanisme d’estat implementat
- demostració de recuperació de la informació
- si hi ha cookies o emmagatzematge en client, demostració de lectura i recuperació
- demostració de neteja o invalidació quan siga necessari
- explicació clara de la frontera entre estat i conservació funcional
- captura o demo del comportament

**Instrument d’avaluació**

Checklist de manteniment d’estat.

**Indicadors d’assoliment**

- hi ha informació realment mantinguda
- el comportament canvia segons l’estat
- l’equip sap explicar diferència entre sessió i altres mecanismes

**Riscos habituals**

- confondre estat amb autenticació
- guardar informació sense necessitat
- no poder demostrar recuperació real

**Verificació del treball real**

- execució en directe del canvi d’estat
- pregunta oral sobre què es guarda, on i per què

**Pes orientatiu dins del repte**

15%

---

### Microprojecte MP5 — Autenticació i primera operació protegida

**Tipus**

Microprojecte procedimental.

**Objectiu**

Connectar el flux tècnic anterior amb una primera necessitat real del producte: una operació que només es pot executar si l’usuari compleix una condició d’accés.

**Tasca**

L’equip implementa:

- alta o identificació d’usuari
- autenticació funcional
- comprovació d’usuari autenticat
- una operació real del domini protegida
- una restricció observable de rol, permís o regla de negoci

La funcionalitat protegida ha de tindre valor real dins del producte del curs i treballar amb informació que després continue sent útil dins del mateix projecte.

**Relació amb el producte principal**

Este és el centre visible del repte: demostrar que el backend ja no sols rep i processa dades, sinó que gestiona identitat i protegix accions amb sentit.

**CA coberts**

- **RA4.d**
- **RA4.e**

**Descripció dels CA en llenguatge docent**

- L’alumnat identifica mecanismes d’autenticació.
- L’alumnat implementa autenticació funcional.
- L’alumnat restringix una acció del sistema de manera real i verificable.

**Paper de la IA**

La IA pot suggerir esquelets o fluxos d’accés, però l’alumnat ha de validar-los i demostrar-los.

**Evidències obligatòries**

- registre o identificació funcional
- login funcional
- comprovació d’usuari autenticat
- operació protegida
- dada o conjunt de dades reutilitzables dins del flux protegit
- cas autoritzat
- cas denegat
- evidència de la restricció aplicada
- commits associats

**Instrument d’avaluació**

Rúbrica de funcionalitat autenticada i protegida.

**Indicadors d’assoliment**

- el login no és decoratiu
- hi ha una operació real protegida
- la restricció és observable
- el comportament és coherent en cas positiu i negatiu

**Riscos habituals**

- autenticació superficial
- funcionalitat de domini ornamental
- restricció no demostrable

**Verificació del treball real**

- execució en directe del cas autoritzat
- execució en directe del cas denegat
- pregunta oral sobre en quin punt es bloqueja l’acció

**Pes orientatiu dins del repte**

25%

---

### Microprojecte MP6 — Prova, depuració, documentació i preparació del Repte 3

**Tipus**

Microprojecte de tancament i verificació.

**Objectiu**

Comprovar que el flux complet funciona, que els errors són observables i que l’equip sap explicar què caldrà reorganitzar o millorar en el repte següent.

**Tasca**

L’equip:

- revisa casos positius i negatius
- prova validacions i errors
- comprova que la informació correcta es pot recuperar o reutilitzar
- usa alguna eina o entorn simple de prova i depuració
- documenta instruccions de prova
- registra incidències detectades
- actualitza la documentació tècnica
- identifica punts de deute tècnic o necessitat de reorganització per al Repte 3

**Relació amb el producte principal**

Sense esta capa, el repte podria funcionar aparentment, però no quedaria prou verificat ni orientat al pas següent.

**CA coberts**

- **RA4.f**

**Descripció dels CA en llenguatge docent**

- L’alumnat usa eines, tècniques o entorns per provar i depurar.
- L’alumnat comprova i documenta el comportament real del sistema.

**Paper de la IA**

La IA pot ajudar a generar casos de prova o text documental, però l’alumnat ha de verificar que el que documenta és real.

**Evidències obligatòries**

- registre de proves mínimes
- casos positius i negatius
- incidències detectades
- rastre de l’eina o entorn utilitzat per provar o depurar
- evidència breu de reutilització de dades
- documentació tècnica actualitzada
- llista de millores o refactoritzacions futures
- defensa tècnica breu

**Instrument d’avaluació**

Checklist de verificació + defensa tècnica.

**Indicadors d’assoliment**

- les proves són reals
- la documentació correspon al comportament observat
- l’equip sap explicar què caldrà millorar en el Repte 3

**Riscos habituals**

- proves fictícies
- documentació embellida
- no saber justificar el pas següent del projecte

**Verificació del treball real**

- execució dels casos documentats
- contrast entre documentació, repositori i demo
- pregunta oral sobre què caldria reorganitzar en el Repte 3

**Pes orientatiu dins del repte**

15%

---

## 6. Taula resum de microprojectes i criteris d’avaluació

| Microprojecte | Tipus | Producte o lliurable | CA coberts | Evidències principals | Instrument | Pes orientatiu |
|---|---|---|---|---|---|---|
| MP1 | Procedimental | Formulari base i recuperació de dades | RA3.e, RA3.f, RA3.g | formulari, recuperació, demo, comentaris | checklist | 15% |
| MP2 | Procedimental | Processament bàsic de la petició | RA2.a, RA2.b, RA2.c, RA2.d, RA2.e, RA2.f, RA2.g, RA2.h | codi executable, codi embegut, variables, directiva, demo | rúbrica breu | 15% |
| MP3 | Procedimental | Decisions, arrays i funcions aplicades | RA3.a, RA3.b, RA3.c, RA3.d | lògica observable, funcions, demo | rúbrica | 15% |
| MP4 | Procedimental | Estat, sessió i/o cookies | RA4.a, RA4.b, RA4.c | demo d’estat, recuperació i invalidació | checklist | 15% |
| MP5 | Procedimental | Autenticació i operació protegida | RA4.d, RA4.e | login, operació protegida, cas autoritzat i denegat | rúbrica | 25% |
| MP6 | Tancament / verificació | Proves, documentació i preparació del Repte 3 | RA4.f | proves, incidències, documentació, defensa | checklist + defensa | 15% |

---

## 7. Evidències globals del repte

**Evidències mínimes comunes**

- issue principal amb microtasques
- seqüència de commits significativa
- formulari funcional o entrada equivalent
- recuperació real de dades
- processament bàsic en servidor
- ús visible de lògica amb decisions, arrays o funcions
- evidència d’estat, sessió o cookies
- autenticació funcional
- operació real protegida
- cas positiu i cas negatiu
- registre de proves mínimes
- documentació tècnica actualitzada
- AI log quan hi haja ús d’IA

**Evidències opcionals d’ampliació**

- més d’una operació protegida
- millora dels missatges d’error
- rols addicionals
- test automatitzat mínim
- millor observabilitat del flux
- preparació més detallada del Repte 3

### 7.1 Forma mínima de prova del repte

En `R2` no és suficient afirmar que el flux funciona. Cal deixar una prova visible i verificable del comportament real del sistema.

La prova mínima hauria d’incloure, com a mínim:

- enviament correcte del formulari o entrada equivalent
- error de validació visible
- correcció d’una entrada inicialment incorrecta
- tractament correcte de la informació en servidor
- conservació funcional o reutilització posterior de la informació correcta
- cas autoritzat de la funcionalitat protegida
- cas denegat de la funcionalitat protegida
- tractament d’imatge o fitxer, si forma part del flux

### 7.2 Presentació de proves

Les proves es poden registrar de manera simple, però han de ser clares i reutilitzables en revisió docent.

Formats recomanables:

- checklist de verificació
- taula curta de casos de prova
- col·lecció de peticions o registre equivalent

Si s’opta per una taula curta, convé incloure camps com:

- cas de prova
- entrada
- resultat esperat
- resultat obtingut
- incidències detectades

### 7.3 Documentació del codi i PHPDoc

En este repte, la documentació del codi ha de ser útil i proporcionada.

No es tracta d’omplir el projecte de text, sinó de fer visible:

- què fa cada part important del flux
- on es valida la informació
- on es tracta l’autenticació o la comprovació d’accés
- on es processa la imatge o el fitxer, si n’hi ha
- com es conserva després la informació

Es recomana l’ús selectiu de `PHPDoc` en funcions pròpies amb lògica rellevant, sobretot en validació, tractament de dades, tractament de fitxers, comprovació d’accés o funcions reutilitzables no evidents.

Si s’utilitza, hauria d’aportar comprensió real del codi, per exemple amb:

- descripció breu
- `@param`
- `@return`
- `@throws`, quan realment aplique

No es demana:

- documentar cada variable
- omplir de DocBlocks fitxers trivials
- generar documentació automàtica completa
- afegir documentació decorativa sense utilitat funcional

---

## 8. Instruments d’avaluació del repte

### 8.1 Instruments principals

- rúbrica base del repte
- rúbriques específiques de microprojecte
- checklists de formulari, estat i verificació
- revisió de repositori
- defensa tècnica breu

### 8.2 Instruments de verificació

- execució en directe del flux
- casos positius i negatius
- revisió de commits i issues
- preguntes tècniques breus
- microcanvis en viu
- contrast entre documentació, AI log i comportament observat

---

## 9. Riscos d’ús inadequat de la IA

| Risc | Com es manifesta | Impacte | Mesura de control |
|---|---|---|---|
| Delegació excessiva | flux aparentment funcional però no comprés | Alt | defensa i preguntes tècniques |
| Validació superficial | el cas feliç funciona però els errors no | Alt | casos negatius obligatoris |
| Confusió conceptual | barreja entre estat, sessió, autenticació i autorització | Alt | execució guiada i preguntes de contrast |
| Proves fictícies | documentació sense correspondència amb el sistema | Alt | execució real |
| Funcionalitat ornamental | hi ha login però no hi ha valor real protegit | Alt | exigir operació de domini observable |

---

## 10. Mesures de control i verificació

**Per comprovar aprenentatge real**

- execució real del formulari i la recuperació de dades
- demostració del processament en servidor
- comprovació de la lògica bàsica aplicada
- demostració d’estat, sessió o cookies
- execució real de l’autenticació
- demo de cas autoritzat i denegat
- revisió de commits i issues
- contrast entre proves descrites i comportament real
- pregunta de transferència
- canvi tècnic menut en directe

**Per distingir nivells d’autonomia**

- **treball autònom real**: l’alumne explica, adapta, prova i defensa
- **treball assistit per IA**: l’alumne usa suport, però valida i pren decisions
- **treball excessivament delegat**: l’alumne no comprén, no transferix i no pot corregir

---

## 11. Adaptació realista a l’aula

**Duració orientativa**

6 a 8 sessions, segons el nivell del grup i la solidesa de la base comuna en `PHP`.

**Moment del curs**

Després del Repte 1 i abans del Repte 3.

**Prerequisits**

- repositori funcional del Repte 1
- base backend executable
- README operatiu
- treball mínim amb Git, issues i commits

**Possibles variants tecnològiques**

Es pot implementar sobre la base comuna en `PHP` fixada pel curs o pel departament, sempre que permeta:

- tractament d’entrada de dades
- processament en servidor
- ús de lògica bàsica
- manteniment d’estat
- autenticació
- protecció d’operacions
- documentació i verificació funcional

**Part comuna del grup**

- formulari o entrada equivalent
- processament bàsic
- lògica mínima aplicada
- estat o sessió
- autenticació funcional
- una operació protegida
- proves mínimes
- documentació i defensa

**Ampliacions realistes**

- més d’una restricció
- més d’un rol
- més d’una operació protegida
- millor qualitat de validació
- proves automatitzades
- preparació més forta per al Repte 3

**Recuperació o reforç per CA**

- si fallen CA de **RA2**: reconstrucció del processament bàsic i explicació d’àmbits, variables i operadors
- si fallen CA de **RA3**: reconstrucció del formulari, recuperació de dades i lògica aplicada
- si fallen CA de **RA4**: reimplementació o correcció d’estat, autenticació i protecció d’operacions

---

## 12. Tancament del repte

**Pregunta de síntesi per a l’alumnat**

Com hem passat d’un simple punt d’entrada de dades a una funcionalitat de producte real protegida, i què necessitarem reorganitzar en el Repte 3?

**Criteri de superació del repte**

El repte es considera superat quan:

- existix un flux complet i verificable des de l’entrada de dades fins a una operació protegida
- el sistema recupera i processa informació en servidor
- s’utilitza lògica bàsica amb sentit
- hi ha evidència real de manteniment d’estat
- l’autenticació és funcional
- almenys una operació del domini queda protegida i es pot demostrar tant en cas autoritzat com en cas denegat
- les proves mínimes i la documentació són coherents amb el comportament observat
- l’alumnat pot defensar tècnicament allò construït

**Observacions docents**

Este repte s’ha de llegir com una progressió completa dins de SA2. Per tant, no s’hauria de reduir a un bloc d’autenticació. El seu valor està en connectar fonaments bàsics de programació en servidor amb una primera funcionalitat de producte realment protegida.
