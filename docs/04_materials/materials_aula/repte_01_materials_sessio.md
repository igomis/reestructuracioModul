# Materials de sessió del Repte 1

## Finalitat del document

Contextualitzar les plantilles d'aula del curs per al `R1` amb `4` microreptes com a passos lògics, compactats en `2` sessions principals de `3` hores i una tercera sessió opcional de defensa o checkpoint formal.

## Seqüència base del repte

- Sessió `1` -> Microrepte `1` + inici del Microrepte `2`: model client/servidor, decisió inicial i arrencada de l'entorn
- Sessió `2` -> tancament del Microrepte `2` + Microrepte `3` + Microrepte `4`: entorn complet, punt d'entrada funcional i documentació del repte
- Sessió `3` opcional -> defensa tècnica, execució seguint README, revisió de traçabilitat o microcanvis en viu

## Mini-briefings de les sessions clau

### Sessió 1. Microrepte 1 + inici del Microrepte 2

- Objectiu de la sessió: entendre què fa el servidor dins del producte, fixar una base tècnica guiada i iniciar l'entorn executable.
- Què s'espera al final: [fitxa breu d'exploració tècnica inicial](../../08_materials_compartibles/fitxa_exploracio_tecnica_inicial.md), decisió tècnica orientativa, estructura mínima del projecte i primeres proves d'arrencada.
- Error habitual a evitar: convertir la sessió en un debat genèric de tecnologies sense impacte real en el producte.
- Evidència mínima del dia: fitxa breu amb criteri tècnic visible i base mínima de projecte començada.
- Pregunta de tancament: quin paper jugarà el servidor en el vostre producte, amb quina base començareu i què heu arribat a muntar?

### Sessió 2. Tancament del Microrepte 2 + Microreptes 3 i 4

- Obertura possible: repàs del que falta per tancar l'entorn executable.
- Objectiu de la sessió: acabar l'entorn, crear el primer punt d'entrada funcional i deixar documentació útil dins del repositori.
- Què s'espera al final: projecte arrancant, serveis mínims definits, primera funcionalitat mínima, `README`, documentació en repositori i una decisió o incidència registrada.
- Error habitual a evitar: copiar la demo del professorat sense adaptar-la ni saber explicar què fa cada servei.
- Evidència mínima del dia: arrencada reproduïble, BBDD i phpMyAdmin incorporats si cal, punt d'entrada funcional i documentació enllaçada.
- Pregunta de tancament: què has adaptat, què funciona de veritat, on està documentat i com ho comproves?

### Sessió 3 opcional. Defensa / checkpoint formal

- S'activa si cal separar la defensa tècnica o la revisió forta d'evidències del treball de construcció.
- Pot incloure execució real seguint el `README`, revisió de commits, contrast de comprensió i microcanvis en viu.
- No afegix un cinqué microrepte: només acredita amb més calma el tancament de `R1`.

## Checkpoints curts específics

- `CP-R1.1`
  - Què hauria d'estar fet: fitxa breu d'exploració tècnica inicial, explicació client/servidor i decisió tècnica orientativa.
  - Com es verifica en `2-3` minuts: revisar la fitxa, explicar el paper del servidor i justificar amb què començarien.
  - Senyal d'alerta: hi ha noms d'eines, però no hi ha criteri de producte ni comprensió del flux.
  - Acció correctiva ràpida: reduir la fitxa, tancar una sola decisió tècnica defensable i deixar visibles els dubtes oberts.
- `CP-R1.2`
  - Què hauria d'estar fet: entorn executable amb `Docker`, `PHP`, servidor web, BBDD i phpMyAdmin.
  - Com es verifica en `2-3` minuts: arrancar projecte, llegir els passos des del `README` i explicar què s'ha adaptat respecte del model docent.
  - Senyal d'alerta: existixen fitxers de configuració, però ningú sap què aixequen, com provar-los o quina part ha completat.
  - Acció correctiva ràpida: congelar canvis laterals i tancar només arrencada, serveis mínims, documentació i una incidència o decisió real.
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
- Tasca: concretar producte, paper del servidor i completar la [fitxa breu d'exploració tècnica inicial](../../08_materials_compartibles/fitxa_exploracio_tecnica_inicial.md) amb tecnologies identificades, opcions explorades, primera decisió orientativa i dubtes detectats.
- Evidència a generar: fitxa breu d'exploració tècnica inicial.
- Validació mínima: una altra persona entén què farà el backend, quines tecnologies heu identificat i per què la base triada és assumible.
- Ajuda si et bloqueges: torna al briefing inicial i a la guia `README`/`ADR`.
- Ampliació si acabes prompte: documenta una alternativa descartada amb un trade-off curt.

### Full 2. Entorn executable

- Objectiu: deixar el projecte arrancant amb `Docker`, `PHP`, servidor web, BBDD i phpMyAdmin.
- Tasca: partir del model mínim mostrat pel professorat, adaptar-lo al projecte propi, completar l'entorn amb persistència i documentar passos.
- Evidència a generar: `README` inicial, prova d'arrencada reproduïble, decisió tècnica curta i incidència o dubte registrat.
- Validació mínima: una altra persona pot seguir els passos essencials i entendre què fa cada servei.
- Ajuda si et bloqueges: simplifica l'entorn i tanca només el mínim que realment arranca amb serveis comprovables.
- Ampliació si acabes prompte: millora scripts, organització de carpetes o comprovació dels serveis.

### Full 3. Punt d'entrada funcional

- Objectiu: obrir una primera resposta real del backend.
- Tasca: implementar una ruta, vista, `endpoint` o `healthcheck` coherent amb el producte.
- Evidència a generar: resposta visible del sistema en execució.
- Validació mínima: el backend fa alguna cosa real i explicable.
- Ajuda si et bloqueges: reduïx a una única resposta simple del sistema.
- Ampliació si acabes prompte: millora el missatge, la claredat o una segona resposta simple.

### Full 4. Documentació i checkpoint

- Objectiu: deixar `R1` documentat, verificat i preparat per a `R2`.
- Tasca: revisar `README`, comprovar arrencada, preparar defensa curta, crear directori de documentació, penjar les fitxes o documents del repte i explicar el pas següent.
- Evidència a generar: demo curta, `README` executable i documentació del repte enllaçada dins del repositori.
- Validació mínima: el producte es pot arrancar i explicar sense ajuda externa, i la documentació es pot localitzar des d'un índex o pàgina visible.
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

- Sessió `1`: fitxa breu d'exploració tècnica inicial, criteri tècnic, explicació client/servidor i inici d'entorn executable.
- Sessió `2`: projecte arrancant, BBDD i phpMyAdmin incorporats si cal, punt d'entrada funcional, `README`, documentació en repositori i decisió/incidència registrada.
- Sessió `3` opcional: defensa tècnica, execució real seguint `README`, revisió de traçabilitat o microcanvi en viu.

## Connexió amb el repte següent

El `R1` només queda ben preparat si deixa una base executable i un punt d'entrada real del backend que puga créixer en `R2`. Si al final d'este repte només hi ha infraestructura o només hi ha intenció, el pas a sessions i auth començarà sobre una base falsa.
