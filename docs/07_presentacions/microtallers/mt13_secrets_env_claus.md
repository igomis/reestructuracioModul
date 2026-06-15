# MT13. Secrets, .env i claus

Micro-presentació docent breu per a `R5S2`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- una clau exposada és una incidència
- `.env` separa configuració i codi
- el repositori no ha de contindre secrets reals

## Diapositiva 2. Què és un secret

- contrasenya
- token d'API
- clau privada
- application password
- cadena de connexió sensible
- credencial de servei extern

## Diapositiva 3. Bones pràctiques mínimes

- `.env` fora de Git
- `.env.example` sense secrets
- variables amb noms clars
- error comprensible si falta configuració
- revocar claus exposades

## Diapositiva 4. Errors habituals

- commitejar `.env`
- posar tokens al README
- compartir captures amb claus
- usar claus personals per a demos
- no documentar com configurar l'entorn

## Diapositiva 5. Evidència del dia

- `.gitignore` revisat
- `.env.example` actualitzat
- lectura de configuració implementada
- prova sense clau
- instrucció segura en README

## Diapositiva 6. Tancament

- la integració ha de ser reproduïble sense exposar credencials
- una bona demo no justifica filtrar secrets
- pregunta final: què passaria si publiques ara el repositori?
