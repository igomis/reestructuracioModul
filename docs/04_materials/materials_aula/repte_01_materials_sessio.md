# Materials de sessió del Repte 1

## Finalitat del document
Contextualitzar les plantilles d'aula del curs per al `R1`, de manera que el professorat dispose d'un paquet curt per obrir la fase d'arrancada funcional del producte sense quedar-se en tria d'stack o en esquelet buit.

## Mini-briefings de les sessions clau
### Sessió clau 1. Marc comú i producte
- Objectiu de la sessió: entendre què s'ha de posar en marxa realment al `R1`
- Què s'espera al final: domini provisional triat i repositori ja obert
- Error habitual a evitar: confondre kickoff amb instal·lar framework sense producte
- Evidència mínima del dia: repositori creat i `README` inicial
- Pregunta de tancament: quin primer flux real del producte voleu poder ensenyar?

### Sessió clau 2. Decisió tècnica i primera peça funcional
- Objectiu de la sessió: convertir la decisió de domini i stack en una entrada funcional del producte
- Què s'espera al final: landing page o equivalent i formulari mínim
- Error habitual a evitar: justificar tecnologia sense cap interacció funcional
- Evidència mínima del dia: pantalla d'entrada o equivalent + formulari executable
- Pregunta de tancament: què pot fer ja una persona usuària dins del producte?

### Sessió clau 3. Validació i primer registre
- Objectiu de la sessió: tancar el primer flux amb validació i registre bàsic
- Què s'espera al final: dada enviada, validada i registrada o persistida
- Error habitual a evitar: mostrar només el cas feliç sense resposta d'error
- Evidència mínima del dia: prova d'enviament correcta i incorrecta
- Pregunta de tancament: què queda realment guardat o registrat després del formulari?

## Checkpoints curts específics
- `CP-R1.1`
  - Què hauria d'estar fet: repositori usable, `README` curt i decisió tècnica visible
  - Com es verifica en `2-3` minuts: obrir repo, localitzar `README` i explicar domini + stack
  - Senyal d'alerta: hi ha codi, però no hi ha criteri de producte ni traçabilitat
  - Acció correctiva ràpida: congelar nova configuració i tancar només domini, `README` i arranque
- `CP-R1.2`
  - Què hauria d'estar fet: landing page o equivalent i formulari mínim
  - Com es verifica en `2-3` minuts: arrancar projecte i mostrar el flux d'entrada
  - Senyal d'alerta: només hi ha ruta de prova o plantilla estàtica
  - Acció correctiva ràpida: reduir a una sola interacció real i eliminar decoració sobrant
- `CP-R1.3`
  - Què hauria d'estar fet: validació mínima i primer registre de dades
  - Com es verifica en `2-3` minuts: enviar una dada correcta i una incorrecta
  - Senyal d'alerta: el producte sembla funcionar, però no registra ni valida res
  - Acció correctiva ràpida: tancar únicament camps obligatoris, resposta d'error i registre mínim

## Exemples de feedback ràpid
- Vas bé: `Ja tens arranque, primera interacció i una evidència visible. Ara tanca la validació i deixa el README executable.`
- Cal corregir abans de seguir: `Encara no pots passar a R2 perquè el que tens és només infraestructura. Necessite veure una acció real del producte.`
- Tens funcionalitat però falta verificació: `La pantalla inicial està, però encara falta provar l'enviament i deixar rastre del registre.`
- Tens solució massa superficial: `Has triat stack i has muntat entorn, però encara no puc veure cap cas d'ús d'entrada al producte.`
- Tens marge per ampliar: `Si ja tens el mínim del R1, pots reforçar validació, missatges d'error o claredat del README, però sense obrir un segon flux.`

## Fulls de treball base contextualitzats
### Full 1. Kickoff funcional
- Objectiu: deixar el projecte obert amb domini, stack i arranque recognoscibles
- Tasca: crear repositori, `README`, decisió tècnica i estructura mínima
- Evidència a generar: repositori usable + `README` + justificació breu del domini
- Validació mínima: una altra persona pot entendre què fareu i com arranca
- Ajuda si et bloqueges: torna a l'apunt real de `R1` i a la guia `README`/`ADR`
- Ampliació si acabes prompte: prepara una segona alternativa descartada amb trade-off curt

### Full 2. Primera peça funcional
- Objectiu: obrir una interacció real del producte
- Tasca: implementar landing page o equivalent, formulari mínim i registre bàsic
- Evidència a generar: prova del flux d'entrada correcte i incorrecte
- Validació mínima: la dada entra, es valida i queda registrada de manera mínima
- Ajuda si et bloqueges: simplifica camps i tanca només el cas principal
- Ampliació si acabes prompte: millora feedback d'errors o persistència inicial

## Suport per alumnat endarrerit
- reduir el repte a un únic flux d'entrada real del producte
- evitar obrir diverses vistes o formularis si encara no hi ha un que funcione complet
- revisar primer `README`, validació i registre abans de tocar disseny o estructura extra
- fer microcheckpoint de recuperació abans d'entrar en `R2`

## Ampliacions per alumnat avançat
- reforçar validació i missatges d'error del primer flux
- documentar millor la decisió tècnica i el cas d'ús triat
- afegir una segona dada de domini, però sempre dins del mateix flux d'entrada

## Evidència mínima per tram
- Tram inicial: repositori, `README`, decisió tècnica i domini triat
- Tram funcional: landing page o equivalent i formulari útil
- Tram de tancament: validació mínima, primer registre i traçabilitat recognoscible

## Connexió amb el repte següent
El `R1` només queda ben preparat si deixa una entrada real al producte que puga convertir-se en funcionalitat autenticada al `R2`. Si al final d'este repte només hi ha infraestructura, el pas a sessions i auth començarà sobre una base falsa.
