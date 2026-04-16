# Materials de sessió del Repte 1

## Finalitat del document

Contextualitzar les plantilles d'aula del curs per al `R1` amb una seqüència curta i realista de `4` sessions de `3` hores, una per microrepte.

## Seqüència base del repte

- Sessió `1` -> Microrepte `1`: model client/servidor i elecció guiada de stack
- Sessió `2` -> Microrepte `2`: entorn executable amb Docker, PHP i servidor web
- Sessió `3` -> Microrepte `3`: primer punt d'entrada funcional del backend
- Sessió `4` -> Microrepte `4`: documentació tècnica, verificació i checkpoint

## Mini-briefings de les sessions clau

### Sessió 1. Microrepte 1

- Objectiu de la sessió: entendre què fa el servidor dins del producte i fixar una base tècnica guiada.
- Què s'espera al final: decisió tècnica inicial i explicació clara del model client/servidor.
- Error habitual a evitar: convertir la sessió en un debat genèric de tecnologies sense impacte real en el producte.
- Evidència mínima del dia: justificació breu de stack i criteri tècnic visible.
- Pregunta de tancament: quin paper jugarà el servidor en el vostre producte i per què esta base és assumible?

### Sessió 2. Microrepte 2

- Objectiu de la sessió: posar en marxa un entorn executable amb `Docker`, `PHP` i servidor web.
- Què s'espera al final: projecte arrancant i `README` inicial prou clar per repetir l'arrencada.
- Error habitual a evitar: tindre configuració aparent però no un entorn realment executable.
- Evidència mínima del dia: arrencada reproduïble i instruccions mínimes d'ús.
- Pregunta de tancament: què aixeca `Docker`, què executa `PHP` i què aporta el servidor web?

### Sessió 3. Microrepte 3

- Objectiu de la sessió: deixar un primer punt d'entrada funcional del backend.
- Què s'espera al final: ruta, vista, `endpoint` o `healthcheck` simple però funcional.
- Error habitual a evitar: quedar-se en esquelet, plantilla o text estàtic sense comportament de backend.
- Evidència mínima del dia: resposta real del sistema en execució.
- Pregunta de tancament: què pot ensenyar ja el backend que no siga només infraestructura?

### Sessió 4. Microrepte 4

- Objectiu de la sessió: tancar `R1` amb documentació usable, verificació i checkpoint.
- Què s'espera al final: `README` executable, defensa breu i pas justificat cap a `R2`.
- Error habitual a evitar: tindre el projecte arrancat però no saber explicar-lo ni reproduir-lo.
- Evidència mínima del dia: demostració seguint el `README` i explicació del flux que s'obrirà en `R2`.
- Pregunta de tancament: què queda prou sòlid per continuar el projecte sense tornar a començar?

## Checkpoints curts específics

- `CP-R1.1`
  - Què hauria d'estar fet: explicació client/servidor i decisió tècnica breu.
  - Com es verifica en `2-3` minuts: explicar el paper del servidor i justificar la base triada.
  - Senyal d'alerta: hi ha noms d'eines, però no hi ha criteri de producte ni comprensió del flux.
  - Acció correctiva ràpida: reduir la comparativa i tancar una sola decisió tècnica defensable.
- `CP-R1.2`
  - Què hauria d'estar fet: entorn executable amb `Docker`, `PHP` i servidor web.
  - Com es verifica en `2-3` minuts: arrancar projecte i llegir els passos des del `README`.
  - Senyal d'alerta: existixen fitxers de configuració, però ningú sap què aixequen ni com provar-los.
  - Acció correctiva ràpida: congelar canvis laterals i tancar només arrencada i documentació mínima.
- `CP-R1.3`
  - Què hauria d'estar fet: punt d'entrada funcional del backend.
  - Com es verifica en `2-3` minuts: mostrar la ruta, vista, `endpoint` o `healthcheck` en execució.
  - Senyal d'alerta: només hi ha una plantilla o un esquelet que no respon amb sentit.
  - Acció correctiva ràpida: reduir a una sola resposta funcional i eliminar decoració sobrant.
- `CP-R1.4`
  - Què hauria d'estar fet: documentació tècnica usable i checkpoint de pas a `R2`.
  - Com es verifica en `2-3` minuts: obrir `README`, arrancar projecte, mostrar punt d'entrada i explicar el següent flux del producte.
  - Senyal d'alerta: el projecte funciona només en l'ordinador de l'autor o no es pot defendre.
  - Acció correctiva ràpida: reescriure `README`, simplificar demo i tornar a provar l'arrencada davant del professorat.

## Exemples de feedback ràpid

- Vas bé: `Ja tens clar el paper del servidor i l'entorn arranca. Ara deixa el punt d'entrada funcional i documenta'l bé.`
- Cal corregir abans de seguir: `Encara no pots passar a R2 perquè el que tens és només infraestructura. Necessite veure una resposta real del backend.`
- Tens arrencada però falta verificació: `El projecte s'alça, però encara falta demostrar que el README servix per a repetir-ho.`
- Tens solució massa superficial: `Has muntat contenidors i fitxers, però encara no puc veure quin valor funcional deixa el backend.`
- Tens marge per ampliar: `Si ja tens el mínim de R1, pots millorar el README, l'onboarding o la claredat del punt d'entrada, però sense obrir encara el flux complet de R2.`

## Fulls de treball base contextualitzats

### Full 1. Model client/servidor i stack

- Objectiu: decidir amb criteri què s'arrancarà i com s'explicarà.
- Tasca: concretar producte, paper del servidor i decisió tècnica inicial.
- Evidència a generar: comparativa breu o `ADR` curt.
- Validació mínima: una altra persona entén què farà el backend i per què la base triada és assumible.
- Ajuda si et bloqueges: torna al briefing inicial i a la guia `README`/`ADR`.
- Ampliació si acabes prompte: documenta una alternativa descartada amb un trade-off curt.

### Full 2. Entorn executable

- Objectiu: deixar el projecte arrancant amb `Docker`, `PHP` i servidor web.
- Tasca: preparar entorn, documentar passos i comprovar l'arrencada.
- Evidència a generar: `README` inicial i prova d'arrencada reproduïble.
- Validació mínima: una altra persona pot seguir els passos essencials.
- Ajuda si et bloqueges: simplifica l'entorn i tanca només el mínim que realment arranca.
- Ampliació si acabes prompte: millora scripts o organització de carpetes.

### Full 3. Punt d'entrada funcional

- Objectiu: obrir una primera resposta real del backend.
- Tasca: implementar una ruta, vista, `endpoint` o `healthcheck` coherent amb el producte.
- Evidència a generar: resposta visible del sistema en execució.
- Validació mínima: el backend fa alguna cosa real i explicable.
- Ajuda si et bloqueges: reduïx a una única resposta simple del sistema.
- Ampliació si acabes prompte: millora el missatge, la claredat o una segona resposta simple.

### Full 4. Documentació i checkpoint

- Objectiu: deixar `R1` documentat, verificat i preparat per a `R2`.
- Tasca: revisar `README`, comprovar arrencada, preparar defensa curta i explicar el pas següent.
- Evidència a generar: demo curta i `README` executable.
- Validació mínima: el producte es pot arrancar i explicar sense ajuda externa.
- Ajuda si et bloqueges: retalla text i centra't en els passos reals de reproducció.
- Ampliació si acabes prompte: afina millor onboarding o checklist de comprovació.

## Suport per alumnat endarrerit

- reduir el repte a una única decisió tècnica clara i un únic punt d'entrada funcional
- evitar obrir formularis, fluxos complets o persistència si encara no arranca el projecte
- revisar primer `README`, arrencada i punt d'entrada abans de tocar disseny o estructura extra
- fer microcheckpoint de recuperació abans d'entrar en `R2`

## Ampliacions per alumnat avançat

- documentar millor la decisió tècnica i el paper de cada component
- afegir una segona resposta simple del backend sense obrir encara el flux complet de dades
- millorar onboarding, scripts o verificació de l'entorn

## Evidència mínima per sessió

- Sessió `1`: criteri tècnic i explicació client/servidor.
- Sessió `2`: projecte arrancant i `README` inicial usable.
- Sessió `3`: punt d'entrada funcional del backend.
- Sessió `4`: documentació, verificació i checkpoint de pas.

## Connexió amb el repte següent

El `R1` només queda ben preparat si deixa una base executable i un punt d'entrada real del backend que puga créixer en `R2`. Si al final d'este repte només hi ha infraestructura o només hi ha intenció, el pas a sessions i auth començarà sobre una base falsa.
