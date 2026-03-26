# Repte 2. Sessions, autenticació i primera funcionalitat de negoci amb microprojectes i criteris d’avaluació explícits

## 1. Visió general del repte

**Finalitat del repte**  
Construir la primera funcionalitat de negoci real i autenticada del producte backend del curs. Este repte transforma la base tècnica del Repte 1 en un mòdul usable, verificable i connectat amb una necessitat professional recognoscible.

**Producte principal del repte**  
Una primera funcionalitat de domini real protegida per autenticació i control d’accés, amb:
- registre o alta d’usuari
- login i logout
- comprovació d’usuari autenticat o de sessió activa
- almenys una operació de negoci protegida
- una restricció de rol, permís o regla de negoci
- validació d’entrada del costat servidor
- tractament consistent d’errors
- proves mínimes o verificacions registrades
- documentació tècnica actualitzada

**Context professional simulat o realista**  
Després del kickoff, l’equip ja disposa d’un repositori funcional, però encara no pot gestionar identitat d’usuari ni protegir operacions reals del producte. En qualsevol backend professional, este és el primer llindar de credibilitat funcional: abans d’ampliar el domini o publicar APIs, cal demostrar que el sistema sap qui és l’usuari, què pot fer i com respon davant dades incorrectes.

**Relació amb el projecte global del curs**  
Este repte reutilitza la base creada en el Repte 1 i prepara explícitament el pas al Repte 3. No és una activitat aïllada: és la primera implementació real del model d’usuaris, del control d’accés i d’una funcionalitat de domini protegida dins del producte únic del curs.

---

## 2. Relació amb resultats d’aprenentatge

**Resultats d’aprenentatge principals**  
- **RA2**: desenvolupament de lògica de servidor per processar peticions, formularis, validacions i respostes amb control d’errors
- **RA3**: implementació de gestió d’estat, sessions i autenticació d’usuaris amb criteri funcional i control d’accés
- **RA4**: construcció de funcionalitat web dinàmica orientada a un cas d’ús real del producte

**Justificació curricular**  
El repte permet passar de la base tècnica inicial a una primera funcionalitat backend útil, amb identitat d’usuari, restriccions d’accés, tractament d’errors i connexió directa amb el domini del projecte. El document actual del repte ja fixa esta orientació i explicita que el valor no està en implementar autenticació aïllada, sinó en connectar-la amb una operació real del domini.

---

## 3. Canvi metodològic que introduïx la IA

**Paper de la IA en este repte**  
La IA es pot usar per a:
- proposar esquelets de fluxos de registre, login i control de sessió
- suggerir matrius de validació
- plantejar casos de prova positius i negatius
- ajudar a interpretar errors d’autenticació, validació o control d’accés
- revisar la claredat dels missatges d’error
- ajudar a documentar incidències i decisions

**Què no es delega**  
L’alumnat ha de:
- entendre què valida el sistema i on ho fa
- explicar què queda guardat en sessió o quin mecanisme d’identificació s’empra
- justificar per què una ruta o operació queda protegida
- provar els casos correctes i incorrectes
- demostrar que la funcionalitat de domini no és decorativa, sinó real i verificable

**Risc principal d’ús inadequat de la IA**  
Copiar fluxos d’autenticació sense entendre sessions, validació, autorització o errors, o bé donar per bo un login aparent sense control real sobre una operació de negoci.

**Mesures de control**  
- AI log quan corresponga
- revisió de commits i issues
- execució en directe de casos positius i negatius
- preguntes tècniques sobre sessió, autenticació i restricció
- modificació menuda en viu
- contrast entre documentació, codi i comportament observat

---

## 4. Nucli del repte

**Objectiu del nucli**  
Deixar operativa una primera funcionalitat de domini real protegida per autenticació, amb control d’accés suficient, validació del costat servidor i evidències verificables de comportament correcte i incorrecte.

**Lliurable principal**  
Mòdul funcional integrat en el producte backend del curs que incloga:
- alta o registre d’usuari
- login i logout
- comprovació d’usuari autenticat
- una operació de domini protegida
- una regla de rol, permís o restricció de negoci
- tractament d’errors coherent
- proves mínimes o registre de verificació
- documentació tècnica actualitzada

**Criteris d’avaluació principals del nucli**  
- CA de RA2 vinculats a tractament de peticions, validació, errors i processament
- CA de RA3 vinculats a sessions, autenticació, estat i control d’accés
- CA de RA4 vinculats a funcionalitat dinàmica real i comportament orientat al producte

**Evidències obligatòries del nucli**  
- repositori actualitzat
- issue principal del repte i microtasques
- seqüència de commits significativa
- demo funcional de registre, login, logout i cas d’ús protegit
- evidència d’una restricció real
- casos positius i negatius verificats
- documentació tècnica actualitzada
- AI log quan hi haja ús d’IA

---

## 5. Microprojectes i microtasques del repte

> **Norma del repte**
>
> - Els microprojectes cobrixen sobretot els criteris procedimentals.
> - Les microtasques d’investigació o decisió cobrixen sobretot els criteris de comprensió, modelització i justificació.
> - Cap microprojecte apareix sense el camp **“CA coberts”**.
> - Cap lliurable d’autenticació es considera suficient si no està connectat a una operació real del domini.

### Microprojecte MP1 — Disseny del flux d’accés i del cas d’ús protegit

**Tipus**  
Microtasca d’investigació i decisió tècnica.

**Objectiu**  
Definir com encaixa la identitat d’usuari dins del domini del producte i quina serà la primera operació real protegida per autenticació, rol o restricció.

**Tasca**  
L’equip concreta:
- el model mínim d’usuari
- el flux de registre, login i logout
- la comprovació d’usuari autenticat
- la primera operació de domini protegida
- la restricció de rol, permís o regla de negoci
- els casos correctes i incorrectes principals

**Relació amb el producte principal**  
Este microprojecte evita que l’autenticació quede desacoblada del producte i força a pensar-la com a infraestructura al servei d’un cas d’ús real.

**CA coberts**  
- **RA3**: criteris relacionats amb identificació d’usuaris, gestió d’estat, autenticació i control d’accés
- **RA4**: criteris relacionats amb la definició d’una funcionalitat dinàmica real dins del producte

**Descripció dels CA en llenguatge docent**  
- L’alumnat sap explicar qui és l’usuari del sistema i quina operació queda protegida.
- L’alumnat diferencia autenticació, autorització i regla de negoci.
- L’alumnat planteja un flux coherent amb el domini, no un exemple artificial.

**Paper de la IA**  
La IA pot ajudar a proposar fluxos, rols o restriccions, però l’equip ha de validar que encaixen amb el producte i amb el nivell del repte.

**Evidències obligatòries**  
- esquema del flux d’accés
- descripció del cas d’ús protegit
- matriu inicial de rols o restriccions
- llista de casos correctes i incorrectes
- defensa oral breu

**Instrument d’avaluació**  
Rúbrica de disseny funcional aplicat.

**Indicadors d’assoliment**  
- el flux és coherent i complet
- hi ha una operació real protegida
- la restricció triada té sentit
- el plantejament és executable i verificable

**Riscos habituals**  
- definir autenticació sense cas d’ús real
- confondre rol amb restricció de negoci
- proposar un flux massa gran o massa artificial

**Verificació del treball real**  
- pregunta oral: “quina operació quedaria mal protegida si no existira la restricció definida?”
- pregunta oral: “què comprova el sistema abans de permetre l’acció?”

**Pes orientatiu dins del repte**  
15%

### Microprojecte MP2 — Registre, login, logout i comprovació d’usuari autenticat

**Tipus**  
Microprojecte procedimental.

**Objectiu**  
Implementar el flux base d’identitat d’usuari perquè el sistema puga donar d’alta, autenticar, mantindre i tancar la sessió d’un usuari.

**Tasca**  
L’equip implementa:
- alta o registre d’usuari amb validacions bàsiques
- login
- logout
- comprovació d’usuari autenticat o de sessió activa
- resposta coherent davant credencials incorrectes o dades invàlides

**Relació amb el producte principal**  
Este microprojecte posa en marxa la infraestructura mínima perquè la funcionalitat de domini puga quedar protegida de manera real.

**CA coberts**  
- **RA2**: criteris de tractament de peticions, formularis, validació i control d’errors
- **RA3**: criteris de sessions, autenticació i manteniment d’estat

**Descripció dels CA en llenguatge docent**  
- L’alumnat sap processar dades d’entrada del costat servidor.
- L’alumnat valida i respon amb errors interpretables.
- L’alumnat implementa una autenticació funcional i verificable.
- L’alumnat sap demostrar quan un usuari està autenticat i quan deixa d’estar-ho.

**Paper de la IA**  
La IA pot suggerir esquelets de codi o matrius de validació, però l’alumnat ha de comprovar què es guarda, què es valida i què es retorna.

**Evidències obligatòries**  
- registre funcional
- login funcional
- logout funcional
- comprovació d’usuari autenticat
- casos vàlid i invàlid
- evidència d’errors controlats
- commits i issue relacionades

**Instrument d’avaluació**  
Rúbrica de microprojecte funcional + checklist de validació.

**Indicadors d’assoliment**  
- el flux base funciona de principi a fi
- hi ha validació real en servidor
- els errors són coherents i visibles
- el comportament és defensable tècnicament

**Riscos habituals**  
- validació aparent
- errors genèrics poc útils
- login funcional però sense comprovació consistent d’estat
- codi copiat sense entendre què fa

**Verificació del treball real**  
- execució en directe de registre correcte i incorrecte
- execució en directe de login correcte i incorrecte
- comprovació de l’estat abans i després del logout
- pregunta tècnica sobre el mecanisme triat per mantindre l’estat

**Pes orientatiu dins del repte**  
30%

### Microprojecte MP3 — Operació de domini protegida per autenticació i restricció

**Tipus**  
Microprojecte procedimental.

**Objectiu**  
Connectar el mòdul d’accés amb una primera necessitat real del producte: una operació de domini que només puga executar-se sota determinades condicions.

**Tasca**  
L’equip implementa almenys una operació real del domini, per exemple:
- alta o modificació d’un recurs
- creació o gestió d’una incidència
- reserva sotmesa a disponibilitat o franja
- canvi d’estat d’un element
- altra operació coherent amb el projecte

Esta operació ha d’estar protegida per:
- autenticació
- i, a més, per una regla de rol, permís o restricció de negoci

**Relació amb el producte principal**  
És la peça que dona sentit al repte: demostra que l’autenticació està al servei del producte i no és un mòdul aïllat.

**CA coberts**  
- **RA3**: criteris de control d’accés i restricció funcional
- **RA4**: criteris de construcció d’una funcionalitat web dinàmica real i útil

**Descripció dels CA en llenguatge docent**  
- L’alumnat construïx una funcionalitat amb valor real dins del projecte.
- L’alumnat controla qui pot executar-la i en quines condicions.
- L’alumnat demostra tant el cas correcte com el cas denegat.

**Paper de la IA**  
La IA pot ajudar a pensar restriccions o casos de prova, però la implementació i la verificació han de respondre al domini triat per l’equip.

**Evidències obligatòries**  
- operació funcional de domini
- protecció per autenticació
- restricció de rol, permís o regla de negoci
- demo de cas autoritzat
- demo de cas denegat
- prova o registre d’error quan no es complix la condició

**Instrument d’avaluació**  
Rúbrica de funcionalitat de negoci protegida.

**Indicadors d’assoliment**  
- la funcionalitat no és decorativa
- el control d’accés és real
- la restricció és observable
- el comportament és coherent en cas positiu i negatiu

**Riscos habituals**  
- operació trivial sense valor
- protecció només aparent
- restricció no comprovable
- domini inventat sense connexió amb el producte base

**Verificació del treball real**  
- execució en directe del cas autoritzat
- execució en directe del cas denegat
- pregunta oral: “quina condició concreta bloqueja l’acció i en quin punt del flux?”
- microcanvi en viu sobre la restricció o el missatge d’error

**Pes orientatiu dins del repte**  
35%

### Microprojecte MP4 — Validació, errors, proves i preparació del pas al Repte 3

**Tipus**  
Microprojecte de tancament i verificació.

**Objectiu**  
Consolidar el repte amb evidències tècniques suficients i deixar identificats els punts de deute tècnic o d’estructura que hauran de passar a refactorització en el Repte 3.

**Tasca**  
L’equip:
- revisa validacions i errors
- comprova casos positius, negatius i límit
- documenta instruccions de prova
- registra incidències detectades
- anota els punts que caldrà reorganitzar, encapsular o consolidar arquitectònicament en el repte següent

**Relació amb el producte principal**  
Sense esta capa final, el repte pot “funcionar”, però no queda prou verificat ni deixa clara la transició cap a una arquitectura més mantenible.

**CA coberts**  
- **RA2**: criteris de validació, tractament d’errors i verificació
- **RA3**: criteris de comprovació del comportament de sessió i accés
- **RA4**: criteris de qualitat funcional i consistència del cas d’ús implementat

**Descripció dels CA en llenguatge docent**  
- L’alumnat no només programa: també comprova i documenta.
- L’alumnat sap distingir entre una solució suficient per al repte actual i una solució encara no consolidada arquitectònicament.
- L’alumnat deixa preparada la transició cap al Repte 3.

**Paper de la IA**  
La IA pot ajudar a generar casos de prova o a redactar documentació, però l’alumnat ha de verificar que les proves descrites corresponen al comportament real.

**Evidències obligatòries**  
- registre de proves mínimes
- casos positius i negatius
- incidències detectades i correccions
- documentació tècnica actualitzada
- llista de punts de deute tècnic o refactorització
- defensa tècnica breu

**Instrument d’avaluació**  
Checklist de verificació + rúbrica de defensa tècnica.

**Indicadors d’assoliment**  
- proves mínimes reals
- errors ben documentats i tractats
- coherència entre documentació i comportament observat
- identificació clara del que passarà al Repte 3

**Riscos habituals**  
- proves inventades
- documentació embellida però no executable
- no saber explicar què falta per a una arquitectura més neta

**Verificació del treball real**  
- execució dels casos documentats
- contrast entre documentació, repositori i demo
- pregunta oral: “què passaria al Repte 3 a capes, servicis o persistència?”

**Pes orientatiu dins del repte**  
20%

---

## 6. Taula resum de microprojectes i criteris d’avaluació

| Microprojecte | Tipus | Producte o lliurable | CA coberts | Evidències principals | Instrument | Pes orientatiu |
|---|---|---|---|---|---|---|
| MP1 | Investigació / decisió tècnica | Flux d’accés, cas d’ús protegit i matriu de restriccions | RA3, RA4 | esquema, matriu, casos, defensa breu | Rúbrica | 15% |
| MP2 | Procedimental | Registre, login, logout i comprovació d’estat | RA2, RA3 | demo funcional, errors, commits, issues | Rúbrica + checklist | 30% |
| MP3 | Procedimental | Operació de domini protegida per autenticació i restricció | RA3, RA4 | cas autoritzat, cas denegat, restricció observable | Rúbrica | 35% |
| MP4 | Tancament / verificació | Proves, documentació, incidències i preparació del Repte 3 | RA2, RA3, RA4 | registre de proves, documentació, defensa | Checklist + rúbrica | 20% |

---

## 7. Evidències globals del repte

**Evidències mínimes comunes**  
- issue principal amb microtasques
- seqüència de commits significativa
- registre o alta d’usuari
- login i logout operatius
- comprovació d’usuari autenticat o sessió activa
- almenys una funcionalitat real del domini protegida
- una regla de rol, permís o restricció de negoci aplicada
- validació del costat servidor
- tractament consistent d’errors
- proves mínimes o registre de verificació funcional
- documentació tècnica actualitzada
- AI log quan hi haja ús d’IA

**Evidències opcionals d’ampliació**  
- ampliació de rols
- casos de prova extra
- millor tractament de missatges d’error
- test automatitzat mínim
- millor separació preliminar de responsabilitats
- anàlisi més fina del deute tècnic

---

## 8. Instruments d’avaluació del repte

### 8.1 Instruments principals
- rúbrica base de reptes adaptada al pes principal de RA2, RA3 i RA4
- rúbrica específica de funcionalitat autenticada
- checklist de revisió de repositori
- checklist específica de validació, autenticació i control d’accés
- defensa tècnica breu

### 8.2 Instruments de verificació
- execució en directe de casos positius i negatius
- comprovació d’estat abans i després del logout
- demostració del flux funcional complet del domini
- revisió d’errors i validacions
- contrast entre AI log, commits i resultat observat
- preguntes tècniques breus

---

## 9. Riscos d’ús inadequat de la IA

| Risc | Com es manifesta | Impacte | Mesura de control |
|---|---|---|---|
| Delegació excessiva | Fluxos d’autenticació no compresos | Alt | Defensa i preguntes tècniques |
| Confusió conceptual | Barreja entre sessió, autenticació, autorització o rol | Alt | Casos de contrast i execució guiada |
| Validació aparent | El cas feliç funciona però els errors no | Alt | Casos negatius obligatoris |
| Proves fictícies | Captures o descripcions sense correspondència amb el codi | Alt | Execució real |
| Funcionalitat de domini ornamental | Hi ha login però no hi ha producte real protegit | Alt | Exigir cas d’ús funcional amb restricció |

---

## 10. Mesures de control i verificació

**Per comprovar aprenentatge real**
- execució real de registre, login i logout
- comprovació d’usuari autenticat
- demo de cas autoritzat i cas denegat
- revisió de commits i issues
- contrast entre validacions definides i errors retornats
- pregunta de transferència
- canvi tècnic menut en directe
- revisió dels punts que passen al Repte 3

**Per distingir nivells d’autonomia**
- **treball autònom real**: l’alumne explica, adapta, prova i defensa
- **treball assistit per IA**: l’alumne usa suport, però valida i pren decisions
- **treball excessivament delegat**: l’alumne no comprén, no manté i no pot corregir

---

## 11. Adaptació realista a l’aula

**Duració orientativa**  
5 a 7 sessions, segons l’stack triat i el grau de maduresa del repositori heretat del Repte 1.

**Moment del curs**  
Després del Repte 1 i abans del Repte 3.

**Prerequisits**  
- repositori funcional del Repte 1
- README operatiu
- primera base backend executable
- criteri mínim de treball amb issues i commits

**Possibles variants tecnològiques**  
Es pot implementar amb l’stack adoptat per al curs, sempre que permeta:
- tractament de formularis o peticions equivalents
- validació en servidor
- sessions o mecanisme equivalent d’identificació
- control d’accés
- documentació i prova funcional

**Part comuna del grup**  
- model mínim d’usuari
- flux de registre, login i logout
- comprovació d’autenticació
- almenys una operació protegida
- validacions bàsiques
- proves mínimes
- documentació i defensa

**Ampliacions realistes**  
- rols addicionals
- més d’una operació protegida
- tractament d’errors més ric
- test automatitzat
- major qualitat arquitectònica preparatòria
- millor observabilitat del flux

**Recuperació o reforç per CA**  
- si fallen CA de RA2: reconstrucció de validacions, tractament d’errors i casos de prova
- si fallen CA de RA3: reimplementació o correcció del flux de sessió, autenticació i restricció
- si fallen CA de RA4: redisseny i defensa d’una funcionalitat de domini realment protegida

---

## 12. Tancament del repte

**Pregunta de síntesi per a l’alumnat**  
Quina operació real del producte hem aconseguit protegir, com demostrem que la identitat d’usuari i les restriccions funcionen, i què caldrà reorganitzar en el Repte 3?

**Criteri de superació del repte**  
El repte es considera superat quan:
- existix un flux funcional complet d’usuari amb registre o alta, login, logout i comprovació d’estat
- almenys una operació del producte queda protegida per autenticació
- existix com a mínim una regla de rol, permís o restricció de negoci aplicada i verificable
- la validació i el tractament d’errors són coherents i visibles
- el repositori aporta evidències autèntiques de treball
- l’ús de IA, si n’hi ha, queda registrat i validat
- el resultat deixa preparada la transició al Repte 3 sense haver de reconstruir la funcionalitat des de zero

**Observacions docents**  
El repte s’ha de llegir com a pas de funcionalitat usable dins del producte evolutiu. Un mòdul limitat a login, registre o logout sense una funcionalitat de negoci autenticada no es considera suficient.
