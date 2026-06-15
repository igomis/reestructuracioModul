# MT07. Migrar un cas d'ús a framework

Micro-presentació docent breu per a `R3S1`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- migrar no és copiar carpetes
- el cas d'ús ha de continuar sent recognoscible
- el framework aporta estructura, no màgia

## Diapositiva 2. Què es conserva

- actor principal
- regla de negoci
- entrada i eixida
- cas d'error
- evidència de funcionament

## Diapositiva 3. Què canvia

- rutes
- controladors
- serveis o casos d'ús
- models o entitats
- configuració
- proves

## Diapositiva 4. Mapa de migració

- flux antic en PHP base
- punt d'entrada nou
- capa que processa
- capa que persisteix
- resposta final
- prova equivalent

## Diapositiva 5. Evidència del dia

- diagrama curt o taula de correspondència
- primer flux portat parcialment
- decisió d'estructura
- prova manual del punt d'entrada

## Diapositiva 6. Tancament

- el framework ha de fer més mantenible el mateix producte
- si no saps on ha anat el cas d'ús, has perdut traçabilitat
- pregunta final: quin flux de `R2` continua viu en `R3`?
