# R2S5. Autenticacio i funcionalitat protegida

## Finalitat de la sessio

Esta sessio connecta l'estat de `R2M4` amb una necessitat real del producte: una operacio que no pot executar qualsevol visitant. L'objectiu no és crear una pantalla de login decorativa, sinó demostrar identificacio, autenticacio i una restriccio funcional sobre una accio del domini.

Al final de la sessio, l'alumnat ha de poder mostrar un cas permés i un cas denegat, i assenyalar exactament on el servidor pren la decisio.

## Encaix dins del Repte 2

- **Repte**: `R2. Processament bàsic, estat, autenticació i primera funcionalitat protegida`
- **Microrepte**: `R2M5`
- **Sessio**: `R2S5`
- **Duracio orientativa**: `3 hores`
- **Focus**: login mínim, sessio autenticada, operacio protegida, cas autoritzat i cas denegat
- **No entra encara**: sistema complet de rols, recuperacio de contrasenya, registre públic, OAuth, JWT o arquitectura completa

## Relacio amb RA i criteris de treball

| Element | Concrecio en el microrepte |
|---|---|
| `RA4.d` | autenticacio funcional mínima |
| `RA4.e` | restriccio d'accés a una operacio real |
| Evidencia central | operacio protegida amb cas permés i denegat |
| Verificacio docent | execucio directa de la ruta o accio protegida i pregunta sobre el punt de control |

## Producte esperat

Una evolucio del flux que incloga:

- identificacio d'usuari amb formulari o mecanisme equivalent;
- comprovacio de credencials de prova amb mecanisme coherent per al nivell;
- guardat d'usuari autenticat en sessio o equivalent;
- logout o invalidacio;
- una operacio real del domini protegida;
- cas no autenticat denegat;
- cas autenticat permés;
- cas autenticat però no autoritzat si el projecte ja té rol, propietat o restriccio simple;
- documentacio d'usuaris de prova i casos.

## Preparacio previa del professorat

Convé preparar:

- exemple mínim de credencials de prova;
- esquema identificacio -> autenticacio -> autoritzacio;
- exemple de proteccio al servidor abans d'executar l'operacio;
- pauta per triar una operacio real, no una pàgina buida;
- recordatori de no guardar contrasenyes en clar com a pràctica definitiva.

## Seqüencia d'aula de 3 hores

### 0:00-0:25. Marc conceptual

Diferenciar:

- identificacio: l'usuari diu qui és;
- autenticacio: el sistema ho comprova;
- autoritzacio: el sistema decideix què pot fer;
- operacio protegida: accio real del producte sotmesa a restriccio.

Resultat: cada equip tria una operacio a protegir.

### 0:25-0:55. Modelatge docent

Mostrar:

- formulari de login;
- comprovacio de credencials de prova;
- sessio autenticada;
- proteccio d'una operacio;
- resposta denegada;
- logout.

Resultat: queda clar que el control ha d'estar en servidor.

### 0:55-1:40. Implementacio d'autenticacio

Tasques:

- crear o adaptar login;
- comprovar credencials;
- guardar usuari autenticat;
- mostrar error si fallen;
- implementar logout o invalidacio.

Resultat: hi ha sessio autenticada comprovable.

### 1:40-2:20. Proteccio d'una operacio real

Tasques:

- triar una accio del domini ja existent;
- impedir-la sense autenticacio;
- aplicar restriccio simple si hi ha rol o propietat;
- comprovar que no es pot saltar cridant directament la URL.

Resultat: l'operacio queda protegida al servidor.

### 2:20-2:45. Prova de casos

Casos mínims:

- usuari no autenticat intenta l'operacio;
- usuari autenticat executa l'operacio;
- logout i nou intent;
- usuari no autoritzat si aplica.

Resultat: hi ha cas permés i denegat reproduïbles.

### 2:45-3:00. Checkpoint docent

Cada equip mostra:

- login;
- sessio activa;
- operacio protegida;
- cas permés;
- cas denegat;
- codi on es comprova la restriccio.

Pregunta: quina operacio real queda protegida, qui pot executar-la i on ho decideix el servidor?

## Tasques concretes de l'alumnat

- Implementar login mínim.
- Comprovar credencials.
- Guardar usuari autenticat.
- Protegir una operacio real.
- Provar accés permés, denegat i logout.
- Documentar usuaris de prova i casos.

## Evidencies minimes

| Evidencia | Minim acceptable |
|---|---|
| Login | formulari o mecanisme funcional |
| Autenticacio | credencials comprovades en servidor |
| Sessio | usuari autenticat recuperable |
| Operacio protegida | accio real del domini |
| Denegacio | cas no autenticat bloquejat |
| Permís | cas autenticat permés |
| Documentacio | usuaris de prova i passos |

## Criteris d'exit

- El login no és només visual.
- La proteccio està en servidor.
- L'operacio protegida té valor dins del projecte.
- Hi ha cas permés i denegat.
- Logout o invalidacio funciona.
- L'alumnat diferencia autenticacio i autoritzacio.

## Que no és suficient

- Protegir només una pàgina buida.
- Ocultar un botó però deixar l'operacio executable.
- Fer login sense sessio o estat autenticat.
- No provar accés directe a la ruta.
- Confondre usuari autenticat amb usuari autoritzat.

## Us de la IA

La IA pot ajudar a revisar diferències conceptuals o detectar punts d'accés no protegits. Control: l'alumnat ha de fer una demo sense IA dels casos no autenticat, autenticat permés i logout.

## Suport per alumnat amb més dificultat

Usar dos usuaris de prova i una única operacio protegida. No afegir rols fins que el cas no autenticat i el cas autenticat funcionen.

## Ampliacio per alumnat avançat

- Restriccio per rol o propietari.
- Hashing de contrasenyes si el projecte ho permet.
- Missatges diferenciats d'autenticacio i autoritzacio.
- Proves manuals documentades amb més precisio.

## Checklist de tancament

- [ ] Tinc login funcional.
- [ ] Comprove credencials en servidor.
- [ ] Guarde usuari autenticat.
- [ ] He triat una operacio real.
- [ ] La bloquege sense autenticacio.
- [ ] La permeta amb autenticacio vàlida.
- [ ] He provat logout.
- [ ] He documentat usuaris i casos.

## Connexio amb R2M6

`R2M6` convertirà el flux complet en una bateria mínima de proves. La pregunta de pas és:

Quins casos demostren que el flux no és una demo puntual?

