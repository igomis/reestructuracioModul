# R2S1. Entrada variada i validació de servidor

## Finalitat de la sessió

Esta sessió obri el `Repte 2` i treballa el microrepte `R2M1` amb una primera entrada real de dades del producte. L'objectiu no és practicar un camp solt ni fer tots els controls possibles, sinó entendre bé el recorregut mínim d'un formulari: text, llista o opció tancada, checkbox, recepció en servidor, validació, errors visibles i reintent.

Al final de la sessió, cada alumne o parella ha de poder explicar quines dades envia cada control mínim, com arriben al servidor, quines validacions s'apliquen i què passa quan alguna dada no és acceptable.

## Encaix dins del Repte 2

- **Repte**: `R2. Processament bàsic, estat, autenticació i primera funcionalitat protegida`
- **Microrepte**: `R2M1`
- **Sessió**: `R2S1`
- **Duració orientativa**: `3 hores`
- **Focus**: formulari mínim amb text, llista/opció i checkbox; recuperació de dades en `PHP`; validació de servidor; errors visibles i reintent
- **No entra encara**: login, rols, sessió persistent, base de dades com a centre del treball o arquitectura completa

## Relació amb RA i criteris de treball

| Element | Concreció en el microrepte |
|---|---|
| `RA2` | codi servidor integrat amb resposta web, recepció de dades, variables, arrays i generació de resposta |
| `RA3` | formularis amb diferents tipus d'entrada, comprovació de dades i bifurcació entre cas vàlid i cas amb error |
| Evidència central | enviament incorrecte, errors visibles, correcció i reenviament correcte |
| Verificació docent | execució en directe i pregunta sobre el recorregut de cada dada |

## Producte esperat

Un primer flux executable del producte amb un formulari o entrada equivalent que incloga, com a mínim:

- una acció concreta del domini;
- un camp de text o àrea de text;
- una llista desplegable o selecció equivalent;
- un checkbox simple amb sentit dins del flux;
- una validació específica per a cada tipus de dada;
- missatges d'error clars i associats al control afectat;
- un reintent corregit que deixe continuar el flux;
- una nota breu al `README`, issue o registre de treball indicant com provar el cas correcte i els casos incorrectes.

Queden com a ampliació o modelatge docent:

- checkbox múltiple amb catàleg de valors permesos;
- conservació més còmoda dels valors introduïts en el reintent;
- fitxer opcional si el cas d'ús ho justifica, amb `enctype`, `$_FILES`, error de pujada, mida i tipus permés.

## Preparació prèvia del professorat

Abans de la sessió convé tindre preparat:

- un exemple mínim de formulari amb `method="post"` i controls diversos;
- una variant curta amb `enctype="multipart/form-data"` només per mostrar fitxers si el grup va ràpid;
- un error controlat per a text buit, llista sense selecció o valor no permés i checkbox no marcat;
- una pauta curta per ajudar l'alumnat a triar una acció real del seu producte;
- el criteri de tancament: no es passa a processament ni guardat si no hi ha validació visible en servidor.

Exemples d'accions assumibles:

- registrar una incidència amb títol, prioritat i acceptació de condicions;
- sol·licitar una reserva amb nom, franja horària i confirmació;
- afegir un producte provisional amb nom, categoria i opció de visibilitat;
- demanar una cita amb dades de contacte, preferències i acceptació de condicions;
- crear una proposta amb descripció, tipus i confirmació de requisits.

## Controls mínims i ampliacions

| Control | Què ha de veure l'alumnat | Validació mínima de servidor |
|---|---|---|
| Text o textarea | arriba com a cadena i cal normalitzar-la | obligatori, longitud mínima o màxima |
| Select o radio | arriba com a valor triat d'un conjunt | el valor ha d'estar dins de la llista permesa |
| Checkbox simple | pot no aparéixer en la petició si no està marcat | comprovar presència quan siga obligatori |
| Checkbox múltiple | ampliació: arriba com a array si el `name` està ben definit | almenys una opció i opcions dins del catàleg permés |
| Fitxer | ampliació/modelatge: arriba per `$_FILES` i pot fallar abans de validar contingut | error de pujada, mida, extensió o MIME permés |

## Seqüència d'aula de 3 hores

### 0:00-0:15. Entrada al repte i acotació del formulari

El professorat recorda que `R2` no comença per autenticació. Primer cal una entrada real que arribe al backend amb dades de formats diferents.

Tasques:

- recuperar el punt d'entrada creat en `R1`;
- triar una acció concreta del producte;
- decidir els controls mínims: text, llista o opció tancada i checkbox;
- escriure quina dada aporta cada control al flux.

Resultat del tram: cada equip té una acció i un conjunt mínim de controls identificats.

### 0:15-0:45. Modelatge docent

El professorat mostra un flux mínim:

- formulari amb text, select i checkbox;
- recepció amb `$_POST`;
- diferència entre dada absent, cadena buida i array d'opcions;
- validació contra una llista de valors permesos;
- resposta d'error o resposta correcta.

Si el grup està preparat o el docent vol deixar-ho vist com a ampliació, el modelatge inclou una pujada de fitxer:

- `enctype="multipart/form-data"`;
- lectura de `$_FILES`;
- comprovació d'error, mida i tipus permés;
- explicació de per què no es confia en el nom del fitxer.

Resultat del tram: l'alumnat veu que cada control genera una forma diferent de dada i que la validació s'ha de fer en servidor.

### 0:45-1:30. Implementació guiada

L'alumnat implementa o adapta el seu formulari.

Tasques:

- crear o revisar el formulari;
- comprovar que el botó envia realment una petició;
- recuperar text, llista i checkbox en `PHP`;
- mostrar temporalment les dades rebudes per verificar què arriba;
- afegir validacions específiques per a cada control;
- deixar checkbox múltiple o fitxer per a ampliació si el mínim encara no està tancat.

Resultat del tram: hi ha dades variades recuperades i validacions inicials executant-se.

### 1:30-2:05. Errors visibles i reintent

L'alumnat força casos incorrectes i ajusta la resposta.

Tasques:

- provar text buit o massa curt;
- provar valor manipulat o no permés en la llista;
- provar checkbox obligatori sense marcar;
- provar checkbox múltiple o fitxer només si s'han implementat com a ampliació;
- mostrar missatges d'error concrets;
- conservar o reconstruir la informació necessària perquè el reintent siga possible.

Resultat del tram: el flux diferencia casos incorrectes i cas correcte, amb errors associats al control afectat.

### 2:05-2:30. Revisió per parelles

Una altra persona prova el formulari.

Pauta de revisió:

- quins controls envia el formulari?
- què arriba com a cadena, què arriba com a array i què pot no arribar?
- quin error es veu si una dada és incorrecta?
- es pot corregir sense reiniciar el projecte?
- on està la validació de cada tipus de dada?

Resultat del tram: cada equip rep una observació concreta i corregeix almenys una confusió o omissió.

### 2:30-2:45. Traçabilitat i documentació mínima

L'alumnat deixa rastre del que ha fet.

Tasques:

- actualitzar el `README`, issue o registre de treball;
- escriure com provar el cas correcte;
- escriure com provocar almenys tres errors diferents;
- registrar una dificultat trobada i com s'ha resolt o què queda pendent.

Resultat del tram: el flux és reproduïble per una altra persona.

### 2:45-3:00. Checkpoint docent

El professorat fa una comprovació curta.

Cada equip mostra:

- enviament incorrecte amb errors visibles;
- reenviament corregit;
- fragment de codi on es recupera text, llista i checkbox;
- fragment de codi on es valida contra valors permesos;
- fragment de codi de fitxer només si s'ha treballat com a ampliació.

Pregunta de tancament: què passa exactament quan falta una dada, quan arriba una opció no permesa o quan el checkbox no s'ha marcat?

## Tasques concretes de l'alumnat

- Triar una acció real del seu producte.
- Crear o adaptar un formulari amb controls diversos.
- Recuperar dades de text, llista i checkbox en `PHP`.
- Validar en servidor els controls mínims.
- Mostrar errors útils i comprensibles.
- Provar casos incorrectes i un cas correcte.
- Documentar com repetir les proves.

## Evidències mínimes

| Evidència | Mínim acceptable |
|---|---|
| Formulari o entrada | envia una petició real amb controls diversos |
| Recuperació de dades | el codi mostra on es llig text, select/radio i checkbox |
| Validació | text, llista/opció i checkbox tenen una regla en servidor |
| Error visible | el cas incorrecte queda bloquejat amb missatge concret |
| Reintent | la persona pot corregir i enviar de nou |
| Ampliació | checkbox múltiple o fitxer només si el mínim ja està aconseguit |
| Documentació | el repositori explica com provar cas correcte i errors |

## Criteris d'èxit

El microrepte està aconseguit si:

- el formulari no és decoratiu;
- hi ha més d'un tipus de control treballat;
- la validació no depén només del navegador;
- els valors de llistes i opcions es comproven contra catàlegs permesos;
- els checkbox no es tracten com si sempre arribaren;
- el cas incorrecte no continua com si fora correcte;
- l'error ajuda a corregir;
- el cas correcte és reproduïble;
- l'alumne pot assenyalar el recorregut de cada dada en el codi.

## Què no és suficient

- Tindre només `HTML` sense tractament en servidor.
- Fer un formulari amb un únic camp de text.
- Usar només `required` o validació de client.
- Acceptar qualsevol valor d'un select o d'un checkbox manipulat.
- Afegir fitxers abans de tindre validats text, llista i checkbox.
- Mostrar un missatge d'error sense condició real.
- Fer login o registre d'usuaris sense haver validat abans dades del domini.
- Copiar codi generat per IA sense poder modificar una regla de validació.
- Escriure al `README` que funciona sense indicar com provar-ho.

## Ús de la IA

La IA es pot usar per:

- proposar una estructura inicial de formulari amb controls diversos;
- revisar missatges de validació;
- suggerir casos d'error;
- explicar diferències entre `$_POST` i `$_FILES`;
- ajudar a redactar la nota de reproducció.

Control obligatori:

- l'alumnat ha de poder canviar una regla de validació en directe;
- ha d'explicar què ha acceptat, descartat o modificat de la resposta de la IA;
- ha de provar un cas manipulat o no previst, no només el cas feliç;
- si la IA ha generat una part rellevant del codi, s'ha de registrar breument al `AI log` o registre equivalent.

## Suport per alumnat amb més dificultat

Reduir el flux a:

- un text obligatori;
- un select amb tres valors permesos;
- un checkbox d'acceptació obligatori;
- una sola regla clara per control;
- una pàgina de resposta;
- una prova correcta i tres incorrectes.

Frase guia: "No afegis més pantalles fins que pugues ensenyar una dada incorrecta bloquejada per cada tipus de control."

## Ampliació per alumnat avançat

Si el mínim ja està tancat, l'alumnat pot:

- afegir checkbox múltiple amb catàleg permés;
- conservar els valors escrits i seleccionats perquè el reintent siga més còmode;
- afegir validació de fitxer amb mida i MIME;
- separar funcions simples de validació;
- afegir proves manuals més precises al `README`;
- preparar quines dades es processaran i guardaran en `R2M2`.

L'ampliació no ha d'obrir encara autenticació, rols ni arquitectura completa.

## Checklist de tancament

- [ ] He triat una acció real del meu producte.
- [ ] El formulari envia dades al servidor.
- [ ] He usat almenys text, llista i checkbox.
- [ ] Puc assenyalar on recupere cada dada en `PHP`.
- [ ] Valide text, llista/opció i checkbox en servidor.
- [ ] Comprove opcions contra valors permesos.
- [ ] He provat almenys tres casos incorrectes.
- [ ] Els errors indiquen què cal corregir.
- [ ] He provat el reintent amb dades correctes.
- [ ] Si hi ha fitxer, valide error, mida i tipus.
- [ ] El `README`, issue o registre explica com repetir les proves.
- [ ] Si he usat IA, he registrat què m'ha aportat i què he verificat.

## Connexió amb R2M2

`R2M2` només té sentit si `R2M1` deixa dades correctes i validades. La pregunta de pas és:

Quines dades validades del teu formulari es poden processar, guardar de manera simple i tornar a mostrar en la pròxima sessió?
