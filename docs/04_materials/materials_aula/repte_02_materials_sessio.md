# Materials de sessió del Repte 2

## Finalitat del document
Contextualitzar les plantilles d'aula del curs per al `R2`, de manera que el professorat puga conduir la construcció de la primera funcionalitat de negoci autenticada sense reduir el repte a “fer login”.

## Mini-briefings de les sessions clau
### Sessió clau 1. Auth com a infraestructura
- Objectiu de la sessió: obrir registre, login o estat equivalent al servei d'un flux del producte
- Què s'espera al final: mecanisme bàsic d'accés i actor del domini identificat
- Error habitual a evitar: quedar-se en formularis d'autenticació sense operació real
- Evidència mínima del dia: alta o login funcional
- Pregunta de tancament: quin cas d'ús del producte quedarà protegit per esta auth?

### Sessió clau 2. Primera funcionalitat de negoci protegida
- Objectiu de la sessió: connectar auth amb una operació del domini que tinga valor real
- Què s'espera al final: acció protegida i regla mínima de negoci
- Error habitual a evitar: protegir una ruta decorativa
- Evidència mínima del dia: flux amb accés autoritzat i accés denegat
- Pregunta de tancament: què pot fer una persona autenticada que abans no podia fer?

### Sessió clau 3. Validació, errors i prova del flux
- Objectiu de la sessió: tancar `R2` amb verificació mínima
- Què s'espera al final: casos correctes, casos límit i `README` actualitzat
- Error habitual a evitar: tindre funcionalitat aparent sense prova reproduïble
- Evidència mínima del dia: prova breu del flux complet i del cas d'error
- Pregunta de tancament: què passa si les dades són incorrectes o si l'usuari no té accés?

## Checkpoints curts específics
- `CP-R2.1`
  - Què hauria d'estar fet: alta o login bàsic operatiu
  - Com es verifica en `2-3` minuts: crear o autenticar un usuari de prova
  - Senyal d'alerta: el flux només funciona en el cas feliç
  - Acció correctiva ràpida: tancar abans un cas d'error clar
- `CP-R2.2`
  - Què hauria d'estar fet: una operació real del domini protegida
  - Com es verifica en `2-3` minuts: repetir la mateixa operació amb i sense accés
  - Senyal d'alerta: hi ha auth, però no hi ha valor funcional del producte
  - Acció correctiva ràpida: congelar noves opcions i connectar auth a un únic cas d'ús
- `CP-R2.3`
  - Què hauria d'estar fet: validacions i errors mínims controlats
  - Com es verifica en `2-3` minuts: provar dada incorrecta o accés no autoritzat
  - Senyal d'alerta: el grup explica què passaria, però no ho pot mostrar
  - Acció correctiva ràpida: documentar i provar només dos casos clau abans de seguir

## Exemples de feedback ràpid
- Vas bé: `Ja tens auth connectada a una acció real del domini. Ara tanca errors i prova el flux complet.`
- Cal corregir abans de seguir: `No pots obrir R3 si encara no hi ha una operació de negoci protegida i reproduïble.`
- Tens funcionalitat però falta verificació: `La funcionalitat es veu, però encara no has provat el cas denegat ni has actualitzat el README.`
- Tens solució massa superficial: `El login funciona, però el producte encara no resol res rellevant amb eixa auth.`
- Tens marge per ampliar: `Si el flux principal ja està tancat, pots afegir una regla de rol o millor tractament d'errors.`

## Fulls de treball base contextualitzats
### Full 1. Alta i accés
- Objectiu: posar auth o estat equivalent en marxa amb criteri mínim
- Tasca: crear alta/login i una primera verificació d'accés
- Evidència a generar: usuari operatiu + estat d'accés clar
- Validació mínima: un cas correcte i un cas incorrecte
- Ajuda si et bloqueges: torna a l'apunt real de `R2` i simplifica el nombre d'actors
- Ampliació si acabes prompte: millora missatges o separa millor auth i autorització

### Full 2. Cas d'ús protegit
- Objectiu: deixar el primer flux funcional real del producte
- Tasca: connectar auth amb una operació del domini i una restricció mínima
- Evidència a generar: operació protegida + prova de denegació + nota al `README`
- Validació mínima: es pot repetir el flux davant del professorat
- Ajuda si et bloqueges: tanca només una operació central i elimina funcionalitat lateral
- Ampliació si acabes prompte: afegeix permís, rol o segona prova del mateix flux

## Suport per alumnat endarrerit
- treballar amb un sol actor i una sola operació protegida
- eliminar extensions de rols fins que el flux principal estiga tancat
- revisar primer accés denegat, validació i `README` abans d'afegir noves pantalles
- microcheckpoint obligatori abans d'obrir `R3`

## Ampliacions per alumnat avançat
- segona restricció de negoci sobre el mateix flux
- proves més sistemàtiques del cas correcte i incorrecte
- millor tractament d'errors i registre d'incidències

## Evidència mínima per tram
- Tram inicial: auth o estat equivalent funcional
- Tram funcional: operació de negoci protegida
- Tram de tancament: errors mínims controlats, prova reproduïble i `README` actualitzat

## Connexió amb el repte següent
El `R2` ha de deixar un flux prou real per justificar `R3`. Si només hi ha auth aparent, la refactorització i la persistència no tindran una base funcional seriosa sobre la qual treballar.
