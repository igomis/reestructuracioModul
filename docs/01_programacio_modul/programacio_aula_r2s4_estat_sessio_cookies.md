# R2S4. Estat, sessio i cookies

## Finalitat de la sessio

Esta sessio introdueix el manteniment d'informacio temporal entre peticions. Després de rebre dades, conservar reintents, guardar funcionalment casos correctes i aplicar una regla del projecte, el backend ha de poder recordar una dada provisional del flux sense confondre-la amb persistencia del domini.

L'objectiu és que l'alumnat distingisca estat, sessio, cookie i guardat funcional, implemente un mecanisme real de recuperacio i demostre una invalidacio controlada.

## Encaix dins del Repte 2

- **Repte**: `R2. Processament bàsic, estat, autenticació i primera funcionalitat protegida`
- **Microrepte**: `R2M4`
- **Sessio**: `R2S4`
- **Duracio orientativa**: `3 hores`
- **Focus**: dada temporal, `$_SESSION` o cookie, recuperacio posterior i invalidacio
- **No entra encara**: login complet, rols, autoritzacio complexa, base de dades com a centre o arquitectura MVC

## Relacio amb RA i criteris de treball

| Element | Concrecio en el microrepte |
|---|---|
| `RA4.a` | identificacio de mecanismes per conservar informacio entre peticions |
| `RA4.b` | ús de sessio o mecanisme equivalent de servidor |
| `RA4.c` | ús o inspeccio de cookies o informacio en client quan tinga sentit |
| Evidencia central | dada temporal recuperable i invalidacio demostrada |
| Verificacio docent | execucio abans/després i pregunta sobre client, servidor i persistencia |

## Producte esperat

Una evolucio del flux que incloga, com a minim:

- una dada temporal amb sentit dins del producte;
- guardat en sessio o mecanisme equivalent;
- lectura de la dada en una peticio posterior;
- si s'usa cookie, explicacio de què queda en client;
- accio de neteja, reinici o invalidacio;
- demo abans/després de la invalidacio;
- nota al `README`, issue o registre explicant què es guarda, on i per què és temporal.

## Preparacio previa del professorat

Convé tindre preparat:

- exemple mínim de `session_start()`, escriptura, lectura i neteja;
- exemple visual de cookie de sessio en el navegador;
- comparacio entre estat temporal i guardat funcional;
- llista de dades que no s'han de posar en cookies sense criteri;
- pauta per triar una dada temporal menuda: pas del flux, últim filtre, esborrany, preferencia o resultat provisional.

## Seqüencia d'aula de 3 hores

### 0:00-0:25. Aclariment conceptual

El professorat separa quatre idees:

- estat: informacio que cal recordar durant un flux;
- sessio: estat associat a un client i guardat al servidor;
- cookie: dada en el navegador que pot identificar o recordar informacio limitada;
- persistencia: dada estable del domini.

Resultat: cada equip identifica una dada temporal candidata.

### 0:25-0:50. Modelatge docent

Mostrar:

- inici de sessio;
- guardat d'una dada;
- lectura en una altra peticio;
- inspeccio de cookie;
- neteja o destruccio de la dada.

Resultat: l'alumnat veu on viu cada part del mecanisme.

### 0:50-1:35. Implementacio d'estat temporal

Tasques:

- decidir què cal recordar temporalment;
- guardar-ho en sessio o cookie segons el cas;
- recuperar-ho en una pantalla posterior;
- evitar dades sensibles en cookies;
- mostrar una resposta clara quan la dada existeix.

Resultat: el flux recupera informacio entre peticions.

### 1:35-2:10. Invalidacio i comprovacio

Tasques:

- afegir accio de neteja, reinici o eixida del flux;
- comprovar què passa abans i després;
- revisar la cookie o l'estat visible;
- evitar que la dada temporal continue afectant el flux després de netejar-la.

Resultat: hi ha invalidacio controlada.

### 2:10-2:40. Contrast amb guardat funcional

Tasques:

- identificar què és temporal i què és dada del producte;
- explicar per què esta dada no substitueix la persistencia;
- ajustar noms i missatges si confonen.

Resultat: queda clara la frontera conceptual.

### 2:40-3:00. Checkpoint docent

Cada equip mostra:

- dada temporal guardada;
- recuperacio posterior;
- cookie o mecanisme observat si aplica;
- invalidacio;
- explicacio de què queda en client i servidor.

Pregunta: quina informacio recorda el sistema només durant el flux, on està guardada i quan s'invalida?

## Tasques concretes de l'alumnat

- Triar una dada temporal del flux.
- Guardar-la en sessio, cookie o mecanisme equivalent.
- Recuperar-la en una peticio posterior.
- Implementar invalidacio.
- Documentar què es guarda i què no és persistencia.

## Evidencies minimes

| Evidencia | Minim acceptable |
|---|---|
| Estat | dada temporal amb sentit dins del flux |
| Guardat | codi d'escriptura en sessio/cookie o equivalent |
| Recuperacio | lectura posterior demostrable |
| Invalidacio | accio que neteja o reinicia l'estat |
| Explicacio | frontera entre estat temporal i guardat funcional |
| Documentacio | instruccions per reproduir abans/després |

## Criteris d'exit

- La dada temporal no és decorativa.
- Es recupera en una peticio diferent.
- La invalidacio és comprovable.
- L'alumnat diferencia client, servidor i persistencia.
- No es guarden dades sensibles en cookies sense criteri.

## Que no és suficient

- Dir que hi ha sessio sense cap dada recuperable.
- Usar una variable normal que desapareix entre peticions.
- Guardar-ho tot en sessio com si fora base de dades.
- Posar contrasenyes, rols o dades sensibles en cookies sense justificacio.
- No tindre forma de netejar o invalidar.

## Us de la IA

La IA pot ajudar a comparar sessio i cookie, interpretar errors o redactar la prova. Control: l'alumnat ha de demostrar en execucio què es guarda, on es guarda i quan desapareix.

## Suport per alumnat amb més dificultat

Reduir-ho a una dada: últim nom introduït, pas actual o filtre simple. Guardar-la en sessio, mostrar-la en una altra pàgina i afegir un botó de neteja.

## Ampliacio per alumnat avançat

- Caducitat funcional d'una dada temporal.
- Preferencia simple en cookie no sensible.
- Missatge diferent si l'estat és invàlid.
- Taula de proves abans/després.

## Checklist de tancament

- [ ] He triat una dada temporal.
- [ ] La guarde en sessio, cookie o equivalent.
- [ ] La recupere en una peticio posterior.
- [ ] Puc explicar què queda en client i servidor.
- [ ] He implementat invalidacio.
- [ ] He documentat com provar-ho.

## Connexio amb R2M5

`R2M5` aprofitarà la idea d'estat per construir autenticacio funcional i protegir una operacio real. La pregunta de pas és:

Quina operacio del teu projecte necessita saber qui està actuant o si pot continuar?

