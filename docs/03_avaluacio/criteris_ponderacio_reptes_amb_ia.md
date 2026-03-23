# Criteris de ponderació dels reptes amb IA

## Finalitat del document
Fixar un model de ponderació coherent per avaluar els reptes del mòdul DWES en un context on la IA forma part normal del treball, però on la qualificació ha de continuar depenent del que l'alumnat és capaç de construir, verificar, explicar i defensar.

## Problema de la rúbrica tradicional en context amb IA
Una rúbrica tradicional massa centrada en qualitat formal del codi genera dos problemes:
- confon bon resultat docent amb bon acabat superficial de codi
- no dona prou pes a la verificació tècnica, la defensa, la traçabilitat i la capacitat de contrastar l'ús de la IA

En este context, el criteri principal no és si el codi "pareix" molt bo, sinó si el repte:
- està resolt funcionalment
- resol un cas d'ús professional mínim i no una tècnica aïllada
- queda validat amb proves o comprovacions
- és explicable i defensable
- mostra procés real i ús verificable de la IA

## Criteris que han de guanyar pes
- resolució funcional del repte com a cas d'ús professional mínim
- verificació tècnica, proves i validació
- defensa tècnica i autoria sobre el flux funcional complet
- ús verificable de la IA
- traçabilitat del procés

## Criteris que han de perdre pes
- qualitat del codi com a gran criteri diferencial
- valoració implícita del "codi bonic" per damunt del repte realment resolt
- penalització excessiva per imperfeccions estructurals que no comprometen funcionalitat, verificació ni defensa
- tolerància a solucions trivials, decoratives o massa simples només perquè "funcionen"

## Proposta de ponderació base
| Criteri | Pes base | Lectura docent |
|---|---:|---|
| Resolució funcional i adequació al repte | 25% | criteri principal: el repte ha de quedar resolt sobre un mínim professional no trivial |
| Verificació tècnica, proves i validació | 15% | el resultat s'ha de poder contrastar |
| Defensa tècnica i autoria | 15% | l'alumnat ha de poder explicar i defensar el flux funcional complet |
| Ús verificable de la IA | 15% | la IA només compta si està contrastada i traçada |
| Traçabilitat del procés i Git/GitHub | 10% | el procés ha de ser llegible i verificable |
| Comprensió tècnica i justificació | 10% | cal saber per què s'ha fet cada decisió clau |
| Documentació tècnica operativa | 5% | la documentació ha de servir per revisar el lliurable |
| Qualitat tècnica bàsica del codi i estructura | 5% | continua sent important, però no és el centre de la nota |

Lectura global:
- la qualitat del codi queda com a criteri de llindar i suport
- la nota principal es juga en funcionalitat, verificació, defensa, IA verificable i traçabilitat
- una resolució massa trivial o només decorativa no hauria d'arribar a nivell adequat encara que el codi semble correcte

## Llindar de no trivialitat
No es considera que un repte està ben resolt si es queda en alguna d'estes situacions:
- `R1`: triar stack o instal·lar framework sense primera peça funcional del producte
- `R2`: fer login o registre sense una funcionalitat de negoci autenticada
- `R3`: reorganitzar codi o persistència sense professionalitzar un cas d'ús real
- `R4`: exposar rutes o documentació sense contracte API realment consumit
- `R5`: construir una integració ornamental sense flux complet ni valor funcional

## Variacions segons tipus de repte
| Repte | Criteris que guanyen pes | Criteris que perden pes | Lectura operativa |
|---|---|---|---|
| **Repte 1** | traçabilitat, comprensió, documentació i primera funcionalitat real | qualitat del codi com a criteri central | importa més la posada en marxa professional amb una primera peça funcional que el refinament del codi |
| **Repte 2** | resolució funcional, validació, proves i defensa del flux de negoci | documentació extensa o refinament estructural prematur | cal demostrar funcionalitat autenticada real, no només login o esquelet |
| **Repte 3** | verificació tècnica, defensa, persistència contrastada | obsessió per neteja formal del codi | importa que l'arquitectura professionalitze un cas d'ús real i siga explicable |
| **Repte 4** | funcionalitat d'`API`, proves, documentació operativa | pes excessiu de decisions de disseny no visibles en el producte | el contracte d'`API` ha de coincidir amb el comportament real i amb un cas d'ús publicable |
| **Repte 5** | defensa, IA verificable, traçabilitat, prova de punta a punta | valoració cosmètica del resultat final | importa el tancament real, la integració útil i la capacitat de justificar-la |

## Definition of done del model d'avaluació
Este model es considera completat quan:
- deixa clar per què la rúbrica tradicional queda curta en context amb IA
- explicita quins criteris han de guanyar i perdre pes
- oferix una ponderació base usable per als reptes del mòdul
- permet variar el focus segons el tipus de repte sense perdre coherència global
- manté l'avaluació centrada en producte, verificació, defensa, autoria i procés
- deixa explícit que una solució trivial o només decorativa no és suficient encara que siga tècnicament aparent
