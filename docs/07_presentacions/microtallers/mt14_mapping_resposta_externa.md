# MT14. Mapping de resposta externa

Micro-presentació docent breu per a `R5S3`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- consumir dades externes no és mostrar JSON cru
- el backend ha de traduir-les al seu domini
- el mapping dona valor a la integració

## Diapositiva 2. Què cal transformar

- noms de camps
- formats de data
- estats
- identificadors
- unitats
- errors o absències

## Diapositiva 3. Model propi

- què necessita el producte?
- quina dada externa és fiable?
- quina dada cal normalitzar?
- què es guarda?
- què només es mostra?

## Diapositiva 4. Errors habituals

- acoblar tota l'aplicació al format extern
- no tractar camps absents
- duplicar dades sense criteri
- perdre l'origen de la informació
- no provar resposta inesperada

## Diapositiva 5. Evidència del dia

- exemple de resposta externa
- taula de mapping
- transformació implementada o prototipada
- cas amb dada incompleta
- documentació de límits

## Diapositiva 6. Tancament

- el mapping és una decisió de domini
- si canvia la font externa, el producte no hauria d'enfonsar-se sencer
- pregunta final: quina dada externa es converteix en valor del teu producte?
