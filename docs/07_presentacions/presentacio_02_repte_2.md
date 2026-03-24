# Presentació 02. Repte 2

Micro-presentació docent breu. Equival aproximadament a `8` diapositives.

## Diapositiva 1. Idea central
- `R2` converteix la base tècnica en un primer flux autenticat del producte
- auth no és la finalitat del repte
- el centre és una funcionalitat real protegida

## Diapositiva 2. Què resol el repte
- alta o login funcional
- control de sessió o estat equivalent
- primera operació de negoci protegida
- primera regla de rol, permís o restricció

## Diapositiva 3. Què no és suficient
- registre, login i logout aïllats
- protegir una ruta decorativa
- no aplicar cap restricció real
- provar només el cas feliç

## Diapositiva 4. Què modela el professorat
- auth com a infraestructura al servei del producte
- un flux curt amb accés autoritzat i denegat
- validació mínima del costat servidor
- un error clar i visible

## Diapositiva 5. Què construeix l'alumnat
- mòdul funcional d'accés
- operació real del domini protegida
- una restricció de negoci o de rol
- documentació i verificació del flux

## Diapositiva 6. Evidència mínima
- demostració de login o accés equivalent
- prova d'un cas permés i un cas denegat
- commits i `README` actualitzats
- verificació de validacions i errors

## Diapositiva 7. Errors habituals
- deixar auth desacoblada del producte
- no distingir auth i autorització
- no provar credencials incorrectes o accessos sense permís
- voler obrir massa funcionalitats sense tancar el nucli

## Diapositiva 8. Connexió amb `R3`
- el flux que naix ací ha de continuar viu en `R3`
- `R3` no és començar de zero, sinó professionalitzar esta funcionalitat
- si `R2` és superficial, `R3` no tindrà un cas d'ús seriós per mantindre
