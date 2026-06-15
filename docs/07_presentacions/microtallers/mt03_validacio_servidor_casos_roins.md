# MT03. Validació de servidor amb casos roïns

Micro-presentació docent breu per a `R2S1-R2S2`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- validar no és només comprovar que el cas bo entra
- el servidor ha de protegir el flux
- els errors també són part del producte

## Diapositiva 2. Casos que cal pensar

- camp buit
- format incorrecte
- valor fora de rang
- duplicat
- dada manipulada des del client
- operació fora d'estat

## Diapositiva 3. Validació útil

- regla visible en el servidor
- missatge comprensible
- dada bona conservada si té sentit
- dada roïna rebutjada
- resposta coherent per a usuari o API

## Diapositiva 4. Taula mínima

- entrada
- resultat esperat
- error esperat
- on es valida
- com es prova
- què queda registrat

## Diapositiva 5. Evidència del dia

- llista de casos vàlids i invàlids
- implementació d'almenys dues validacions
- prova manual o automatitzada
- README o nota tècnica curta

## Diapositiva 6. Tancament

- si només proves el cas feliç, no has provat el backend
- el client pot ajudar, però no substituïx el servidor
- pregunta final: quina entrada maliciosa o errònia bloqueja ara el teu projecte?
