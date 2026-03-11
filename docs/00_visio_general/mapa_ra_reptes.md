# Mapa curricular RA -> reptes del mòdul DWES

## Finalitat del document
Este document relaciona els resultats d’aprenentatge (RA) del mòdul DWES amb la nova estructura per reptes per garantir una planificació docent coherent, avaluable i executable en context professional.

## Criteris de construcció del mapa
- tots els RA del currículum apareixen com a mínim amb un espai de treball principal
- la distribució segueix la seqüència real del curs per reptes (R1 -> R5)
- cada RA es vincula a evidències autèntiques i instruments d’avaluació verificables
- la reorganització és metodològica (ordre i context), no reductora de contingut curricular
- Git, debugging, testing, documentació i APIs apareixen com a pràctiques transversals

## Taula general de correspondència

| RA | Descripció resumida | Reptes on es treballa | Pes principal / transversal | Evidències principals | Instruments d’avaluació | Materials actuals associats |
|---|---|---|---|---|---|---|
| RA1 | Selecciona arquitectura i configura l’entorn de desenvolupament backend. | Repte 1 (principal), Repte 3 (reforç) | Principal en R1; transversal en R3 | ADR inicial, repositori base funcional, README tècnic de kickoff | Rúbrica de repte, checklist de repositori, defensa tècnica curta | Bloc 1 (arquitectures web) |
| RA2 | Desenvolupa lògica de servidor per a processar peticions i formularis. | Repte 2 (principal), Repte 3 (reforç) | Principal en R2; transversal en R3 | Casos d’ús implementats, validacions, proves funcionals bàsiques | Rúbrica de repte, revisió de codi, proves funcionals | Bloc 2 (PHP) |
| RA3 | Implementa gestió d’estat, sessions i autenticació d’usuaris. | Repte 2 (principal), Repte 5 (reforç) | Principal en R2; transversal en R5 | Flux complet registre/login/logout, control de sessió, incidències resoltes | Rúbrica de repte, checklist de seguretat, defensa tècnica | Bloc 2 (PHP) + reforç del bloc 5 (seguretat) |
| RA4 | Construeix funcionalitat web dinàmica orientada a necessitats reals. | Repte 2 (principal), Repte 4 (reforç) | Principal en R2; transversal en R4 | Històries d’usuari operatives, evidències d’execució, documentació de comportament | Rúbrica de repte, validació en directe, seguiment d’issues | Bloc 2 (PHP) |
| RA5 | Organitza el codi amb arquitectura MVC i criteris de mantenibilitat. | Repte 1 (inici), Repte 3 (principal), Repte 5 (consolidació) | Principal en R3; transversal en R1 i R5 | Refactorització per capes, estructura MVC, convencions de projecte | Rúbrica de repte, checklist de qualitat de codi, revisió tècnica | Bloc 1 + blocs 3 i 4 (Laravel MVC + dades) |
| RA6 | Gestiona persistència de dades i accés segur a base de dades. | Repte 3 (principal), Repte 4 (reforç) | Principal en R3; transversal en R4 | Model de dades, consultes segures, proves d’integració de persistència | Rúbrica de repte, proves d’integració, revisió de codi | Blocs 3 i 4 + blocs 6a/6b (APIs) |
| RA7 | Dissenya, publica i consumeix APIs documentades. | Repte 4 (principal), Repte 5 (consolidació) | Principal en R4; transversal en R5 | Endpoints documentats, col·lecció de proves API, client de consum | Rúbrica de repte, checklist d’API, demostració funcional | Blocs 6a i 6b (APIs) |
| RA8 | Aplica qualitat, seguretat, debugging i testing sobre el backend. | Repte 3 (part principal), Repte 5 (principal), reforç en R2 i R4 | Principal en R5; transversal en R2-R4 | Registre de debugging, proves de regressió, correccions de seguretat | Checklist de repositori, rúbrica de qualitat, defensa tècnica | Bloc 5 (seguretat i reactivitat) |
| RA9 | Integra serveis externs i automatitzacions en solucions híbrides. | Repte 5 (principal), Repte 4 (previ) | Principal en R5; transversal en R4 | Integració externa operativa, flux automatitzat, pla de manteniment | Rúbrica de repte final, demo tècnica, defensa individual | Bloc 7 (webs híbrides) + suport de blocs 6a/6b |

## RA principals per repte
- Repte 1: RA1, inici de RA5.
- Repte 2: RA2, RA3 i RA4.
- Repte 3: RA5, RA6 i part de RA8.
- Repte 4: RA7, amb reforç de RA6.
- Repte 5: RA8 i RA9, amb consolidació de RA5-RA7.

## RA transversals
Els RA5, RA6, RA7 i RA8 es treballen en més d’un repte perquè afecten decisions d’arquitectura, qualitat del codi, persistència, APIs i manteniment global del producte. Esta transversalitat reforça la progressió professional del curs.

## Integració de la IA dins del mapa d’evidències i verificació
La IA s’integra com a eina habitual de suport (comparativa de solucions, generació inicial de codi, debugging i documentació), però sempre amb verificació explícita:
- AI log mínim per repte quan hi ha ús de IA
- validació amb proves i execució real
- coherència entre commits, documentació i decisions tècniques
- defensa tècnica individual per confirmar comprensió i autoria efectiva

## Garantia de cobertura curricular
No es perd cap RA del currículum: els RA1-RA9 estan coberts en el conjunt dels 5 reptes, amb pes principal i espais transversals quan correspon.

La reorganització plantejada és metodològica i no reductora: reordena el treball perquè siga més contextualitzat i professional sense eliminar objectius curriculars.

L’avaluació es basa en evidències autèntiques i verificables (repositori, proves, documentació i defensa tècnica), incloent la verificació de l’ús de IA com a part del procés i no com a substitució del criteri docent.
