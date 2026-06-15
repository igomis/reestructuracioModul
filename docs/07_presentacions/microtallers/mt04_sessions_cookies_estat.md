# MT04. Sessió, cookies i estat

Micro-presentació docent breu per a `R2S4`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- no tot el que recorda l'aplicació és persistència del domini
- sessió i cookies resolen estat temporal
- la base de dades resol fets del producte

## Diapositiva 2. Què pot anar en sessió

- usuari autenticat
- missatges temporals
- pas actual d'un flux curt
- dades provisionals amb vida limitada
- preferències temporals no crítiques

## Diapositiva 3. Què no convé guardar

- contrasenyes
- decisions permanents del domini
- informació sensible innecessària
- estat que ha de sobreviure a tancament de sessió
- dades que han d'estar auditades

## Diapositiva 4. Cookies

- poden identificar una sessió
- poden guardar preferències simples
- poden ser manipulades si no es protegeixen
- no són una base de dades
- han de tindre abast i duració raonables

## Diapositiva 5. Evidència del dia

- llista de dades temporals i permanents
- decisió sobre sessió, cookie o base de dades
- prova d'inici i tancament de sessió
- prova de comportament sense sessió

## Diapositiva 6. Tancament

- el criteri és vida útil, sensibilitat i responsabilitat
- no guardes en sessió el que després hauràs de defensar com a fet del domini
- pregunta final: què recorda el teu backend i durant quant de temps?
