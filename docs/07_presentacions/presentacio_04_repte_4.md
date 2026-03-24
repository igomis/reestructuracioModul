# Presentació 04. Repte 4

Micro-presentació docent breu. Equival aproximadament a `8` diapositives.

## Diapositiva 1. Idea central
- `R4` convertix el backend en un servei publicable i consumible
- no és obrir rutes perquè sí
- l'`API` ha d'exposar casos d'ús reals del producte

## Diapositiva 2. Què resol el repte
- endpoints prioritaris i no trivials
- contracte clar de petició i resposta
- documentació usable per tercers
- prova real de consum

## Diapositiva 3. Què no és suficient
- rutes soltes
- `Swagger` ornamental
- JSON sense valor funcional
- documentació que no coincideix amb el codi

## Diapositiva 4. Què modela el professorat
- un endpoint nuclear del producte
- un cas correcte i un cas d'error
- una prova curta i reproduïble de consum
- lectura del contracte d'`API`

## Diapositiva 5. Què construeix l'alumnat
- `API` coherent amb el seu producte
- validació d'entrada i codis d'estat justificables
- consum real des d'un client o script
- documentació tècnica operativa

## Diapositiva 6. Evidència mínima
- documentació d'`API`
- col·lecció de proves o script de consum
- casos correctes i incorrectes verificats
- traçabilitat del procés en repositori

## Diapositiva 7. Errors habituals
- fer una `API` ornamental
- oblidar autenticació o permisos
- no provar errors ni dades invàlides
- donar per bo un contracte que el consumidor no usa realment

## Diapositiva 8. Connexió amb `R5`
- `R5` reutilitza esta `API` dins d'un flux híbrid
- si el contracte no està clar, la integració final es trenca
- `R4` és la base directa del tancament integrat del curs
