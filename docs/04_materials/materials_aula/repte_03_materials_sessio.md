# Materials de sessió del Repte 3

## Finalitat del document
Contextualitzar les plantilles d'aula del curs per al `R3`, de manera que el professorat puga professionalitzar una funcionalitat real del producte amb arquitectura i persistència, sense reduir el repte a “fer MVC” o “guardar dades”.

## Mini-briefings de les sessions clau
### Sessió clau 1. Què s'ha de refactoritzar
- Objectiu de la sessió: detectar quin flux de `R2` mereix passar a una estructura més mantingible
- Què s'espera al final: mapa bàsic de capes o equivalent i entitats principals
- Error habitual a evitar: reorganitzar carpetes sense millorar el flux real
- Evidència mínima del dia: cas d'ús triat i model mínim del domini
- Pregunta de tancament: quina part del vostre flux actual és la més fràgil o opaca?

### Sessió clau 2. Persistència funcional
- Objectiu de la sessió: fer persistent el flux principal del producte
- Què s'espera al final: primera entitat i operació principal persistides
- Error habitual a evitar: afegir base de dades però no integrar-la en el cas d'ús real
- Evidència mínima del dia: lectura o escriptura persistent reproduïble
- Pregunta de tancament: què passa ara amb les dades del vostre flux quan es torna a executar?

### Sessió clau 3. Regressió i tancament de `R3`
- Objectiu de la sessió: demostrar que la funcionalitat principal continua viva després de la refactorització
- Què s'espera al final: arquitectura explicable, persistència coherent i prova mínima del flux
- Error habitual a evitar: canviar estructura i perdre verificació
- Evidència mínima del dia: flux principal persistent + prova curta + `README` tècnic
- Pregunta de tancament: què podeu explicar ara millor del vostre producte que abans de `R3`?

## Checkpoints curts específics
- `CP-R3.1`
  - Què hauria d'estar fet: entitats i responsabilitats principals identificades
  - Com es verifica en `2-3` minuts: mostrar mapa curt de flux, model i punt d'entrada
  - Senyal d'alerta: hi ha diagrama o discurs, però no canvis recognoscibles al projecte
  - Acció correctiva ràpida: refactoritzar una sola operació del flux principal
- `CP-R3.2`
  - Què hauria d'estar fet: persistència real del cas d'ús central
  - Com es verifica en `2-3` minuts: crear o recuperar un registre real del domini
  - Senyal d'alerta: persistència parcial o només per a demo
  - Acció correctiva ràpida: tancar només una entitat i una operació completa
- `CP-R3.3`
  - Què hauria d'estar fet: regressió mínima controlada
  - Com es verifica en `2-3` minuts: repetir el flux principal i comparar resultat
  - Senyal d'alerta: el grup diu que “ha millorat”, però no pot provar-ho
  - Acció correctiva ràpida: afegir prova mínima o pas manual reproduïble abans d'obrir `R4`

## Exemples de feedback ràpid
- Vas bé: `La persistència ja està lligada al flux principal i la refactorització es pot explicar. Ara tanca regressió i README tècnic.`
- Cal corregir abans de seguir: `No pots passar a R4 si la persistència encara és parcial o si el flux principal continua fràgil.`
- Tens funcionalitat però falta verificació: `La dada es guarda, però encara no has mostrat que el cas d'ús antic continua viu després del canvi.`
- Tens solució massa superficial: `Has reorganitzat fitxers, però el producte no és més mantingible ni més defensable.`
- Tens marge per ampliar: `Si R3 ja està tancat, pots reforçar proves, model de dades o claredat d'arquitectura del mateix flux.`

## Fulls de treball base contextualitzats
### Full 1. Refactorització dirigida
- Objectiu: fer més mantenible una funcionalitat ja existent
- Tasca: identificar flux, separar responsabilitats i tocar només una operació central
- Evidència a generar: estructura refactoritzada recognoscible
- Validació mínima: el flux encara es pot executar després del canvi
- Ajuda si et bloqueges: torna a una sola operació i elimina refactorització lateral
- Ampliació si acabes prompte: millora noms, proves o claredat d'una capa

### Full 2. Persistència del domini
- Objectiu: fer persistent el cas d'ús principal
- Tasca: modelar entitat, guardar-la o recuperar-la i revisar validació lligada al model
- Evidència a generar: prova persistent + traça de model de dades + nota al `README`
- Validació mínima: el cas d'ús es pot repetir amb resultat coherent
- Ajuda si et bloqueges: una sola entitat, una sola relació si cal i una sola operació
- Ampliació si acabes prompte: afegir relació o prova de regressió millor tancada

## Suport per alumnat endarrerit
- forçar una sola funcionalitat persistent de punta a punta
- no tocar diverses capes si encara no hi ha una primera entitat estable
- revisar flux principal, model i `README` abans d'afegir noves relacions
- bloquejar el pas a `R4` si no hi ha arquitectura mínimament explicable

## Ampliacions per alumnat avançat
- relació addicional del domini dins del mateix cas d'ús
- prova de regressió més clara o automatitzada
- millor separació de capes o servei més robust

## Evidència mínima per tram
- Tram inicial: cas d'ús triat per refactoritzar i model mínim
- Tram funcional: persistència real de l'operació principal
- Tram de tancament: arquitectura explicable, prova mínima i documentació actualitzada

## Connexió amb el repte següent
El `R3` només té sentit si deixa una base prou estable per publicar una `API` amb valor. Si la persistència encara és provisional o el flux no és defensable, `R4` es convertirà en una capa pública d'un backend encara immadur.
