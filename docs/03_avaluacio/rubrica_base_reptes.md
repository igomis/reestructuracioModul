# Rúbrica base de reptes del mòdul DWES

## Finalitat del document
Disposar d'una rúbrica base reutilitzable per avaluar de manera coherent tots els reptes del mòdul DWES en un context on la IA és una eina normalitzada de treball i, per tant, el valor principal no recau en la "puresa" del codi, sinó en la capacitat de construir, verificar, traçar i defensar una solució funcional real.

## Problema de la rúbrica tradicional en context amb IA
En un context de treball amb IA, una rúbrica massa centrada en qualitat formal del codi genera dos distorsions:
- premia aparença estructural encara que el repte no estiga prou verificat, provat o defensat
- invisibilitza el valor real de la traçabilitat, la validació tècnica i la capacitat d'explicar què s'ha fet i per què

Per això, en este mòdul:
- la qualitat del codi continua sent important, però deixa de ser el criteri central
- la resolució funcional, la verificació tècnica, la defensa, l'ús verificable de la IA i la traçabilitat passen a ser criteris principals

## Criteris generals d'ús
- esta rúbrica és el marc comú per als reptes `1-5`
- totes les dimensions s'han d'avaluar amb evidències observables del producte, del repositori i de la defensa
- el pes pot ajustar-se lleugerament segons el repte, però la lògica general s'ha de mantindre
- una bona presentació no pot compensar l'absència de funcionalitat, proves o traçabilitat
- un codi formalment correcte no pot compensar manca de verificació, manca de comprensió o ús opac de la IA
- Git/GitHub es tracta com a metodologia de treball i criteri de traçabilitat, no com a iniciació des de zero

## Dimensions comunes d'avaluació
1. Resolució funcional i adequació al repte.
2. Verificació tècnica, proves i validació.
3. Defensa tècnica i autoria.
4. Ús verificable de la IA.
5. Traçabilitat del procés i Git/GitHub.
6. Comprensió tècnica i justificació de decisions.
7. Documentació tècnica operativa.
8. Qualitat tècnica bàsica del codi i estructura.

## Nivells de domini
- **Excel·lent:** resol el repte amb criteri alt, verificació sòlida i defensa consistent.
- **Adequat:** resol el nucli del repte amb mancances menors no crítiques.
- **En desenvolupament:** assolix només una part del repte o no el pot verificar i defensar amb solvència.
- **Insuficient:** no arriba als mínims funcionals, tècnics o d'autoria exigibles.

## Taula de rúbrica
| Dimensió | Pes base | Excel·lent | Adequat | En desenvolupament | Insuficient | Evidències associades |
|---|---:|---|---|---|---|---|
| Resolució funcional i adequació al repte | 25% | El repte queda resolt de manera funcional, estable i alineada amb l'encàrrec real. | El nucli funcional està resolt amb incidències menors no crítiques. | La solució és parcial, fràgil o només funciona en part dels casos previstos. | El repte no queda resolt o no es correspon amb l'encàrrec. | Demostració funcional, compliment de requisits, execució real del producte. |
| Verificació tècnica, proves i validació | 15% | Hi ha proves, comprovacions i validacions suficients per demostrar que el resultat és fiable. | Hi ha verificació bàsica i evidències tècniques suficients de funcionament. | La validació és escassa, reactiva o massa dependent de demostracions puntuals. | No hi ha proves útils ni verificació tècnica rellevant. | Tests, col·leccions de peticions, casos límit, registres de debugging i correccions. |
| Defensa tècnica i autoria | 15% | Explica amb precisió què ha fet, per què funciona, què ha fallat i com ho ha corregit. | Defensa el treball amb seguretat general i dubtes puntuals no crítics. | La defensa és parcial, superficial o insegura en parts rellevants. | No pot defensar el treball ni demostrar autoria efectiva. | Defensa oral o escrita, preguntes de contrast, microcanvis en directe, coherència amb el repositori. |
| Ús verificable de la IA | 15% | La IA s'ha utilitzat amb criteri, traça clara i validació tècnica posterior demostrable. | La IA s'ha utilitzat de forma acceptable i l'equip pot justificar què ha revisat i què ha descartat. | L'ús de la IA és poc clar, amb control feble o justificació insuficient. | Hi ha dependència opaca, manca de traça o incapacitat de verificar el resultat generat. | `AI log`, contrast posterior, proves post-IA, coherència entre explicació i resultat. |
| Traçabilitat del procés i Git/GitHub | 10% | El procés és clar, llegible i verificable: commits útils, evolució recognoscible i evidència de treball real. | La traça general és suficient per seguir el desenvolupament del repte. | La traçabilitat és irregular o incompleta. | El procés no és verificable o el repositori s'usa només com a contenidor final. | Historial Git, commits, branques si escau, relació amb microtasques, evolució del repositori. |
| Comprensió tècnica i justificació de decisions | 10% | Justifica decisions, alternatives i impacte tècnic amb criteri professional. | Justifica les decisions principals amb coherència suficient. | La justificació és superficial o no arriba a les decisions crítiques. | No pot explicar decisions bàsiques ni relació amb el repte. | Defensa, ADR o registre equivalent, explicació de decisions, coherència tècnica. |
| Documentació tècnica operativa | 5% | La documentació permet entendre, executar i revisar el lliurable sense contradiccions. | La documentació és usable i està alineada amb l'estat general del projecte. | La documentació és parcial o queda desactualitzada en punts rellevants. | La documentació és absent, poc fiable o inútil per revisar el treball. | `README`, ADR, documentació d'API, instruccions d'execució, notes tècniques. |
| Qualitat tècnica bàsica del codi i estructura | 5% | El codi manté un nivell sòlid de claredat, separació i mantenibilitat bàsica. | El codi és usable amb punts de millora clars però no crítics. | L'estructura és feble o amb deute tècnic que dificulta la revisió. | El codi és desordenat fins al punt d'impedir manteniment o verificació raonable. | Estructura del projecte, separació de responsabilitats, consistència mínima del codi. |

## Lectura dels pesos
- la resolució funcional, la verificació tècnica, la defensa, l'ús verificable de la IA i la traçabilitat sumen el nucli principal de la qualificació
- la qualitat del codi no desapareix, però passa a ser un criteri de suport i de llindar mínim, no el centre de la rúbrica
- la documentació continua sent obligatòria, però compta sobretot per la seua utilitat operativa i coherència amb el treball real

## Evidències observables
Per aplicar la rúbrica, cal recollir com a mínim:
- producte funcional o demostració reproduïble del repte
- proves, validacions o comprovacions tècniques
- historial del repositori i traçabilitat del procés
- documentació tècnica operativa
- `AI log` o evidència equivalent quan s'ha usat IA
- defensa tècnica del treball realitzat

## Nota específica sobre ús verificable de la IA
La IA és una eina admesa i habitual, però no és un criteri positiu per si sola. Només compta de manera favorable quan:
- queda clar què s'ha utilitzat i en quin moment
- el resultat s'ha contrastat amb proves, execució o revisió humana posterior
- l'alumnat pot explicar i modificar allò que entrega
- hi ha coherència entre `AI log`, repositori, evidències i defensa

## Criteris d'adaptació a cada repte
- **Repte 1:** augmentar lleugerament pes de traçabilitat, comprensió i documentació; el codi no ha de dominar l'avaluació.
- **Repte 2:** reforçar resolució funcional i verificació tècnica de fluxos, validacions i errors.
- **Repte 3:** reforçar verificació, defensa i qualitat tècnica bàsica del pas a arquitectura i persistència, sense convertir el codi en criteri principal.
- **Repte 4:** reforçar funcionalitat, proves i documentació d'`API`.
- **Repte 5:** reforçar defensa tècnica, ús verificable de la IA, traçabilitat i prova de punta a punta.

## Definition of done del document
Esta rúbrica base es considera completada quan:
- reequilibra el pes de l'avaluació per a un context de treball normalitzat amb IA
- redueix el protagonisme de la qualitat del codi com a criteri central
- augmenta el pes de resolució funcional, verificació, defensa, IA verificable i traçabilitat
- manté una estructura usable per als reptes `1-5`
- permet adaptacions per repte sense perdre coherència global
