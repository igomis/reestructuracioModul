# R2S2. Processament i guardat funcional

## Finalitat de la sessió

Esta sessió continua el microrepte `R2M1`: una vegada el formulari ja envia dades i almenys una dada clau queda validada en servidor, l'alumnat ha de convertir eixa informació correcta en una resposta útil del producte.

El focus no és encara construir una arquitectura de persistència, ni introduir arrays i funcions com a contingut central. El focus és entendre el processament bàsic en servidor: variables, operadors, sentències simples, resposta generada, guardat funcional controlat i reutilització posterior de la dada.

Al final de la sessió, cada alumne o parella ha de poder demostrar que una dada vàlida entra pel flux, es tracta en el backend, queda guardada de manera simple i torna a aparéixer en una pantalla, llista o resposta posterior.

## Encaix dins del Repte 2

- **Repte**: `R2. Processament bàsic, estat, autenticació i primera funcionalitat protegida`
- **Microrepte**: `R2M2`
- **Sessió**: `R2S2`
- **Duració orientativa**: `3 hores`
- **Focus**: processament de dades ja validades, resposta generada en servidor, variables i operadors amb sentit, guardat funcional simple i reutilització visible
- **No entra encara**: arrays i funcions com a focus principal, regles de domini complexes, sessió, cookies, login, rols, arquitectura MVC o persistència formal

## Relació amb RA i criteris de treball

| Element | Concreció en el microrepte |
|---|---|
| `RA2` | generació de resposta amb codi de servidor, ús de sintaxi, variables, operadors, sentències simples, directives i àmbits bàsics |
| `RA3` | continuïtat del flux iniciat en `R2M1`, només amb dades que ja han superat la validació bàsica |
| Evidència central | dada correcta processada, guardada funcionalment i reutilitzada dins del projecte |
| Verificació docent | execució d'un cas vàlid complet i pregunta sobre què es guarda, on es guarda i on es torna a usar |

## Producte esperat

Una evolució del flux de `R2M1` que incloga, com a mínim:

- ús d'una dada validada del formulari anterior;
- separació recognoscible entre dada rebuda, dada neta i resultat generat;
- alguna transformació, càlcul, normalització o composició de resposta amb sentit dins del domini;
- resposta generada en servidor a partir de les dades;
- guardat funcional simple de la informació correcta;
- reutilització posterior de la dada guardada en una llista, pantalla, resum o resposta equivalent;
- nota breu al `README`, issue o registre indicant com provar el recorregut complet.

Mecanismes de guardat assumibles:

- fitxer simple controlat;
- estructura temporal del projecte si ja existix;
- emmagatzematge mínim facilitat pel docent;
- base de dades només si ja està preparada i no desplaça el focus de la sessió.

## Preparació prèvia del professorat

Abans de la sessió convé tindre preparat:

- un exemple curt on una dada validada es transforma i es mostra;
- una opció de guardat funcional simple;
- un exemple de reutilització visible posterior;
- una pauta per evitar guardar dades quan la validació falla;
- un criteri clar de tancament: no compta guardar si la informació no torna a usar-se.

## Seqüència d'aula de 3 hores

### 0:00-0:20. Recuperació de R2M1

El professorat demana executar el formulari de la sessió anterior amb un cas vàlid.

Tasques:

- identificar quina dada validada passa a processament;
- localitzar en el codi on es valida;
- decidir què no s'ha de guardar si la validació falla;
- descriure quina resposta útil generarà el backend.

Resultat del tram: cada equip sap quina dada correcta processarà i per a què servirà.

### 0:20-0:45. Modelatge docent

El professorat mostra un flux mínim:

- recuperació de la dada ja validada;
- normalització o transformació simple;
- ús de variables i operadors amb efecte visible;
- resposta generada amb codi de servidor;
- guardat funcional simple;
- recuperació posterior de la dada.

Resultat del tram: l'alumnat veu que processar no és només imprimir `$_POST`, sinó convertir una entrada correcta en una eixida útil del producte.

### 0:45-1:30. Processament de l'alumnat

L'alumnat implementa una primera transformació o composició.

Tasques:

- crear variables amb noms clars;
- aplicar una transformació, càlcul o normalització simple;
- mostrar una resposta generada a partir de la dada;
- comprovar que la resposta canvia quan canvia l'entrada;
- mantindre la validació de `R2M1` com a porta d'entrada.

Resultat del tram: hi ha processament observable i no només recepció de dades.

### 1:30-2:10. Guardat funcional

L'alumnat guarda només informació correcta.

Tasques:

- triar el mecanisme simple de guardat;
- guardar la dada processada o la dada neta necessària;
- evitar guardar dades quan el cas és invàlid;
- comprovar que el guardat és reproduïble;
- deixar anotat si el mecanisme és provisional per a `R2`.

Resultat del tram: una dada correcta queda conservada de manera controlada.

### 2:10-2:35. Reutilització

L'alumnat fa que la informació torne a aparéixer.

Tasques:

- mostrar una llista, resum, pantalla de detall o resposta equivalent;
- verificar que apareix la dada guardada;
- provar una nova entrada i comprovar que el resultat es reutilitza;
- revisar si s'està guardant informació innecessària.

Resultat del tram: el guardat té sentit funcional perquè la informació reapareix dins del producte.

### 2:35-2:50. Traçabilitat i documentació mínima

L'alumnat deixa rastre del recorregut.

Tasques:

- actualitzar el `README`, issue o registre de treball;
- escriure com provar el cas vàlid complet;
- indicar on es processa, on es guarda i on es reutilitza la dada;
- registrar limitacions del mecanisme triat.

Resultat del tram: una altra persona pot repetir el recorregut.

### 2:50-3:00. Checkpoint docent

Cada equip mostra:

- formulari o entrada amb dades vàlides;
- fragment on es processa la dada;
- lloc on queda guardada;
- pantalla o resposta on es reutilitza;
- nota de prova al repositori.

Pregunta de tancament: on es veu que la dada validada no només s'ha rebut, sinó que s'ha processat, guardat i reutilitzat?

## Tasques concretes de l'alumnat

- Executar el flux vàlid de `R2M1`.
- Triar una dada correcta per processar.
- Aplicar una transformació, càlcul, normalització o composició de resposta.
- Generar una eixida visible des del servidor.
- Guardar la informació correcta amb un mecanisme simple i controlat.
- Reutilitzar la dada guardada en una pantalla o resposta posterior.
- Documentar com provar el recorregut.

## Evidències mínimes

| Evidència | Mínim acceptable |
|---|---|
| Continuïtat amb `R2M1` | parteix d'una dada validada en servidor |
| Processament | hi ha variables, operadors o sentències simples amb efecte visible |
| Resposta generada | el servidor construeix una eixida a partir de les dades |
| Guardat funcional | la informació correcta queda conservada amb un mecanisme controlat |
| Reutilització | la dada torna a aparéixer en una pantalla, llista, resum o resposta |
| Documentació | el repositori explica com provar el cas complet |

## Criteris d'èxit

El microrepte està aconseguit si:

- el cas invàlid de `R2M1` no es guarda com si fora correcte;
- el processament modifica, prepara o usa la dada amb sentit;
- la resposta no és una maqueta fixa;
- el mecanisme de guardat és simple però explicable;
- la dada guardada es pot tornar a mostrar o usar;
- l'alumnat pot assenyalar el camí complet de la dada;
- la documentació permet repetir la prova.

## Què no és suficient

- Imprimir directament `$_POST` sense tractament.
- Guardar una dada que no ha passat la validació.
- Crear un fitxer, taula o registre que després no s'utilitza.
- Fer una persistència sofisticada mentre el flux bàsic no es pot explicar.
- Introduir arrays, funcions o classes com a obligació si encara no aporten claredat al cas.
- Fer login, sessió o rols abans de tindre una dada processada i reutilitzada.
- Dir que funciona sense ensenyar on es guarda i on reapareix la informació.

## Ús de la IA

La IA es pot usar per:

- proposar una transformació simple de dades;
- revisar sintaxi de `PHP`;
- comparar mecanismes senzills de guardat;
- ajudar a redactar la prova del `README`;
- suggerir una manera de mostrar la dada reutilitzada.

Control obligatori:

- l'alumnat ha de poder canviar una variable o operador i explicar l'efecte;
- ha de provar una dada nova, no només l'exemple generat;
- ha de justificar per què el mecanisme de guardat és suficient per a esta sessió;
- si la IA ha generat codi rellevant, s'ha de registrar breument al `AI log` o registre equivalent.

## Suport per alumnat amb més dificultat

Reduir el flux a:

- una dada validada de `R2M1`;
- una transformació simple, com normalitzar text, calcular una etiqueta o construir un resum;
- un guardat en fitxer o mecanisme facilitat pel docent;
- una pantalla que torne a mostrar eixa dada;
- una prova documentada.

Frase guia: "No afegis cap regla nova fins que pugues mostrar una dada correcta que entra, es processa, es guarda i torna a aparéixer."

## Ampliació per alumnat avançat

Si el mínim ja està tancat, l'alumnat pot:

- guardar més d'una dada coherent del formulari;
- afegir una llista simple de registres;
- preparar dades que després s'usaran en `R2M3`;
- validar i guardar un fitxer només si el cas d'ús ho justifica;
- documentar limitacions del mecanisme de guardat triat;
- començar a detectar duplicacions per a la refactorització de `R2M7`.

L'ampliació no ha d'obrir encara estat, autenticació ni arquitectura completa.

## Checklist de tancament

- [ ] He reutilitzat una dada validada de `R2M1`.
- [ ] Puc explicar què passa si la validació falla.
- [ ] He processat la dada amb codi de servidor.
- [ ] La resposta generada depén de la dada rebuda.
- [ ] He guardat només informació correcta.
- [ ] Puc assenyalar el mecanisme de guardat.
- [ ] La informació guardada torna a aparéixer en el projecte.
- [ ] El `README`, issue o registre explica com provar el recorregut.
- [ ] Si he usat IA, he registrat què m'ha aportat i què he verificat.

## Connexió amb R2M3

`R2M3` només té sentit si `R2M2` deixa informació correcta disponible. La pregunta de pas és:

Quina regla del teu projecte podrà aplicar el backend sobre la informació que ara ja està processada, guardada i reutilitzable?
