# MT10. Dissenyar endpoint abans de programar

Micro-presentació docent breu per a `R4S1`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- una API no és una col·lecció improvisada de rutes
- primer es dissenya el contracte
- després s'implementa i es prova

## Diapositiva 2. Contracte mínim

- recurs
- mètode HTTP
- URL
- paràmetres
- cos de petició
- resposta correcta
- errors possibles

## Diapositiva 3. Preguntes útils

- qui consumirà l'endpoint?
- quina operació del domini representa?
- què passa si falta una dada?
- què passa si no hi ha permís?
- quin estat HTTP té sentit?

## Diapositiva 4. Errors habituals

- programar primer i documentar després
- retornar qualsevol JSON sense criteri
- no diferenciar `400`, `401`, `403` i `404`
- exposar dades internes
- no provar peticions incorrectes

## Diapositiva 5. Evidència del dia

- fitxa de contracte abans del codi
- exemple de petició
- exemple de resposta
- dos errors previstos
- decisió sobre autenticació

## Diapositiva 6. Tancament

- una tercera persona hauria de poder consumir l'endpoint sense llegir el codi
- el contracte és una promesa tècnica
- pregunta final: què pot fer exactament este endpoint i què no?
