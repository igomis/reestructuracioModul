# R2S10. Taller de contracte d'autenticacio per a DWEC

## Finalitat de la sessio

Esta sessio és un taller intermodular associat a `R2M6`. No crea un microrepte nou: reforça que la mini API d'autenticació siga realment consumible pel mòdul de `Desenvolupament Web en Entorn Client`.

El focus no és programar el client. El focus de `DWES` és publicar un contracte backend clar, estable i verificable perquè `DWEC` puga implementar el consum amb `fetch` sense haver d'endevinar formats, codis, headers o dades de prova.

## Encaix dins del Repte 2

- **Repte**: `R2. Processament bàsic, estat, autenticació i primera funcionalitat protegida`
- **Sessio**: `R2S10`
- **Tipus**: taller obligatori de reforç associat a `R2M6`
- **Duracio orientativa**: `3 hores`
- **Focus**: contracte d'autenticació consumible per DWEC, normalització de respostes, headers, dades demo i prova creuada mínima
- **No entra encara**: construir la interfície de client, dissenyar pantalles, gestionar estat visual, fer una API completa, OpenAPI, OAuth, JWT professional o refresh tokens

## Relacio amb `R2M6`

`R2M6` respon a esta pregunta:

> El backend ofereix una mini API d'autenticació correcta?

Este taller respon a esta altra:

> Una altra persona pot consumir eixa autenticació sense preguntar al grup com funciona?

Per això, el taller es valora dins de `R2M6`, especialment en la dimensió de contracte per a `DWEC`.

## Producte esperat

Cada equip ha de deixar un document curt, per exemple:

```text
docs/api-auth-contract.md
```

El document ha d'incloure:

- URL base;
- endpoint de login;
- endpoint protegit;
- mètodes HTTP;
- headers necessaris;
- body esperat;
- resposta `200`;
- resposta `401`;
- resposta d'error de validació si s'usa;
- usuari demo i contrasenya demo;
- exemple de token o explicació del format;
- limitacions conegudes;
- indicació de CORS si afecta el consum des de client.

## Preparacio previa del professorat

Convé preparar:

- plantilla de contracte `api-auth-contract.md`;
- exemple de contracte bo i contracte ambigu;
- acord mínim amb el professorat de `DWEC`;
- criteri sobre URL base i ports locals;
- criteri sobre CORS si els mòduls treballen en orígens diferents;
- exemple de petició/resposta final amb `curl` o Postman.

## Seqüencia d'aula de 3 hores

### 0:00-0:20. Model docent del contracte

El professorat mostra:

- què és un contracte consumible;
- diferència entre “funciona en el meu backend” i “un client pot usar-ho”;
- exemple de resposta ambigua;
- exemple de resposta estable.

Resultat: l'alumnat sap què ha de publicar, no només què ha programat.

### 0:20-0:45. Inventari d'endpoints reals

Tasques de l'alumnat:

- identificar URL real de `POST /api/login` o equivalent;
- identificar URL real de `GET /api/me` o equivalent;
- confirmar mètodes HTTP;
- confirmar quin header s'usa per al token;
- anotar quines dades entren i quines ixen.

Resultat: cada equip té una primera taula d'endpoints.

### 0:45-1:15. Normalitzacio de respostes

Tasques:

- revisar que el cas correcte retorna `JSON` estable;
- revisar que el cas incorrecte retorna `401`;
- revisar que els errors siguen interpretables;
- eliminar contrasenyes, hashes o dades internes de la resposta;
- decidir noms de camps estables.

Resultat: el client pot interpretar la resposta sense llegir el codi PHP.

### 1:15-1:45. Headers, dades demo i CORS si cal

Tasques:

- documentar `Content-Type`;
- documentar `Authorization: Bearer ...` o mecanisme equivalent;
- preparar usuari demo i contrasenya demo;
- comprovar si un client en un altre origen necessitarà CORS;
- documentar limitacions si encara no es resol CORS.

Resultat: DWEC rep dades de prova i regles de connexió clares.

### 1:45-2:20. Contracte escrit

Tasques:

- crear o actualitzar `docs/api-auth-contract.md`;
- incloure exemples complets de petició i resposta;
- escriure què ha de fer el client davant `401`;
- indicar què és provisional fins a `R4`.

Resultat: el contracte queda en el repositori.

### 2:20-2:45. Prova creuada mínima

Tasques:

- un altre equip o el professorat llig el contracte sense mirar el codi;
- executa una petició de login;
- executa una ruta protegida;
- registra friccions o ambigüitats.

Resultat: el contracte es valida com a document consumible.

### 2:45-3:00. Tancament

Tasques:

- corregir una ambigüitat detectada;
- deixar evidència final;
- anotar incidències pendents per a `R4`;
- confirmar què s'entrega a `DWEC`.

Pregunta de checkpoint: si demà una persona de `DWEC` vol consumir la teua API, què necessita saber i on ho trobarà?

## Evidencies minimes

| Evidencia | Minim acceptable |
|---|---|
| Contracte | `docs/api-auth-contract.md` o equivalent |
| Endpoints | URL, mètode i finalitat de login i ruta protegida |
| Headers | `Content-Type` i `Authorization` o alternativa documentada |
| Respostes | exemples de `200`, `401` i error de validació si toca |
| Dades demo | usuari i contrasenya de prova no sensibles |
| Prova creuada | validació per professorat o altre equip sense mirar el codi |
| Limitacions | CORS, tokens provisionals o altres deutes explicats |

## Criteris d'exit

- El contracte permet consumir la mini API sense preguntar al grup.
- Les respostes són estables i coherents.
- El client pot distingir cas correcte, no autenticat i error de validació.
- Les dades demo no són credencials personals reals.
- Les limitacions queden escrites.
- El taller millora `R2M6` sense convertir-se en treball propi de `DWEC`.

## Que no és suficient

- Dir oralment les URL però no documentar-les.
- Posar captures sense format de petició i resposta.
- Documentar només el cas correcte.
- No indicar headers.
- No deixar usuari demo.
- Fer un client complet i no corregir el contracte backend.

## Valoracio

El taller no té nota separada. Es valora dins de `R2M6`, especialment en la dimensió **contracte per a DWEC**.

Regla docent recomanada:

> Sense contracte mínim documentat per a `DWEC`, `R2M6` no pot superar el `8`.

## Connexio amb DWEC i R4

`DWEC` implementarà el client, el formulari, el `fetch`, el guardat del token en el client i la gestió visual dels errors. `DWES` ha de deixar el backend i el contracte preparats.

En `R4`, este contracte mínim es convertirà en treball d'API més formal: endpoints, contracte ampliat, protecció, documentació i consum complet.
