# Materials de sessió del Repte 2

## Finalitat del document

Contextualitzar les plantilles d'aula del curs per al `R2`, de manera que el professorat puga conduir la construcció d'una primera funcionalitat real del producte sobre la base comuna en `PHP`, sense reduir el repte a “fer login”.

## Mini-briefings de les sessions clau

### Sessió clau 1. Formulari i validació visible

- Objectiu de la sessió: obrir l'entrada de dades del projecte i fer visibles errors, correcció i reintent.
- Què s'espera al final: dades recuperades en servidor i error interpretable quan una dada no és vàlida.
- Error habitual a evitar: quedar-se en un formulari decoratiu o en missatges genèrics.
- Evidència mínima del dia: enviament incorrecte, error visible i reenviament corregit.
- Pregunta de tancament: quina dada entra al sistema i per què encara no pot continuar el flux?

### Sessió clau 2. Processament i guardat funcional

- Objectiu de la sessió: tractar la petició correcta en servidor i deixar una primera reutilització funcional de la informació.
- Què s'espera al final: dada correcta processada, guardada amb un mecanisme simple i tornada a mostrar o reutilitzar.
- Error habitual a evitar: convertir el repte en un exercici de persistència abans d'hora.
- Evidència mínima del dia: flux correcte de processament i conservació funcional de la dada.
- Pregunta de tancament: com reapareix la informació correcta dins del projecte?

### Sessió clau 3. Lògica del flux i regles del projecte

- Objectiu de la sessió: fer que el backend prenga decisions amb sentit i aplique una regla bàsica del domini.
- Què s'espera al final: una decisió, estructura o funció amb efecte visible sobre el comportament.
- Error habitual a evitar: afegir lògica ornamental només per cobrir criteris.
- Evidència mínima del dia: dos casos amb comportament diferent segons la regla aplicada.
- Pregunta de tancament: quina regla del projecte està prenent el sistema i sobre quines dades?

### Sessió clau 4. Estat, sessió i/o cookies

- Objectiu de la sessió: mantindre informació temporal del flux sense confondre-la amb la persistència del domini.
- Què s'espera al final: estat recuperable, explicació clara del que queda en client o en servidor i invalidació quan toca.
- Error habitual a evitar: usar sessió o cookies sense poder explicar què es guarda i per què.
- Evidència mínima del dia: recuperació d'un pas o esborrany i neteja de l'estat.
- Pregunta de tancament: què és temporal en este flux i què és informació funcional del producte?

### Sessió clau 5. Autenticació i funcionalitat protegida

- Objectiu de la sessió: connectar el flux anterior amb una operació real del domini restringida per autenticació o autorització.
- Què s'espera al final: acció protegida amb cas autoritzat i cas denegat.
- Error habitual a evitar: protegir una ruta decorativa o una pantalla sense valor funcional.
- Evidència mínima del dia: prova del cas permés i prova del cas bloquejat.
- Pregunta de tancament: què pot fer ara un usuari autoritzat que abans no podia fer?

### Sessió clau 6. Prova, depuració i checkpoint

- Objectiu de la sessió: tancar `R2` amb prova reproduïble, documentació mínima i pas clar cap a `R3`.
- Què s'espera al final: checklist breu, `README` actualitzat i demo curta del flux complet.
- Error habitual a evitar: tindre funcionalitat aparent sense prova verificable ni rastre d'error controlat.
- Evidència mínima del dia: flux complet provat, cas autoritzat, cas denegat i un cas d'error registrat.
- Pregunta de tancament: què has demostrat de punta a punta i què hauràs de reorganitzar després en `R3`?

## Checkpoints curts específics

- `CP-R2.1`
  - Què hauria d'estar fet: entrada de dades, validació visible i tractament inicial tancats.
  - Com es verifica en `2-3` minuts: provocar un error de validació, corregir-lo i mostrar la dada recuperada.
  - Senyal d'alerta: el grup diu què passaria, però no ho pot ensenyar.
  - Acció correctiva ràpida: tancar primer un únic cas d'error clar i el seu reintent.
- `CP-R2.2`
  - Què hauria d'estar fet: informació correcta processada, guardada funcionalment i reutilitzable.
  - Com es verifica en `2-3` minuts: crear una dada i tornar-la a mostrar en el mateix projecte.
  - Senyal d'alerta: la dada s'accepta, però després no reapareix enlloc.
  - Acció correctiva ràpida: congelar noves opcions i tornar a un únic cas d'ús complet.
- `CP-R2.3`
  - Què hauria d'estar fet: regla del projecte i estat temporal recognoscibles.
  - Com es verifica en `2-3` minuts: mostrar dos comportaments diferents i recuperar un pas del flux.
  - Senyal d'alerta: hi ha sessió, però no es veu quin valor aporta al recorregut.
  - Acció correctiva ràpida: simplificar l'estat a una sola dada temporal útil.
- `CP-R2.4`
  - Què hauria d'estar fet: operació real del domini protegida.
  - Com es verifica en `2-3` minuts: repetir la mateixa operació amb i sense accés.
  - Senyal d'alerta: hi ha auth, però no hi ha valor funcional del producte.
  - Acció correctiva ràpida: connectar la protecció a una única acció central del domini.
- `CP-R2.5`
  - Què hauria d'estar fet: prova mínima, documentació i pas a `R3` preparats.
  - Com es verifica en `2-3` minuts: seguir la demo breu i la guia de reproducció.
  - Senyal d'alerta: el grup ensenya una demo memòria però no una prova repetible.
  - Acció correctiva ràpida: documentar només tres casos clau abans d'obrir `R3`.

## Exemples de feedback ràpid

- Vas bé: `Ja tens el flux complet quasi tancat. Ara deixa clara la reutilització de la dada i registra millor la prova.`
- Cal corregir abans de seguir: `No pots obrir R3 si encara no hi ha una operació de negoci protegida i reproduïble.`
- Tens funcionalitat però falta coherència: `La sessió funciona, però encara no queda clara la diferència entre estat temporal i informació del domini.`
- Tens solució massa superficial: `El login funciona, però el producte encara no resol res rellevant amb eixa auth.`
- Tens marge per ampliar: `Si el flux principal ja està tancat, pots afegir una segona regla del projecte o millorar el tractament d'errors.`

## Fulls de treball base contextualitzats

### Full 1. Entrada, tractament i reutilització

- Objectiu: deixar tancat el recorregut des del formulari fins a la primera reutilització de la dada correcta.
- Tasca: validar, processar i tornar a mostrar informació útil del projecte.
- Evidència a generar: error visible, dada correcta guardada i reutilització posterior.
- Validació mínima: un cas incorrecte i un cas correcte complet.
- Ajuda si et bloqueges: torna a l'apunt real de `R2` i simplifica el nombre de camps o de pantalles.
- Ampliació si acabes prompte: afegeix fitxer o imatge amb control bàsic, si el flux ho demana.

### Full 2. Regla, estat i acció protegida

- Objectiu: deixar el primer flux funcional real del producte amb estat i operació protegida.
- Tasca: connectar una regla del domini, estat temporal i autenticació amb una acció central del projecte.
- Evidència a generar: regla observable, recuperació d'estat, operació protegida i prova de denegació.
- Validació mínima: es pot repetir el flux davant del professorat amb cas permés i cas bloquejat.
- Ajuda si et bloqueges: tanca només una operació central i elimina funcionalitat lateral.
- Ampliació si acabes prompte: afegeix una segona restricció o una prova més sistemàtica del mateix flux.

## Suport per alumnat endarrerit

- treballar amb un sol actor i una sola operació protegida
- simplificar el formulari al mínim útil abans d'afegir rols o extres
- revisar primer error visible, reutilització de la dada i `README` abans d'obrir noves pantalles
- microcheckpoint obligatori abans d'obrir `R3`

## Ampliacions per alumnat avançat

- segona regla de negoci sobre el mateix flux
- millor tractament de fitxer o imatge quan forme part del cas d'ús
- proves més sistemàtiques del cas correcte i incorrecte
- millor registre d'incidències i preparació de `R3`

## Evidència mínima per tram

- Tram inicial: entrada de dades, validació visible i processament bàsic
- Tram funcional: reutilització de la informació correcta, regla del projecte i estat temporal
- Tram protegit: autenticació funcional i operació de negoci protegida
- Tram de tancament: errors mínims controlats, prova reproduïble i `README` actualitzat

## Connexió amb el repte següent

El `R2` ha de deixar un flux prou real per justificar `R3`. Si només hi ha auth aparent, o si la dada correcta encara no es reutilitza dins del producte, la refactorització i la persistència no tindran una base funcional seriosa sobre la qual treballar.
