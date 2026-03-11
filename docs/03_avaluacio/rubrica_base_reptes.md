# Rúbrica base de reptes del mòdul DWES

## Finalitat del document
Disposar d’una rúbrica base reutilitzable per avaluar de manera coherent tots els reptes del mòdul DWES, garantint alineació amb els resultats d’aprenentatge, amb l’entorn professional backend i amb un model d’evidències autèntiques i verificables.

## Criteris generals d’ús
- esta rúbrica és el marc comú per als reptes 1-5 i s’aplica amb adaptacions menors segons el repte
- totes les dimensions s’han d’avaluar amb evidències observables del repositori i del producte
- la qualificació no es basa només en el resultat final, sinó en el procés tècnic i la traçabilitat
- el pes orientatiu pot ajustar-se lleugerament per repte, però sense eliminar dimensions
- la verificació d’autoria, comprensió i ús adequat de la IA és obligatòria

## Dimensions comunes d’avaluació
1. Comprensió tècnica i justificació de decisions.
2. Producte funcional i adequació al repte.
3. Qualitat del codi i estructura.
4. Testing, debugging i validació.
5. Documentació tècnica.
6. Ús de Git i traça del procés.
7. Ús verificable de la IA.
8. Defensa tècnica i autoria.

## Nivells de domini
- **Excel·lent:** domini alt, decisions sòlides i execució consistent.
- **Adequat:** assoliment correcte dels objectius amb limitacions menors.
- **En desenvolupament:** assoliment parcial amb mancances rellevants de qualitat o justificació.
- **Insuficient:** no arriba als mínims del repte o no es pot verificar comprensió/autoria.

## Taula de rúbrica

| Dimensió | Pes orientatiu | Excel·lent | Adequat | En desenvolupament | Insuficient | Evidències associades |
|---|---:|---|---|---|---|---|
| Comprensió tècnica i justificació de decisions | 15% | Explica decisions, alternatives i impacte tècnic amb criteri professional. | Explica decisions principals amb justificació suficient. | Justificació parcial o superficial, amb dubtes en decisions clau. | No pot justificar decisions tècniques bàsiques. | Defensa tècnica, ADR/notes de decisió, coherència entre explicació i codi. |
| Producte funcional i adequació al repte | 20% | Solució completa, estable i ajustada als requisits del repte. | Solució funcional amb incidències menors no crítiques. | Solució parcial o amb errors recurrents de funcionament. | Solució no funcional o desalineada amb l’encàrrec. | Execució del producte, demostració funcional, compliment de requisits del repte. |
| Qualitat del codi i estructura | 15% | Codi net, modular, coherent i fàcil de mantenir. | Codi correcte amb alguns punts de millora estructural. | Codi irregular, amb deute tècnic i estructura feble. | Codi desordenat o difícilment mantenible. | Repositori, estructura de carpetes, revisió de codi, convencions de projecte. |
| Testing, debugging i validació | 10% | Proves rellevants i registre de debugging amb correccions justificades. | Proves bàsiques i depuració amb evidències suficients. | Proves insuficients i depuració reactiva o poc traçada. | Absència de proves útils o de validació tècnica. | Tests executats, logs/incidències, registre de correccions, evidències de validació. |
| Documentació tècnica | 10% | Documentació completa, executable i alineada amb l’estat real del projecte. | Documentació suficient per entendre i executar el lliurable. | Documentació incompleta o amb llacunes operatives. | Documentació absent, desactualitzada o no fiable. | README, ADR, documentació API, instruccions de desplegament/execució. |
| Ús de Git i traça del procés | 10% | Historial clar i traçable: commits útils, branques i issues ben gestionades. | Historial usable amb traçabilitat general correcta. | Traçabilitat parcial (commits pobres o ús limitat d’issues/branques). | Historial caòtic o no verificable. | Commits, branques, pull requests (si escau), issues i enllaç amb microtasques. |
| Ús verificable de la IA | 10% | IA utilitzada amb criteri, AI log complet i validació tècnica demostrada. | IA utilitzada de manera acceptable amb evidències de verificació. | IA amb control limitat o justificació feble de decisions. | Delegació excessiva o incoherència entre ús declarat i resultat. | AI log, justificació de canvis, proves post-IA, coherència amb defensa tècnica. |
| Defensa tècnica i autoria | 10% | Defensa precisa i autònoma, alineada amb evidències del repositori. | Defensa correcta amb dubtes puntuals no crítics. | Defensa parcial, amb inseguretats en parts importants. | No pot defensar el treball ni demostrar autoria efectiva. | Defensa oral/escrita, respostes a preguntes tècniques, microcanvis en directe. |

## Evidències observables
Per aplicar la rúbrica, cal recollir evidències mínimes en cada repte:
- codi i estructura del projecte
- historial Git (commits, branques, issues i/o PR)
- proves i registres de debugging/validació
- documentació tècnica (README, ADR, API docs, etc.)
- AI log i justificació de decisions quan hi ha ús de IA
- defensa tècnica final (individual o d’equip amb contrast individual)

## Nota específica sobre ús verificable de la IA
La IA és una eina habitual i admesa en el mòdul, però la qualificació depén de la verificació del resultat:
- l’alumnat ha de comprendre i poder modificar el codi que entrega
- tota aportació de IA s’ha de validar amb proves o execució real
- la coherència entre AI log, repositori, documentació i defensa és obligatòria
- la delegació no verificable penalitza directament comprensió tècnica, ús de IA i defensa

## Criteris d’adaptació a cada repte
- **Repte 1 (kickoff backend):** augmentar pes de comprensió tècnica, documentació i Git; evidències clau: README, ADR i validació inicial.
- **Repte 2 (sessions i autenticació):** augmentar pes de producte funcional i qualitat del codi; reforçar seguretat i control d’estat.
- **Repte 3 (MVC i persistència):** reforçar qualitat del codi, testing/debugging i estructura; evidències clau: refactorització i persistència segura.
- **Repte 4 (API i consum):** reforçar producte funcional, documentació tècnica i validació; evidències clau: contracte d’API, proves d’endpoints i consum.
- **Repte 5 (integració híbrida i manteniment):** reforçar defensa tècnica, ús verificable de IA i mantenibilitat global; evidències clau: integració externa, traçabilitat i justificació final.

## Definition of done del document
Esta rúbrica base es considera completada quan:
- defineix dimensions comunes aplicables als reptes 1-5
- incorpora els quatre nivells de domini acordats
- relaciona cada dimensió amb evidències observables
- integra explícitament criteris de verificació de l’ús de la IA
- permet adaptació per repte sense perdre coherència curricular
