# Materials de sessió del Repte 3

## Finalitat del document

Contextualitzar les plantilles d'aula del curs per al `R3`, de manera que el professorat puga conduir la reconstrucció del projecte en framework amb base operativa real, persistència mínima real i dos fluxos funcionals verificables.

## Mini-briefings de les sessions clau

### Sessió clau 1. Arrencada real del framework

- Objectiu de la sessió: deixar el projecte arrancant amb Docker, `.env` i una ruta mínima
- Què s'espera al final: framework operatiu i `2` casos d'ús declarats
- Error habitual a evitar: instal·lar el framework però no tindre cap producte executable
- Evidència mínima del dia: Docker funcional, ruta inicial i identificació del flux que ve de `R2`
- Pregunta de tancament: quin flux de `R2` migraràs i quin serà el segon flux?

### Sessió clau 2. Persistència reproduïble

- Objectiu de la sessió: crear BBDD real amb `migrations` i dades inicials amb `seeders` o equivalent
- Què s'espera al final: esquema inicial, dades de prova i primera lectura real
- Error habitual a evitar: carregar dades manualment o simular-les en arrays
- Evidència mínima del dia: reset de BBDD, migracions, seeders i lectura des de l'aplicació
- Pregunta de tancament: pots reconstruir les dades de demo des de zero?

### Sessió clau 3. Dos fluxos i tancament de `R3`

- Objectiu de la sessió: demostrar els `2` casos d'ús end-to-end amb validació, errors i proves mínimes
- Què s'espera al final: base en framework explicable, persistent i preparada per a `R4`
- Error habitual a evitar: tancar amb un únic flux o amb un segon flux només visual
- Evidència mínima del dia: dos fluxos, prova curta, error controlat, README i backlog
- Pregunta de tancament: què queda migrat, què queda pendent i què podria publicar-se com a `API`?

## Checkpoints curts específics

- `CP-R3.1`
  - Què hauria d'estar fet: projecte en framework arrancable amb Docker
  - Com es verifica en `2-3` minuts: executar arrencada i obrir ruta mínima
  - Senyal d'alerta: hi ha carpetes del framework però no entorn reproduïble
  - Acció correctiva ràpida: reduir stack i tancar només arrencada, `.env` i ruta inicial
- `CP-R3.2`
  - Què hauria d'estar fet: BBDD reconstruïble
  - Com es verifica en `2-3` minuts: executar migracions i seeders o equivalent
  - Senyal d'alerta: dades creades a mà o no documentades
  - Acció correctiva ràpida: una entitat central, una migració i un seeder mínim
- `CP-R3.3`
  - Què hauria d'estar fet: `2` fluxos end-to-end
  - Com es verifica en `2-3` minuts: executar els dos recorreguts i provocar un error
  - Senyal d'alerta: només funciona un flux o el segon és cosmètic
  - Acció correctiva ràpida: reduir el segon flux a una operació xicoteta però real

## Exemples de feedback ràpid

- Vas bé: `El projecte arranca, la BBDD es reconstrueix i ja tens clar quin flux ve de R2. Ara tanca el primer recorregut complet.`
- Cal corregir abans de seguir: `No pots passar a R4 si només tens esquelet del framework o dades carregades a mà.`
- Tens funcionalitat però falta verificació: `Els fluxos es poden veure, però encara falta prova mínima, error controlat o README executable.`
- Tens solució massa superficial: `El segon flux no és funcional; és només una vista o canvi visual. Redueix-lo, però fes-lo real.`
- Tens marge per ampliar: `Si R3 ja està tancat, pots reforçar proves, relació de dades o preparació del contracte d'API.`

## Fulls de treball base contextualitzats

### Full 1. Arrencada i dades

- Objectiu: fer arrancable i reproduïble la base del framework
- Tasca: Docker, `.env`, ruta mínima, migracions, seeders i lectura real
- Evidència a generar: projecte arrancable i BBDD reconstruïble
- Validació mínima: reset de BBDD i lectura de dades des de l'aplicació
- Ajuda si et bloqueges: una sola entitat, un seeder i una ruta de prova
- Ampliació si acabes prompte: millora scripts o afegeix relació simple

### Full 2. Fluxos funcionals

- Objectiu: tancar `2` casos d'ús end-to-end
- Tasca: migrar un flux de `R2` i implementar un segon flux o ampliació útil
- Evidència a generar: dos recorreguts funcionals amb BBDD, validació i error mínim
- Validació mínima: cas positiu i cas negatiu dels fluxos
- Ajuda si et bloqueges: redueix cada flux al recorregut més curt que continue sent real
- Ampliació si acabes prompte: reforça proves o prepara recurs d'API

## Suport per alumnat endarrerit

- mantindre un stack i una configuració mínima
- una sola entitat central si cal
- un primer flux heretat de `R2` molt acotat
- segon flux xicotet però real
- no eliminar Docker, `migrations`, `seeders`, proves ni README

## Ampliacions per alumnat avançat

- relació addicional del domini dins dels fluxos
- prova automatitzada més clara
- millor tractament d'errors
- primer esborrany de contracte d'`API`

## Evidència mínima per tram

- Tram inicial: framework arrancable, Docker, `.env` i abast dels `2` fluxos
- Tram funcional: BBDD amb `migrations`, `seeders` i primer flux migrat de `R2`
- Tram de tancament: segon flux, proves mínimes, README i backlog de migració

## Connexió amb el repte següent

El `R3` només té sentit si deixa una base prou estable per publicar una `API` amb valor. Si el projecte no arranca, la BBDD no es reconstrueix o només hi ha un flux, `R4` es convertirà en una capa pública d'un backend encara immadur.
