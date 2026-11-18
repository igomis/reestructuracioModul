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

### Sessió clau 4. Components i manteniment en `R3M4`

- Objectiu de la sessió: mantindre un recurs existent amb una peça de vista reutilitzable i les convencions del framework
- Què s'espera al final: component usat en dos llocs, actualització, eliminació controlada i regressió d'`R3M3`
- Error habitual a evitar: convertir el segon flux en una còpia del primer formulari o en una pantalla sense canvi real en BBDD
- Evidència mínima del dia: `PUT/PATCH` i `DELETE` o equivalents documentats, CSRF, `404`, regla d'eliminació i BBDD coherent
- Pregunta de tancament: què reutilitzes, per què l'operació és `PUT`, `PATCH` o `DELETE`, i què ocorre quan falla?

## Pauta teòrica docent per a R3M4

### Idees que cal fixar abans de programar

1. `R3M4` manté un recurs existent; no repetix l'alta d'`R3M3` amb altres noms.
2. `PATCH` modifica una part del recurs, `PUT` representa una substitució completa i `DELETE` l'elimina.
3. Cancel·lar, completar o arxivar és normalment un canvi d'estat amb `PATCH`, no una eliminació.
4. Els formularis HTML només envien `GET` i `POST`; el framework pot usar *method override* o una acció server-rendered equivalent que l'alumnat ha de documentar.
5. El component rep dades explícites i es reutilitza almenys en dos llocs. El *layout* general no compta.
6. Una operació insegura necessita CSRF, validació en servidor, recurs inexistent controlat i una regla del domini.
7. La transacció només és necessària quan una operació ha de completar diversos canvis relacionats com una unitat.

### Equivalències de component que el professorat pot acceptar

| Framework | Peça reutilitzable adequada |
|---|---|
| Laravel | Component Blade anònim o de classe amb propietats explícites |
| Symfony | Component Twig, macro o `include` amb dades explícites |
| Django 6 o superior | *Template partial* amb `partialdef` i `partial` |
| Django 5.2 o anterior | `include ... with ... only`; `inclusion_tag` si cal preparar dades amb Python |
| NestJS server-rendered | Parcial o component del motor de plantilles configurat |

En Django, no cal exigir una biblioteca externa. Un `include` amb `only` és
suficient quan el fragment només presenta dades. L'`inclusion_tag` té sentit si
cal preparar el context amb lògica Python, però no ha d'amagar regles de negoci.

### Modelatge docent breu

Usar un únic recurs i mostrar el recorregut complet:

```text
GET edició
  -> recuperar recurs o 404
  -> renderitzar formulari amb dades actuals

PATCH/PUT o equivalent
  -> CSRF i validació
  -> regla del domini
  -> canvi en BBDD
  -> redirecció i lectura de l'estat persistent

DELETE o equivalent
  -> CSRF
  -> recuperar recurs o 404
  -> permetre o denegar segons la regla
  -> eliminar i comprovar la BBDD
```

Durant el modelatge, renderitzar la mateixa targeta, fila o fragment de formulari
en dos contextos. Si l'operació modifica diversos registres, provocar una fallada
i mostrar que el *rollback* evita un estat parcial.

### Preguntes de comprovació oral

- Quina diferència funcional hi ha entre l'alta d'`R3M3` i este manteniment?
- Quins camps canvien i això justifica `PUT` o `PATCH`?
- Com expressa el teu framework l'operació des d'un formulari HTML?
- Quines dades rep el component i on es renderitza dues vegades?
- Quina regla impedix una eliminació no vàlida?
- Quina resposta dona un identificador que no existix?
- Quants registres canvien i, per tant, cal una transacció?
- Quina prova demostra que `R3M3` continua funcionant?

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
- `CP-R3.4`
  - Què hauria d'estar fet: manteniment d'un recurs amb component reutilitzable
  - Com es verifica en `2-3` minuts: localitzar els dos usos del component, actualitzar, eliminar i provocar un `404` o denegació
  - Senyal d'alerta: HTML duplicat, canvi amb `GET`, operació sense CSRF o modificació que només existix en la resposta
  - Acció correctiva ràpida: reduir el manteniment a una edició parcial i una eliminació amb una única regla clara

## Exemples de feedback ràpid

- Vas bé: `El projecte arranca, la BBDD es reconstrueix i ja tens clar quin flux ve de R2. Ara tanca el primer recorregut complet.`
- Cal corregir abans de seguir: `No pots passar a R4 si només tens esquelet del framework o dades carregades a mà.`
- Tens funcionalitat però falta verificació: `Els fluxos es poden veure, però encara falta prova mínima, error controlat o README executable.`
- Tens solució massa superficial: `El segon flux no és funcional; és només una vista o canvi visual. Redueix-lo, però fes-lo real.`
- Tens manteniment però falta convenció: `El canvi arriba a la BBDD, però encara has de justificar PUT o PATCH, protegir l'operació i controlar el recurs inexistent.`
- Tens component només de nom: `Has separat un fitxer, però falta entrada explícita i un segon ús real que evite duplicació.`
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

### Full 3. Components i manteniment d'un recurs

- Objectiu: actualitzar i eliminar un recurs existent sense duplicar presentació
- Tasca: extraure un component amb dos usos, implementar `PUT/PATCH` i `DELETE` o equivalents, i aplicar una regla d'eliminació
- Evidència a generar: component, operacions amb BBDD real, error controlat i regressió d'`R3M3`
- Validació mínima: actualització correcta i invàlida, eliminació permesa i denegada, i identificador inexistent
- Ajuda si et bloqueges: una sola entitat, un fragment visual curt, una edició parcial i una regla d'eliminació
- Ampliació si acabes prompte: variants del component, *soft delete* justificat o prova específica de *rollback*

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
- Tram de manteniment: component reutilitzat, `PUT/PATCH`, `DELETE`, `404`, regla de domini i regressió
- Tram de tancament: dos fluxos, proves mínimes, README i backlog de migració

## Connexió amb el repte següent

El `R3` només té sentit si deixa una base prou estable per publicar una `API` amb valor. Si el projecte no arranca, la BBDD no es reconstrueix o només hi ha un flux, `R4` es convertirà en una capa pública d'un backend encara immadur.
