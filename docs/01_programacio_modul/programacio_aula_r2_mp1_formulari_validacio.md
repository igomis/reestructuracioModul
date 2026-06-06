# R2-MP1. Formulari i validació visible

## Finalitat del microrepte

Este microrepte obri el `Repte 2` amb una primera entrada real de dades del producte. L'objectiu no és fer una pantalla bonica ni avançar encara autenticació, sinó demostrar que el servidor rep dades, les valida, mostra errors útils i permet repetir el flux amb dades corregides.

Al final de la sessió, cada alumne o parella ha de poder explicar quin camp entra al servidor, on es valida, què passa quan falla i com es torna a executar el cas correcte.

## Encaix dins del Repte 2

- **Repte**: `R2. Processament bàsic, estat, autenticació i primera funcionalitat protegida`
- **Microrepte**: `MP1`
- **Sessió base**: `1`
- **Duració orientativa**: `3 hores`
- **Focus**: formulari o entrada equivalent, recuperació de dades en `PHP`, validació de servidor, errors visibles i reintent
- **No entra encara**: login, rols, sessió persistent, base de dades com a centre del treball o arquitectura completa

## Relació amb RA i criteris de treball

| Element | Concreció en el microrepte |
|---|---|
| `RA2` | codi servidor integrat amb resposta web, recepció de dades, variables i generació de resposta |
| `RA3` | formularis o entrada equivalent, comprovació de dades i bifurcació entre cas vàlid i cas amb error |
| Evidència central | enviament incorrecte, error visible, correcció i reenviament correcte |
| Verificació docent | execució en directe i pregunta sobre el recorregut de la dada |

## Producte esperat

Un primer flux executable del producte amb:

- una acció concreta del domini que demana almenys una dada;
- un formulari `HTML` o entrada equivalent connectada amb `PHP`;
- recuperació de la dada en el servidor;
- una validació mínima feta en servidor;
- un missatge d'error clar quan la dada no és acceptable;
- un reintent corregit que deixe continuar el flux;
- una nota breu al `README`, issue o registre de treball indicant com provar el cas correcte i el cas incorrecte.

## Preparació prèvia del professorat

Abans de la sessió convé tindre preparat:

- un exemple mínim de formulari amb `method="post"` i tractament en `PHP`;
- un error controlat per mostrar què passa quan falta una dada;
- una pauta curta per ajudar l'alumnat a triar una acció real del seu producte;
- el criteri de tancament: no es passa a processament ni guardat si no hi ha validació visible en servidor.

Exemples d'accions assumibles:

- sol·licitar una reserva amb nom i data;
- afegir un producte provisional a un catàleg;
- registrar una incidència amb títol i descripció;
- demanar una cita o torn amb correu de contacte;
- filtrar una llista per una paraula clau obligatòria.

## Seqüència d'aula de 3 hores

### 0:00-0:15. Entrada al repte i acotació del flux

El professorat recorda que `R2` no comença per autenticació. Primer cal una dada real que entre al backend.

Tasques:

- recuperar el punt d'entrada creat en `R1`;
- triar una acció concreta del producte;
- escriure en una frase quina dada entrarà al servidor i per què és necessària.

Resultat del tram: cada equip té una acció i una dada principal identificades.

### 0:15-0:40. Modelatge docent

El professorat mostra un flux mínim:

- formulari amb una dada obligatòria;
- recepció amb `$_POST` o mecanisme equivalent;
- normalització simple, com `trim`;
- comprovació d'una condició;
- resposta d'error o resposta correcta.

El modelatge ha de verbalitzar el recorregut: navegador envia, servidor rep, `PHP` valida, resposta torna al navegador.

Resultat del tram: l'alumnat veu un patró mínim i identifica on no s'ha de confiar només en el client.

### 0:40-1:25. Implementació guiada

L'alumnat implementa el seu primer formulari o adapta el punt d'entrada existent.

Tasques:

- crear o revisar el formulari;
- comprovar que el botó envia realment una petició;
- recuperar la dada en `PHP`;
- mostrar temporalment la dada rebuda per verificar que arriba;
- afegir una primera validació de servidor.

Resultat del tram: hi ha dada recuperada i una validació inicial executant-se.

### 1:25-1:55. Error visible i reintent

L'alumnat força un cas incorrecte i ajusta la resposta.

Tasques:

- provar camp buit, format incorrecte o valor fora de rang;
- mostrar un missatge d'error concret;
- evitar missatges genèrics com "error";
- conservar o reconstruir la informació necessària perquè el reintent siga possible;
- repetir amb una dada vàlida.

Resultat del tram: el flux diferencia cas incorrecte i cas correcte.

### 1:55-2:25. Revisió per parelles

Una altra persona prova el formulari.

Pauta de revisió:

- quin camp ha enviat?
- quin error es veu si falta o és incorrecte?
- es pot corregir sense reiniciar el projecte?
- on està la validació en el codi?

Resultat del tram: cada equip rep una observació concreta i corregeix almenys una confusió o omissió.

### 2:25-2:45. Traçabilitat i documentació mínima

L'alumnat deixa rastre del que ha fet.

Tasques:

- actualitzar el `README`, issue o registre de treball;
- escriure com provar el cas correcte;
- escriure com provocar l'error;
- registrar una dificultat trobada i com s'ha resolt o què queda pendent.

Resultat del tram: el flux és reproduïble per una altra persona.

### 2:45-3:00. Checkpoint docent

El professorat fa una comprovació curta.

Cada equip mostra:

- enviament incorrecte amb error visible;
- reenviament corregit;
- fragment de codi on es recupera la dada;
- fragment de codi on es valida.

Pregunta de tancament: què passa exactament quan arriba una dada incorrecta i en quin punt del codi es talla el flux?

## Tasques concretes de l'alumnat

- Triar una acció real del seu producte.
- Crear o adaptar un formulari o entrada equivalent.
- Recuperar dades en `PHP`.
- Validar almenys una dada en servidor.
- Mostrar un error útil i comprensible.
- Provar un cas incorrecte i un cas correcte.
- Deixar una nota breu de reproducció al repositori.

## Evidències mínimes

| Evidència | Mínim acceptable |
|---|---|
| Formulari o entrada | envia una petició real al servidor |
| Recuperació de dades | el codi mostra on es llig la dada rebuda |
| Validació | almenys una regla es comprova en servidor |
| Error visible | el cas incorrecte queda bloquejat amb missatge concret |
| Reintent | la persona pot corregir i enviar de nou |
| Documentació | el repositori explica com provar cas correcte i error |

## Criteris d'èxit

El microrepte està aconseguit si:

- el formulari no és decoratiu;
- la validació no depén només del navegador;
- el cas incorrecte no continua com si fora correcte;
- l'error ajuda a corregir;
- el cas correcte és reproduïble;
- l'alumne pot assenyalar el recorregut de la dada en el codi.

## Què no és suficient

- Tindre només `HTML` sense tractament en servidor.
- Usar només `required` o validació de client.
- Mostrar un missatge d'error sense condició real.
- Fer login o registre d'usuaris sense haver validat abans una dada del domini.
- Copiar codi generat per IA sense poder modificar una regla de validació.
- Escriure al `README` que funciona sense indicar com provar-ho.

## Ús de la IA

La IA es pot usar per:

- proposar una estructura inicial de formulari;
- revisar missatges de validació;
- suggerir casos d'error;
- explicar una errada de `PHP`;
- ajudar a redactar la nota de reproducció.

Control obligatori:

- l'alumnat ha de poder canviar una regla de validació en directe;
- ha d'explicar què ha acceptat, descartat o modificat de la resposta de la IA;
- si la IA ha generat una part rellevant del codi, s'ha de registrar breument al `AI log` o registre equivalent.

## Suport per alumnat amb més dificultat

Reduir el flux a:

- un sol camp obligatori;
- una sola regla de validació;
- una sola pàgina de resposta;
- un missatge d'error clar;
- una prova correcta i una incorrecta.

Frase guia: "No afegis més pantalles fins que pugues ensenyar una dada incorrecta bloquejada i una dada correcta acceptada."

## Ampliació per alumnat avançat

Si el mínim ja està tancat, l'alumnat pot:

- afegir una segona regla de validació coherent amb el domini;
- conservar el valor escrit perquè el reintent siga més còmode;
- separar una funció simple de validació;
- afegir una prova manual més precisa al `README`;
- preparar quina dada es processarà i guardarà en `MP2`.

L'ampliació no ha d'obrir encara autenticació, rols ni arquitectura completa.

## Checklist de tancament

- [ ] He triat una acció real del meu producte.
- [ ] El formulari envia dades al servidor.
- [ ] Puc assenyalar on recupere la dada en `PHP`.
- [ ] Hi ha almenys una validació en servidor.
- [ ] He provat un cas incorrecte.
- [ ] El cas incorrecte mostra un error útil.
- [ ] He provat el reintent amb una dada correcta.
- [ ] El `README`, issue o registre explica com repetir les proves.
- [ ] Si he usat IA, he registrat què m'ha aportat i què he verificat.

## Connexió amb MP2

`MP2` només té sentit si `MP1` deixa una dada correcta i validada. La pregunta de pas és:

Quina dada validada del teu producte es pot processar, guardar de manera simple i tornar a mostrar en la pròxima sessió?
