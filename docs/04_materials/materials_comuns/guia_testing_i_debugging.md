# Guia de testing i debugging

## Finalitat
Convertir proves, depuració i registre d'incidències en una pràctica habitual del mòdul, de manera que el repositori aporte evidències verificables de qualitat i manteniment.

## Contingut mínim operatiu
Cada repte ha de definir almenys un conjunt reduït de verificacions sobre els fluxos crítics del producte. No es demana cobertura massiva, sinó proves útils i reproduïbles.

Base mínima de treball:
- identificar els casos crítics del repte
- definir què s'ha de comprovar en cas correcte i en cas d'error
- executar proves automatitzades o verificacions funcionals registrades
- anotar incidències, hipòtesis i resultat de la correcció
- tornar a provar després de cada canvi rellevant

Registre mínim de debugging:
- error observat
- context o passos per reproduir-lo
- causa probable o hipòtesi
- canvi aplicat
- verificació posterior

## Checklist o punts clau
- hi ha almenys una verificació clara dels fluxos més importants
- els casos d'error tenen el mateix pes que els casos feliços
- les incidències rellevants deixen rastre al repositori o a la documentació tècnica
- una correcció va seguida d'una comprovació posterior
- el resultat final es pot revisar i reproduir

## Errors habituals o riscos
- provar només a ull i no deixar cap evidència del que s'ha validat
- corregir errors sense haver-los reproduït abans
- confondre una demo puntual amb una verificació real
- no revisar regressions després d'una correcció
