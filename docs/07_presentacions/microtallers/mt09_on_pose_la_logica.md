# MT09. On pose la lògica

Micro-presentació docent breu per a `R3S3-R3S4`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- la lògica no ha d'acabar tota en el controlador
- cada capa té una responsabilitat
- la decisió ha de poder defensar-se

## Diapositiva 2. Controlador

- rep la petició
- valida o delega validació
- crida el cas d'ús
- prepara la resposta
- no hauria de concentrar tota la regla de negoci

## Diapositiva 3. Servei o cas d'ús

- coordina operacions
- aplica regles del flux
- parla amb repositoris o models
- facilita proves
- fa visible la decisió de negoci

## Diapositiva 4. Model o entitat

- representa dades del domini
- pot protegir invariants simples
- no hauria de saber massa de la interfície
- ha de mantindre coherència interna

## Diapositiva 5. Evidència del dia

- una regla moguda al lloc adequat
- explicació curta de la decisió
- prova del flux després del canvi
- codi més localitzable

## Diapositiva 6. Tancament

- no busquem arquitectura perfecta, busquem responsabilitats clares
- si no saps on canviar una regla, l'estructura encara és confusa
- pregunta final: on canviaries esta regla si demà canviara el negoci?
