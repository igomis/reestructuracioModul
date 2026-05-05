# Programació d'aula del Repte 2

## Finalitat del document

Este document baixa `R2` a una seqüència operativa d'aula perquè el professorat puga conduir el repte com una progressió completa de dades, lògica, estat i autenticació, sense reduir-lo a “formulari + login”.

## Finalitat del repte

- consolidar una base comuna en `PHP` per a tot l'alumnat
- construir una primera funcionalitat real del producte a partir d'un flux complet de servidor
- fer visible la relació entre formulari, processament, lògica, estat, autenticació i funcionalitat protegida
- mantindre la persistència com a suport funcional del flux, no encara com a centre metodològic del repte
- preparar un pas net cap a `R3`, que serà el punt d'entrada dels itineraris diferenciats

## Duració base

- `21 hores`
- `7` sessions de `3` hores
- cada sessió es correspon amb un microprojecte docent concret

`R2` queda fixat amb estes `7` sessions com a base. La sessió `7` està dedicada específicament a refactorització i millora de mantenibilitat sobre un flux ja verificat.

## Coordinació explícita entre sessions i microprojectes

| Sessió | Duració | Microprojecte | Focus principal | Evidència clau |
|---|---:|---|---|---|
| `1` | `3h` | `MP1` | formulari i validació visible | dades recuperades, errors clars i reintent |
| `2` | `3h` | `MP2` | processament i guardat funcional | dada correcta tractada, guardada i reutilitzada |
| `3` | `3h` | `MP3` | lògica del flux i regles del projecte | decisió, estructura o funció amb efecte visible |
| `4` | `3h` | `MP4` | estat, sessió i/o cookies | recuperació del flux i invalidació controlada |
| `5` | `3h` | `MP5` | autenticació i funcionalitat protegida | cas autoritzat i cas denegat d'una operació real |
| `6` | `3h` | `MP6` | prova, depuració, documentació mínima i checkpoint tècnic | checklist, README i demo reproduïble |
| `7` | `3h` | `MP7` | refactorització final, organització en fitxers i primer objecte de domini | comparativa abans/després, reutilització en fitxers i justificació de la millora |

## Correspondència curta sessió -> RA -> evidència -> verificació

Esta taula és el mapa mínim de traçabilitat docent del repte. No substituïx la rúbrica ni les checklists, però ajuda a comprovar ràpidament que cada sessió deixa una evidència observable i una forma concreta de verificar aprenentatge real.

| Sessió | RA principal | Què s'aprén | Evidència mínima | Verificació docent |
|---|---|---|---|---|
| `1` | `RA2` + `RA3` | entrada de dades, recuperació en servidor i validació visible | formulari o entrada equivalent amb error i reintent corregit | execució en directe i pregunta sobre d'on ix cada dada i com arriba al servidor |
| `2` | `RA2` | generació de resposta, variables, operadors, àmbits i conservació funcional simple | dada correcta processada, guardada de manera simple i reutilitzada | canvi menut en viu sobre una variable, operador o directiva i justificació del mecanisme de conservació |
| `3` | `RA3` | decisions, arrays, funcions i regles de domini aplicades | regla amb dos resultats observables i funció o estructura útil | microcanvi en una condició o funció i explicació de per què no és ornamental |
| `4` | `RA4` | estat temporal, sessió, cookies i invalidació | recuperació d'estat i neteja o caducitat demostrada | execució de recuperació i invalidació, més pregunta sobre què queda en client, servidor o flux funcional |
| `5` | `RA4` | identificació, autenticació, autorització i protecció d'una operació real | cas autenticat permés i cas no permés sobre una acció del domini | demo dels dos casos i pregunta sobre el punt exacte on es comprova la restricció |
| `6` | `RA4` | prova, depuració, documentació i reproduïbilitat | taula mínima de proves, incidències i README actualitzat | execució d'un cas triat pel professorat i contrast amb documentació, codi i AI log |
| `7` | `RA3` + `RA4` | refactorització funcional, mantenibilitat i preparació cap a `RA5` | comparativa abans/després, fitxer comú, objecte simple i prova de no regressió | revisió del diff, execució del flux i defensa de què millora ara i què queda per a `R3` |

## Conceptes que han de quedar diferenciats

Durant el repte convé usar estos termes amb precisió, especialment en les sessions `4`, `5` i `6`:

- **Identificació**: l'usuari declara qui diu que és, per exemple amb un correu, nom d'usuari o identificador.
- **Autenticació**: el sistema comprova que eixa identitat és vàlida, per exemple amb credencials, i crea o reconeix una sessió autenticada.
- **Autorització**: el sistema decideix si un usuari ja autenticat pot executar una operació concreta segons rol, permís, propietat del recurs o regla de negoci.
- **Estat**: informació temporal o contextual que permet continuar un flux entre peticions.
- **Sessió**: mecanisme habitual per mantindre estat associat a un client des del servidor.

No es considera suficient dir que una operació està “protegida” si només hi ha login. Cal veure quina identitat s'ha declarat, com s'ha autenticat, quin estat o sessió queda activa i quina comprovació d'autorització o restricció funcional bloqueja o permet l'operació.

## Paper operatiu de la IA per fases

La IA pot aparéixer en totes les sessions, però el seu ús només compta com a suport vàlid si queda contrastat amb execució, proves i defensa posterior:

| Sessió | Ús raonable de la IA | Evidència de control |
|---|---|---|
| `1` | esborrany de formulari, missatges de validació o estructura inicial | l'alumnat explica el recorregut de cada camp i ajusta almenys una validació pròpia |
| `2` | exemples de processament, guardat simple o tractament de fitxer | prova real de reutilització de la dada i justificació del mecanisme triat |
| `3` | suggeriments de funcions, arrays o casos de decisió | defensa de la regla de domini i microcanvi en viu |
| `4` | interpretació d'errors de sessió, cookies o estat | demostració de què es guarda, on es guarda i quan s'invalida |
| `5` | esquelet de login, comprovació d'accés o missatges d'error | demo de cas permés i cas bloquejat, amb explicació del punt de control |
| `6` | generació o ampliació de casos de prova i ajuda en debugging | execució dels casos i registre de què s'ha acceptat, descartat o corregit |
| `7` | proposta de refactorització, detecció de duplicació o documentació | comparativa abans/després i justificació pròpia de la decisió final |

## Seqüència recomanada de sessions

### Sessió 1. Microprojecte 1

**Sessió 1 — Formulari i validació visible**

#### Finalitat específica de la sessió
Obrir el punt d'entrada de dades del producte i deixar clar què arriba al servidor, què es valida i què no pot continuar mentre hi haja errors.

#### RA/focus tècnic
Focus en `RA2` i `RA3`: recepció de dades de formulari o entrada equivalent, validació de servidor, resposta amb errors visibles i reintent corregit.

#### Producte o microresultat esperat
Formulari funcional o entrada equivalent del domini, amb almenys una validació de servidor, un missatge d'error útil i un reenviament correcte.

#### Seqüència temporal orientativa dins de les 3 hores

##### 0:00-0:20 — Obertura del flux de `R2`
- recordar la funcionalitat inicial prevista al final de `R1`
- concretar quina acció real del domini entrarà per formulari
- aclarir que esta sessió encara no comença per autenticació

##### 0:20-0:45 — Modelatge docent
- mostrar un formulari mínim o entrada equivalent
- recuperar dades en servidor
- validar un camp obligatori o una regla simple
- retornar un error comprensible sense perdre el sentit del flux

##### 0:45-1:35 — Implementació guiada
- l'alumnat crea o adapta el formulari
- connecta l'acció amb el servidor
- recupera dades i comprova què arriba realment
- incorpora la primera validació

##### 1:35-2:10 — Errors i reintent
- provar entrada buida, incorrecta o incompleta
- mostrar errors concrets
- conservar o reconstruir la informació necessària per a corregir
- repetir l'enviament amb dades vàlides

##### 2:10-2:40 — Revisió per parelles
- un company executa el formulari d'un altre
- identifica una dada vàlida i una no vàlida
- comprova que l'error talla el flux

##### 2:40-3:00 — Checkpoint final
- revisió ràpida del professorat
- registre de l'evidència mínima
- anotació de què es processarà i guardarà en la sessió `2`

#### Intervenció docent prevista
- acotar l'acció del domini perquè siga realista en una sessió
- evitar formularis decoratius sense tractament de servidor
- demanar errors concrets, no missatges genèrics
- revisar que la validació es fa en servidor encara que hi haja validació visual en client

#### Tasques concretes de l'alumnat
- concretar l'acció del domini que s'enviarà al servidor
- crear o adaptar el formulari
- recuperar dades en `PHP`
- validar almenys un camp o regla
- mostrar l'error i provar un reintent correcte
- deixar una nota breu en el `README` o en el registre de treball sobre el flux provat

#### Evidència verificable de la sessió
- formulari executable
- captura o demo curta d'un cas amb error
- captura o demo curta del mateix cas corregit
- codi on es veu la recuperació i validació de la dada

#### Checkpoint o pregunta de comprovació
Què passa exactament quan arriba una dada incorrecta i en quin punt del codi es talla el flux?

#### Ús de la IA permés i forma de control
Ús permés per aclarir patrons de validació, redactar missatges d'error o revisar si falten casos bàsics. Control: l'alumnat ha d'assenyalar en el seu codi on valida cada dada i ha de poder modificar una regla en directe sense dependre de la resposta generada.

#### Dificultats habituals i resposta docent prevista
- Si el formulari envia però no es comprova res, el professorat demana un cas incorrecte obligatori abans de continuar.
- Si només hi ha validació en client, es modela el mateix cas desactivant o saltant el client i es força la validació en servidor.
- Si l'alumnat vol començar per login, es reconduïx cap al flux de dades del domini i es deixa auth per a la sessió `5`.

### Sessió 2. Microprojecte 2

**Sessió 2 — Processament i guardat funcional**

#### Finalitat específica de la sessió
Convertir la dada validada en una resposta útil del servidor i deixar una primera conservació funcional de la informació correcta.

#### RA/focus tècnic
Focus en `RA2` i `RA3`: tractament de dades en servidor, variables, operadors, estructures bàsiques, guardat funcional i reutilització simple.

#### Producte o microresultat esperat
Entrada validada, processada, guardada de manera simple i reutilitzada en una resposta visible del producte.

#### Seqüència temporal orientativa dins de les 3 hores

##### 0:00-0:20 — Recuperació de la sessió anterior
- executar el formulari amb un cas vàlid
- identificar quina dada correcta passarà a processament
- recordar què no s'ha de guardar si la validació falla

##### 0:20-0:45 — Modelatge de processament
- transformar o calcular una resposta a partir de la dada
- separar dada rebuda, dada neta i resultat generat
- mostrar la resposta al navegador

##### 0:45-1:30 — Processament de l'alumnat
- implementar una transformació o decisió simple
- comprovar que el resultat canvia segons l'entrada
- afegir una eixida visible coherent amb el domini

##### 1:30-2:10 — Guardat funcional
- triar un mecanisme simple de conservació segons la base del grup
- guardar només informació validada
- recuperar-la després en una pantalla, llista o resposta equivalent

##### 2:10-2:40 — Reutilització i justificació
- demostrar que la dada guardada torna a usar-se
- justificar per què el mecanisme triat és suficient en `R2`
- detectar dades que no cal guardar encara

##### 2:40-3:00 — Checkpoint final
- comprovació d'un cas complet: enviar, validar, processar, guardar i reutilitzar
- registre d'incidències pendents
- preparació de la regla de negoci de la sessió `3`

#### Intervenció docent prevista
- recordar que la persistència encara és suport funcional, no el centre metodològic del repte
- orientar mecanismes simples de guardat sense obrir una arquitectura completa
- demanar que el guardat tinga un ús visible, no només un fitxer o taula creats
- revisar que no es guarden dades incorrectes

#### Tasques concretes de l'alumnat
- executar el flux vàlid de la sessió `1`
- processar la dada amb una transformació, càlcul o normalització simple
- guardar la informació correcta
- recuperar o mostrar la dada guardada
- justificar en una nota breu el mecanisme de guardat triat

#### Evidència verificable de la sessió
- codi de processament executable
- dada guardada després d'un cas vàlid
- reutilització visible de la dada
- nota breu de justificació del mecanisme de guardat

#### Checkpoint o pregunta de comprovació
On es veu que la dada validada no només s'ha rebut, sinó que s'ha processat, guardat i reutilitzat?

#### Ús de la IA permés i forma de control
Ús permés per aclarir sintaxi de `PHP`, proposar una transformació simple o revisar si el guardat és coherent. Control: l'alumnat ha de mostrar una prova amb una dada nova i explicar per què només es guarda després de validar.

#### Dificultats habituals i resposta docent prevista
- Si el guardat no es reutilitza, el professorat demana una pantalla o resposta on la dada aparega de nou.
- Si es vol introduir una base de dades completa sense necessitat, es limita a un ús mínim justificat o es posposa el modelatge fort a `R3`.
- Si el codi mescla massa entrada, procés i eixida, es deixa anotat com a material per a la refactorització de la sessió `7`.

### Sessió 3. Microprojecte 3

**Sessió 3 — Lògica del flux i regles del projecte**

#### Finalitat específica de la sessió
Fer que el backend aplique una regla recognoscible del domini i produïsca resultats diferents segons les dades i l'estat del flux.

#### RA/focus tècnic
Focus en `RA3`: condicions, recorreguts, arrays, funcions i regles de negoci simples aplicades al producte.

#### Producte o microresultat esperat
Una regla del domini implementada amb efecte visible i almenys dos casos de prova amb resultat diferent.

#### Seqüència temporal orientativa dins de les 3 hores

##### 0:00-0:25 — Selecció de la regla
- revisar el flux ja existent
- triar una regla xicoteta però significativa del producte
- formular la regla en llenguatge natural abans de programar-la

##### 0:25-0:50 — Modelatge docent
- convertir una regla en una condició o funció
- mostrar dos casos amb resultats diferents
- explicar per què una regla ha de canviar el comportament del sistema

##### 0:50-1:40 — Implementació de la regla
- l'alumnat implementa una decisió, recorregut o funció
- connecta la regla amb dades del flux
- evita dades fixes que només simulen funcionament

##### 1:40-2:15 — Casos de prova
- definir un cas que complix la regla
- definir un cas que no la complix
- executar els dos casos i observar la resposta

##### 2:15-2:40 — Revisió de qualitat mínima
- comprovar noms de variables i funcions
- detectar condicions duplicades o poc clares
- marcar possibles millores per a la sessió `7`

##### 2:40-3:00 — Checkpoint final
- demo curta de la regla
- registre dels dos casos provats
- anticipació de quina informació haurà de mantindre's entre peticions en la sessió `4`

#### Intervenció docent prevista
- ajudar a convertir regles massa grans en una regla executable en tres hores
- impedir lògica ornamental que no afecte el flux
- demanar casos diferents abans de donar per bona la sessió
- assenyalar duplicacions o responsabilitats confuses per a la refactorització final

#### Tasques concretes de l'alumnat
- escriure la regla en una frase clara
- implementar-la amb condició, array, recorregut o funció
- connectar-la amb dades reals del flux
- provar dos casos amb resultat diferent
- registrar quin comportament ha canviat

#### Evidència verificable de la sessió
- regla implementada en codi
- dos casos de prova executables
- resposta diferenciada del sistema
- nota breu de què decidix el backend i per què

#### Checkpoint o pregunta de comprovació
Quina decisió pren ara el servidor que abans no prenia, i com es veu en dos casos diferents?

#### Ús de la IA permés i forma de control
Ús permés per ajudar a expressar la regla, revisar una condició o proposar casos de prova. Control: l'alumnat ha d'explicar la regla sense llegir codi generat i ha de crear almenys un cas de prova propi no suggerit literalment per la IA.

#### Dificultats habituals i resposta docent prevista
- Si la regla és massa ambiciosa, el professorat la reduïx a una decisió mínima verificable.
- Si el resultat és sempre el mateix, es demanen dos casos que forcen branques diferents.
- Si la funció només embolica codi sense aclarir-lo, es revisa el nom, l'entrada i l'eixida esperada.

### Sessió 4. Microprojecte 4

**Sessió 4 — Estat, sessió i cookies sense confondre-ho amb persistència**

#### Finalitat específica de la sessió
Mantindre informació temporal entre peticions per donar continuïtat al flux i distingir clarament estat, sessió i cookies de la persistència del domini.

#### RA/focus tècnic
Focus en `RA2`, `RA3` i `RA4`: gestió d'estat temporal, `$_SESSION`, cookies, invalidació i lectura del recorregut petició-resposta.

#### Producte o microresultat esperat
Flux que recupera una informació temporal necessària, mostra què es guarda en sessió o cookie i permet invalidar-la de manera controlada.

#### Seqüència temporal orientativa dins de les 3 hores

##### 0:00-0:25 — Aclariment conceptual
- estat: informació que el sistema necessita recordar durant un flux
- sessió: estat associat a un usuari o navegador i guardat al servidor amb un identificador
- cookie: dada guardada al navegador, sovint usada per identificar o recordar informació limitada
- persistència: conservació estable de dades del domini més enllà del flux temporal

##### 0:25-0:50 — Modelatge docent
- activar sessió i guardar una dada temporal
- llegir la dada en una petició posterior
- observar la cookie de sessió en el navegador
- destruir o netejar la dada quan ja no té sentit

##### 0:50-1:35 — Implementació d'estat temporal
- l'alumnat tria què necessita recordar temporalment
- guarda la dada en sessió o cookie segons el cas
- recupera el flux en una pantalla posterior
- evita guardar dades sensibles en cookies

##### 1:35-2:10 — Invalidació i comprovació
- implementar eixida, reinici de flux o neteja de sessió
- provar què passa abans i després de la invalidació
- comprovar en eines de navegador què queda en cookies

##### 2:10-2:40 — Contrast amb persistència
- identificar quines dades són temporals
- identificar quines dades pertanyen al domini i haurien de persistir
- revisar errors habituals: usar sessió com si fora base de dades o cookie com si fora magatzem segur

##### 2:40-3:00 — Checkpoint final
- demo d'un flux recuperat
- demo d'invalidació
- explicació oral breu de què està en client, què està en servidor i què no és persistència

#### Intervenció docent prevista
- fer explícita la diferència entre recordar temporalment i guardar com a dada del producte
- revisar amb les eines del navegador quines cookies apareixen
- insistir que la cookie de sessió no conté necessàriament totes les dades de sessió
- tallar usos insegurs: contrasenyes, rols o dades sensibles en cookies sense criteri

#### Tasques concretes de l'alumnat
- decidir una dada temporal necessària del seu flux
- implementar-ne el guardat en sessió o cookie
- recuperar-la en una petició posterior
- invalidar-la amb una acció clara
- documentar en una frase què és estat temporal i què seria persistència del domini

#### Evidència verificable de la sessió
- codi d'inici, lectura i neteja de sessió o cookie
- demo abans/després de la invalidació
- captura o explicació de la cookie observada en el navegador
- nota breu distingint estat temporal, sessió, cookie i persistència

#### Checkpoint o pregunta de comprovació
Quina informació recorda el sistema només durant el flux, on està guardada i per què això no és encara persistència del domini?

#### Ús de la IA permés i forma de control
Ús permés per comparar sessió i cookie, revisar riscos de seguretat bàsics o generar una llista de comprovacions. Control: l'alumnat ha de demostrar en navegador què passa amb la cookie i en codi què passa amb `$_SESSION`, sense confondre-ho amb dades persistides.

#### Dificultats habituals i resposta docent prevista
- Si es diu que una cookie és “la sessió”, el professorat mostra la diferència entre identificador en client i dades de sessió en servidor.
- Si es guarda tot en sessió com si fora persistència, es demana separar dades temporals i dades del domini.
- Si no hi ha invalidació, la sessió no es dona per tancada fins que hi haja una neteja comprovable.

### Sessió 5. Microprojecte 5

**Sessió 5 — Identificació, autenticació, autorització i operació protegida**

#### Finalitat específica de la sessió
Connectar el flux construït amb una operació real del domini que només puga executar-se quan l'usuari està identificat, autenticat i autoritzat.

#### RA/focus tècnic
Focus en `RA4`: identificació d'usuari, comprovació de credencials, inici de sessió autenticada, autorització bàsica i bloqueig d'una operació protegida.

#### Producte o microresultat esperat
Login funcional mínim i una operació del domini protegida amb cas autoritzat i cas denegat reproduïbles.

#### Seqüència temporal orientativa dins de les 3 hores

##### 0:00-0:25 — Marc conceptual operatiu
- identificació: l'usuari diu qui és
- autenticació: el sistema comprova que pot demostrar-ho
- autorització: el sistema decidix què pot fer
- operació protegida: acció real del producte que no pot executar qualsevol visitant

##### 0:25-0:55 — Modelatge docent
- formulari de login o mecanisme equivalent
- comprovació de credencials de prova
- guardat de l'usuari autenticat en sessió
- protecció d'una operació real del domini
- resposta denegada quan no hi ha permís

##### 0:55-1:40 — Implementació d'identificació i autenticació
- l'alumnat crea o adapta el login
- comprova credencials de prova
- inicia sessió autenticada
- mostra una resposta clara d'error quan fallen les credencials

##### 1:40-2:20 — Autorització i operació protegida
- triar una acció del domini construïda en sessions anteriors
- impedir l'accés sense autenticació
- si hi ha rols o propietat, aplicar una restricció bàsica
- comprovar accés permés i denegat

##### 2:20-2:45 — Prova de casos
- usuari no autenticat intenta l'operació
- usuari autenticat executa l'operació
- usuari autenticat però no autoritzat, si el projecte ho permet
- tancament de sessió i nou intent

##### 2:45-3:00 — Checkpoint final
- demo curta del cas autoritzat i denegat
- identificació del punt exacte de codi on es comprova la restricció
- registre de casos pendents per al taller de proves de la sessió `6`

#### Intervenció docent prevista
- impedir que el login siga només una pantalla sense protecció real
- demanar que la protecció recaiga sobre una operació del domini, no només sobre una pàgina buida
- diferenciar verbalment i en codi identificació, autenticació i autorització
- revisar que l'operació protegida no es pot executar cridant directament la URL o el formulari

#### Tasques concretes de l'alumnat
- implementar o adaptar el formulari de login
- comprovar credencials amb un mecanisme mínim coherent
- guardar l'usuari autenticat en sessió
- protegir una operació real del domini
- provar accés permés, accés denegat i tancament de sessió
- documentar usuaris de prova i restriccions aplicades

#### Evidència verificable de la sessió
- login funcional
- sessió autenticada comprovable
- operació protegida del domini
- cas autoritzat i cas denegat executables
- nota breu indicant on es fa identificació, autenticació i autorització

#### Checkpoint o pregunta de comprovació
Quina operació real queda protegida, qui pot executar-la, qui no pot, i en quin punt del codi es decidix?

#### Ús de la IA permés i forma de control
Ús permés per revisar diferències entre identificació, autenticació i autorització, proposar casos de prova o detectar punts d'accés no protegits. Control: l'alumnat ha de fer una demo sense IA amb tres intents: no autenticat, autenticat permés i denegat o logout.

#### Dificultats habituals i resposta docent prevista
- Si només hi ha login però cap operació protegida, el professorat no valida la sessió i demana protegir una acció del domini.
- Si s'equipara autenticació amb autorització, es demana un exemple de “sé qui eres” i un altre de “pots fer açò”.
- Si la ruta protegida es pot invocar directament, es revisa el control al servidor abans de qualsevol execució de l'operació.

### Sessió 6. Microprojecte 6

**Sessió 6 — Taller de proves, depuració i checkpoint tècnic**

#### Finalitat específica de la sessió
Convertir la sessió en un taller de proves del flux complet, amb una bateria mínima comuna, registre d'incidències i documentació suficient per reproduir la demo.

#### RA/focus tècnic
Focus transversal en `RA2`, `RA3` i `RA4`: validació, errors controlats, flux autenticat, operació protegida, depuració i documentació tècnica mínima.

#### Producte o microresultat esperat
Bateria mínima de proves executada, incidències registrades, correccions prioritzades i `README` actualitzat amb instruccions de reproducció.

#### Seqüència temporal orientativa dins de les 3 hores

##### 0:00-0:25 — Presentació de la bateria mínima comuna
- cas `1`: formulari amb dades vàlides
- cas `2`: formulari amb dades invàlides
- cas `3`: dada validada, processada i reutilitzada
- cas `4`: estat temporal recuperat i invalidat
- cas `5`: accés no autenticat a operació protegida
- cas `6`: accés autenticat permés
- cas `7`: logout o invalidació i nou intent denegat
- cas `8`: error previsible documentat amb resposta clara

##### 0:25-0:45 — Modelatge de registre de prova
- mostrar com anotar entrada, passos, resultat esperat i resultat real
- diferenciar error funcional, error de validació i error de permisos
- prioritzar incidències que bloquegen el flux

##### 0:45-1:35 — Execució individual o per parelles
- l'alumnat executa la bateria mínima
- registra resultats i captures si cal
- marca incidències bloquejants i menors
- evita corregir sense haver reproduït abans el problema

##### 1:35-2:15 — Depuració guiada
- corregir primer errors que trenquen el flux complet
- usar missatges, logs o inspecció controlada
- repetir el cas fallit després de corregir
- deixar constància de la correcció

##### 2:15-2:40 — Documentació mínima
- actualitzar `README` amb passos d'arrancada i prova
- afegir usuaris de prova si aplica
- indicar l'operació protegida i els casos bàsics
- deixar pendents clars per a la sessió `7`

##### 2:40-3:00 — Checkpoint tècnic
- demo curta d'un cas complet
- revisió ràpida de la bateria mínima
- decisió docent sobre si el grup pot passar a refactoritzar o ha de reparar abans el flux

#### Intervenció docent prevista
- conduir la sessió com a taller, no com a explicació llarga
- exigir la bateria comuna abans de millores voluntàries
- ajudar a reproduir errors abans de tocar codi
- prioritzar correccions que afecten validació, estat, autenticació i operació protegida

#### Tasques concretes de l'alumnat
- executar la bateria mínima comuna
- registrar resultat esperat i resultat real
- corregir incidències bloquejants
- repetir les proves fallides
- actualitzar `README`
- marcar una zona concreta del codi que es refactoritzarà en la sessió `7`

#### Evidència verificable de la sessió
- taula o checklist de proves completada
- registre d'almenys una incidència o confirmació explícita que no n'hi ha
- correcció comprovada quan hi havia error
- `README` actualitzat
- demo reproduïble del flux complet

#### Checkpoint o pregunta de comprovació
Quins casos mínims demostren que el flux no és una demo puntual, sinó una funcionalitat reproduïble amb errors i permisos controlats?

#### Ús de la IA permés i forma de control
Ús permés per generar casos de prova addicionals, ajudar a interpretar un error o revisar el `README`. Control: la bateria mínima comuna és obligatòria i l'alumnat ha de registrar resultats reals executats, no només una llista generada.

#### Dificultats habituals i resposta docent prevista
- Si l'alumnat corregeix sense reproduir, el professorat demana tornar al cas fallit i registrar-lo.
- Si només prova el camí feliç, es bloqueja el checkpoint fins provar errors i accés denegat.
- Si el `README` no permet repetir la demo, es dedica el tram final a documentació abans de refactoritzar.

**Bateria mínima obligatòria de prova**

La sessió `6` ha de deixar registrada una taula breu amb estos casos, encara que la forma siga manual, amb peticions guardades o amb proves automatitzades simples:

| Cas | Què comprova | Resultat esperat |
|---|---|---|
| cas vàlid | el flux complet accepta dades correctes i executa l'operació prevista | resposta correcta i dada reutilitzable dins del projecte |
| cas invàlid per validació | el servidor rebutja dades absents, mal formades o incoherents | error interpretable i possibilitat de correcció |
| cas no autenticat | una persona sense sessió vàlida intenta accedir a una part protegida | bloqueig, redirecció o resposta coherent |
| cas amb sessió caducada o estat invàlid | el sistema rep un estat que ja no hauria de permetre continuar | invalidació controlada i missatge o resposta coherent |
| cas d'accés a operació protegida | un usuari autenticat intenta una operació sotmesa a restricció de domini | permís o denegació segons la regla definida, no segons una ruta decorativa |

Cada cas ha d'incloure entrada, resultat esperat, resultat obtingut i incidència si n'hi ha. Si la IA ajuda a proposar proves, l'equip ha d'indicar quines accepta, quines descarta i què ha verificat manualment.

### Sessió 7. Microprojecte 7

**Sessió 7 — Refactorització com a millora de responsabilitats i mantenibilitat**

#### Finalitat específica de la sessió
Millorar codi que ja funciona perquè tinga responsabilitats més clares, menys duplicació i una estructura més mantenible, sense convertir el tancament de `R2` en una reescriptura arquitectònica.

#### RA/focus tècnic
Focus transversal en `RA2`, `RA3` i preparació de `R3`: organització de codi, reutilització, responsabilitats, `include` / `require`, funcions comunes i primer objecte simple del domini.

#### Producte o microresultat esperat
Comparativa abans/després amb una millora concreta de mantenibilitat: menys duplicació, responsabilitats més clares, fitxer comú importat amb criteri i, si és viable, una entitat simple del domini.

#### Seqüència temporal orientativa dins de les 3 hores

##### 0:00-0:25 — Selecció de zona de refactorització
- partir de la bateria de proves de la sessió `6`
- triar una part del codi que funciona però és difícil de mantindre
- identificar duplicació, mescla de responsabilitats o noms confusos

##### 0:25-0:55 — Modelatge docent
- mostrar un abans/després curt
- extraure una funció o fitxer comú
- importar-lo amb `require_once` o equivalent
- explicar què ha canviat en responsabilitats, no només en ubicació de fitxers
- repetir una prova per comprovar que no hi ha regressió

##### 0:55-1:45 — Refactorització de l'alumnat
- netejar una part acotada del flux
- separar preparació de dades, validació, acció o renderitzat quan siga possible
- extraure funcions comunes o configuració repetida
- usar `include`, `require`, `include_once` o `require_once` amb criteri

##### 1:45-2:15 — Primer objecte o entitat mínima del domini
- representar una entitat simple si aporta claredat
- evitar POO completa obligatòria
- justificar què representa l'objecte i quina responsabilitat concentra

##### 2:15-2:40 — Prova de no regressió
- repetir casos clau de la bateria mínima
- comprovar operació protegida
- corregir errors introduïts per la refactorització

##### 2:40-3:00 — Tancament `R2 -> R3`
- redactar comparativa abans/després
- justificar la millora de mantenibilitat
- identificar què quedarà per reorganitzar amb més profunditat en `R3`

#### Intervenció docent prevista
- insistir que refactoritzar és millorar responsabilitats i mantenibilitat, no moure codi sense criteri
- limitar l'abast perquè no es trenque el flux complet
- demanar proves després de cada canvi rellevant
- frenar reescriptures grans i convertir-les en pendents de `R3`

#### Tasques concretes de l'alumnat
- triar una zona concreta del codi ja provat
- identificar quin problema de mantenibilitat vol corregir
- fer una refactorització xicoteta i verificable
- extraure o importar almenys un fitxer comú quan tinga sentit
- introduir una entitat simple del domini si ajuda a aclarir responsabilitats
- repetir proves mínimes
- escriure una comparativa abans/després

#### Evidència verificable de la sessió
- diff o comparativa abans/després
- fitxer comú importat amb criteri o funcions comunes reutilitzades
- reducció visible de duplicació, mescla o responsabilitats confuses
- prova de no regressió del flux complet
- justificació breu de la millora de mantenibilitat

#### Checkpoint o pregunta de comprovació
Quina responsabilitat queda ara més clara que abans i com has comprovat que el flux continua funcionant?

#### Ús de la IA permés i forma de control
Ús permés per detectar duplicacions, proposar noms, suggerir una extracció de funció o revisar una comparativa abans/després. Control: cap canvi proposat per IA es dona per bo sense executar la bateria mínima de no regressió i sense justificació pròpia de la responsabilitat millorada.

#### Dificultats habituals i resposta docent prevista
- Si només es mou codi a un altre fitxer, el professorat demana explicar quina responsabilitat ha quedat més clara.
- Si la refactorització trenca el flux, es torna a la prova fallida i es redueix l'abast del canvi.
- Si l'alumnat intenta fer arquitectura completa, es marca com a pont cap a `R3` i es tanca `R2` amb una millora acotada.

La refactorització no s'ha de valorar només per “tindre més fitxers”. Ha de millorar almenys una responsabilitat concreta: validació, tractament de dades, comprovació d'accés, renderitzat, reutilització de missatges o representació d'una entitat del domini. La defensa breu ha d'explicar quin problema del codi inicial s'ha reduït, quin risc de regressió s'ha comprovat i quina part continua pendent per al treball arquitectònic de `R3`.

## Criteri metodològic de la sessió 7

Què sí pot incloure:

- netejar barreja excessiva de `HTML + PHP`
- extraure funcions útils a un fitxer separat
- usar `include` / `require` o, millor encara quan toque, `include_once` / `require_once`
- ordenar millor el codi
- millorar noms
- reduir duplicació
- separar millor preparació de dades i renderitzat
- incorporar una entitat mínima del domini com a objecte simple
- justificar per què la nova versió és més clara i mantenible

Què no ha de convertir-se en:

- entrada obligatòria a POO completa
- entrada obligatòria a BBDD com a focus central
- reescriptura arquitectònica total del repte
- arquitectura completa tipus `MVC`

Si apareixen més classes, més objectes o una persistència més formal, s'han de plantejar com a tast introductori, ampliació opcional o pont cap a `R3`.

## Evidències esperades per sessió

- Sessió `1`: formulari o entrada equivalent, recuperació real de dades i errors visibles.
- Sessió `2`: tractament executable, guardat funcional i primera reutilització de la informació correcta.
- Sessió `3`: decisió, regla o funció amb efecte real sobre el flux.
- Sessió `4`: estat recuperable, demostració d'invalidació i frontera clara entre estat i conservació funcional.
- Sessió `5`: operació del domini protegida amb cas autoritzat i cas denegat.
- Sessió `6`: checklist de prova, documentació mínima i checkpoint tècnic.
- Sessió `7`: comparativa breu abans/després, fitxer comú importat amb criteri, objecte simple del domini i comprovació final del flux.

## Moments de checkpoint

- Checkpoint curt `1`: al final de la sessió `2`, per comprovar que el flux ja rep, valida, processa i reutilitza dades.
- Checkpoint curt `2`: al final de la sessió `4`, per validar que estat, sessió o cookies no s'estan confonent amb persistència del domini.
- Checkpoint curt `3`: al final de la sessió `5`, per confirmar que hi ha una operació real protegida.
- Checkpoint tècnic `4`: al final de la sessió `6`, per confirmar que el flux és reproduïble, provat i documentat.
- Checkpoint de pas `R2 -> R3`: al final de la sessió `7`, per decidir si el grup entra al contrast de frameworks amb una base funcional i una primera millora de mantenibilitat defensable.

## Preparació del tancament del repte

- demanar una demo curta del flux complet, no només del login
- revisar que la informació correcta es recupera o es reutilitza dins del projecte
- exigir la bateria mínima de proves de la sessió `6`: cas vàlid, cas invàlid per validació, cas no autenticat, cas amb sessió caducada o estat invàlid i cas d'accés a operació protegida
- comprovar que la documentació mínima permet repetir la prova
- demanar una refactorització lleu sobre codi que ja funciona i una justificació breu del canvi
- demanar què haurà de reorganitzar-se en `R3` i què encara continua sent suport funcional de `R2`

## Criteri pràctic de tancament

`R2` queda preparat quan el professorat pot veure un flux complet de dades, lògica, estat i autenticació sobre la base comuna en `PHP`, amb una operació real protegida, proves mínimes reproduïbles, una sessió final de refactorització amb millora de mantenibilitat justificable i un pas net cap a `R3`.

La sessió `7` ha de demostrar que el codi queda una mica més clar i mantenible sense convertir el repte en una reescriptura arquitectònica completa.
