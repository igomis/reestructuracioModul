# MT05. Auth mínima defensable

Micro-presentació docent breu per a `R2S5-R2S6`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- auth no és el producte
- auth protegeix una operació real del producte
- cal demostrar cas permés i cas denegat

## Diapositiva 2. Tres preguntes

- qui eres?
- què vols fer?
- tens permís per fer-ho?

## Diapositiva 3. Mínim defensable

- login o mecanisme equivalent
- usuari o rol identificable
- ruta o acció protegida
- resposta quan no hi ha sessió
- resposta quan no hi ha permís

## Diapositiva 4. Errors habituals

- protegir una pantalla decorativa
- no comprovar permisos en servidor
- confondre autenticació i autorització
- provar només amb l'usuari correcte
- no documentar dades demo

## Diapositiva 5. Evidència del dia

- acció real protegida
- prova amb usuari autoritzat
- prova sense sessió o sense permís
- codi localitzat on es comprova l'accés
- nota al README

## Diapositiva 6. Tancament

- si no pots ensenyar el cas denegat, la protecció és feble
- la defensa ha d'arribar fins al punt exacte del codi
- pregunta final: què impedix ara el teu backend que abans no impedia?
