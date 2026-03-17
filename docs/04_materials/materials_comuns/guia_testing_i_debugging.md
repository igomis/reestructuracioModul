# Guia de testing i debugging

## Finalitat
Convertir proves, depuració i registre d'incidències en una pràctica habitual del mòdul, de manera que el repositori aporte evidències verificables de qualitat i manteniment.

Esta guia no demana sofisticació excessiva. El seu objectiu és que cada repte deixe una prova clara que l'equip sap comprovar el que construïx, reproduir errors i justificar correccions sense dependre només d'una demo o d'una explicació oral.

## Contingut mínim operatiu
Cada repte ha de definir almenys un conjunt reduït de verificacions sobre els fluxos crítics del producte. No es demana cobertura massiva, sinó proves útils i reproduïbles.

Base mínima de treball:
- identificar els casos crítics del repte
- definir què s'ha de comprovar en cas correcte i en cas d'error
- executar proves automatitzades o verificacions funcionals registrades
- anotar incidències, hipòtesis i resultat de la correcció
- tornar a provar després de cada canvi rellevant

Tipus mínims de comprovació que convé cobrir:
- cas correcte principal del repte
- almenys un cas d'error o dada invàlida
- comprovació posterior a una correcció rellevant
- comprovació de regressió quan un canvi toca una part sensible del producte

Registre mínim de debugging:
- error observat
- context o passos per reproduir-lo
- causa probable o hipòtesi
- canvi aplicat
- verificació posterior

Formats acceptables d'evidència:
- proves automatitzades del stack triat
- col·leccions de peticions o comprovacions manuals registrades
- registre curt d'incidències al `README`, en documentació tècnica o en la issue del repte

Criteri docent:
- importa més que la prova siga significativa i reproduïble que no la quantitat bruta de proves
- el debugging ha de mostrar procés, no només resultat final
- una incidència ben registrada té valor docent i professional, encara que la correcció siga menuda

## Checklist o punts clau
- hi ha almenys una verificació clara dels fluxos més importants
- els casos d'error tenen el mateix pes que els casos feliços
- les incidències rellevants deixen rastre al repositori o a la documentació tècnica
- una correcció va seguida d'una comprovació posterior
- el resultat final es pot revisar i reproduir
- el material de prova està alineat amb el repte i amb el producte real, no amb exemples desconnectats
- el registre de debugging permet entendre què fallava i com s'ha validat la correcció

## Errors habituals o riscos
- provar només a ull i no deixar cap evidència del que s'ha validat
- corregir errors sense haver-los reproduït abans
- confondre una demo puntual amb una verificació real
- no revisar regressions després d'una correcció
- acumular proves irrellevants i no comprovar precisament els punts crítics del repte
- usar la IA per generar proves aparentment correctes sense contrastar que corresponen al comportament real del projecte
