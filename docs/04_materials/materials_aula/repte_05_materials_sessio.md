# Materials de sessió del Repte 5

## Finalitat del document
Contextualitzar les plantilles d'aula del curs per al `R5`, de manera que el professorat puga conduir una integració o automatització amb valor real del producte, sense reduir el repte a “usar `n8n`” o a fer un workflow decoratiu.

## Mini-briefings de les sessions clau
### Sessió clau 1. Decisió d'integració
- Objectiu de la sessió: decidir quina necessitat real del producte es resoldrà amb integració o flux híbrid
- Què s'espera al final: integració justificada i flux d'entrada/eixida definit
- Error habitual a evitar: triar ferramenta o connector abans de tindre el cas d'ús
- Evidència mínima del dia: esquema funcional del flux híbrid
- Pregunta de tancament: quin problema real del producte resol esta integració?

### Sessió clau 2. Implementació del flux híbrid
- Objectiu de la sessió: posar en marxa el recorregut principal de la integració
- Què s'espera al final: workflow o integració executant una acció amb valor real
- Error habitual a evitar: automatització que no es pot explicar ni mantenir
- Evidència mínima del dia: flux parcial executable
- Pregunta de tancament: què entra, què ix i què es transforma en el vostre workflow?

### Sessió clau 3. Tancament i defensa
- Objectiu de la sessió: provar el flux complet, registrar incidències i preparar defensa final
- Què s'espera al final: integració de punta a punta, documentada i defensable
- Error habitual a evitar: arribar a la defensa amb workflow només aparent
- Evidència mínima del dia: prova del flux complet + documentació final
- Pregunta de tancament: si el flux fallara demà, sabríeu explicar on i per què?

## Checkpoints curts específics
- `CP-R5.1`
  - Què hauria d'estar fet: integració triada i justificada
  - Com es verifica en `2-3` minuts: mostrar entrada, eixida i valor funcional del flux
  - Senyal d'alerta: hi ha eina, però no necessitat real del producte
  - Acció correctiva ràpida: reduir el flux a un únic recorregut amb sentit
- `CP-R5.2`
  - Què hauria d'estar fet: workflow o integració parcial executable
  - Com es verifica en `2-3` minuts: llançar el flux i observar-ne un resultat útil
  - Senyal d'alerta: el grup descriu el procés, però no l'ensenya en funcionament
  - Acció correctiva ràpida: eliminar passos laterals i estabilitzar el recorregut principal
- `CP-R5.3`
  - Què hauria d'estar fet: prova final, errors mínims i documentació de tancament
  - Com es verifica en `2-3` minuts: repetir el flux complet i mostrar què passa si falla
  - Senyal d'alerta: hi ha automatització, però no control mínim d'incidència ni defensa clara
  - Acció correctiva ràpida: tancar una sola prova de punta a punta i documentar-la

## Exemples de feedback ràpid
- Vas bé: `La integració ja resol un problema real del producte. Ara tanca prova completa, incidències i defensa.`
- Cal corregir abans de seguir: `No pots donar per tancat R5 si encara no pots reproduir el flux complet davant del professorat.`
- Tens funcionalitat però falta verificació: `El workflow corre, però encara no hi ha prova clara del recorregut complet ni registre d'errors.`
- Tens solució massa superficial: `Has usat n8n o una integració externa, però encara no puc veure quin valor real aporta al producte.`
- Tens marge per ampliar: `Si el flux principal ja està estable, pots reforçar traçabilitat, errors o qualitat de documentació del mateix recorregut.`

## Fulls de treball base contextualitzats
### Full 1. Disseny del flux híbrid
- Objectiu: decidir una integració amb sentit real
- Tasca: definir necessitat, entrada, eixida i eina o servei necessari
- Evidència a generar: esquema funcional del flux
- Validació mínima: es pot explicar què resol i per què és útil
- Ajuda si et bloqueges: torna al cas d'ús principal i elimina passos ornamentals
- Ampliació si acabes prompte: afina errors, traçabilitat o criteri de manteniment

### Full 2. Prova de punta a punta
- Objectiu: demostrar que la integració està viva i és defensable
- Tasca: executar el flux complet, registrar resultat i incidències bàsiques
- Evidència a generar: prova reproduïble + documentació final + nota d'incidències
- Validació mínima: el professorat pot veure l'entrada, el procés i l'eixida
- Ajuda si et bloqueges: estabilitza només el recorregut principal i retalla passos secundaris
- Ampliació si acabes prompte: reforça control d'errors o defensa tècnica del flux

## Suport per alumnat endarrerit
- treballar amb un únic flux híbrid de punta a punta
- no afegir passos addicionals si encara no hi ha un recorregut clar i estable
- revisar primer prova, documentació i incidències abans de refinar l'automatització
- prioritzar defensa del que realment funciona

## Ampliacions per alumnat avançat
- millor control d'errors o branques d'incidència del mateix flux
- millor traçabilitat del recorregut
- segon pas justificat dins de la mateixa necessitat funcional, si el flux principal ja està tancat

## Evidència mínima per tram
- Tram inicial: integració justificada i dissenyada
- Tram funcional: workflow o integració parcial executable
- Tram de tancament: prova completa, documentació final i defensa preparada

## Connexió amb el repte següent
El `R5` no obri un repte tècnic nou, sinó el tancament del producte i la seua defensa. Si este repte queda superficial, la defensa final serà només discursiva i no una comprovació real del producte construït.
