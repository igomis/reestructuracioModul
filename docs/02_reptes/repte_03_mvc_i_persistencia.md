# Repte 3. Reconstrucció en framework, persistència real i primers fluxos funcionals

## Fitxa canònica del repte

- **Funció didàctica principal**: consolidació.
- **Objectiu**: reconstruir el projecte en framework i deixar persistència real amb fluxos end-to-end verificables.
- **Producte esperat**: aplicació arrancable en framework amb Docker, base de dades real, migracions o mecanisme equivalent, fixtures/seeders o càrrega reproduïble, validació, proves mínimes i almenys dos fluxos funcionals, amb almenys un flux **server-rendered**.
- **Evidències**: casos d'ús end-to-end, model de dades, migracions o mecanisme equivalent, fixtures/seeders o càrrega reproduïble, README d'arrencada, nota tècnica de decisió breu de migració, commit rellevant comentat, proves, almenys una resposta HTML renderitzada en servidor i traçabilitat de decisions.
- **Paper de la IA**: ús assistit per IA permés per modelat, migracions, proves i revisió d'estructura; els límits i la delegació excessiva depenen de [us-ia-professorat-i-alumnat.md](../us-ia-professorat-i-alumnat.md).
- **Relació amb el projecte base**: professionalitza la base comuna de `R2` i obri el contrast d'itineraris sobre el mateix projecte base.
- **Checkpoint de control**: `CP-R3A` per validar framework + Docker + BBDD + migracions/fixtures/seeders o script equivalent + primer flux **server-rendered**; `CP-R3B` per validar segon flux, proves mínimes, README i mini defensa.
- **Instrument dominant**: rúbrica de reconstrucció en framework.
- **Instrument de comprensió**: defensa tècnica curta sobre migració i circuit petició -> controlador -> dades -> resposta.
- **Instrument de control de delegació excessiva**: revisió de commit rellevant comentat, contrast amb `AI log` i prova guiada sobre un flux migrat.
- **Instrument de recuperació o millora**: reobertura del segon flux o reducció d'abast funcional mantenint Docker, BBDD, migracions/fixtures/seeders o script equivalent i un flux **server-rendered** complet.

## Justificació docent

- **Evidència principal**: aplicació en framework amb persistència real i dos fluxos end-to-end, almenys un migrat de `R2`.
- **Evidències secundàries**: Docker, `.env`, migracions o equivalent, fixtures/seeders o càrrega reproduïble, proves, README, nota tècnica de decisió breu i defensa del circuit petició -> resposta.
- **Mínim suficient**: no és migrar fitxers; ha d'arrancar des de zero, crear dades reproduïbles i executar dos fluxos verificables.
- **Feedback previst**: `CP-R3A` sobre base tècnica i `CP-R3B` sobre segon flux, proves i explicació de responsabilitats.

## 1. Visió general del repte

**Finalitat del repte**

El `Repte 3` consistix a reconstruir el projecte en un framework amb una base operativa real, persistència mínima real i primers fluxos funcionals verificables.

No es demana migrar tota l'aplicació heretada de `R2`. Sí es demana construir una nova base tècnica en framework i portar-hi almenys `2` casos d'ús end-to-end. Com a mínim `1` d'eixos casos d'ús ha de vindre del projecte anterior. El segon pot ser també heretat o pot ser una ampliació funcional xicoteta si ajuda a fer visible el valor del framework.

El repte no és una reflexió abstracta sobre `MVC`, ni una simple separació de presentació i lògica, ni moure fitxers des del projecte antic. El que ha de quedar és una aplicació arrancable, amb Docker, configuració, rutes, controladors, vistes o plantilles, models o capa equivalent de dades, base de dades real, migracions o mecanisme equivalent, fixtures/seeders o càrrega reproduïble, validació, errors mínims, proves bàsiques i documentació d'ús.

És també el punt on s'obri el contrast de frameworks del curs. El mateix problema de producte que en `R2` s'ha treballat sobre base comuna en `PHP` continua ara amb `Laravel`, `Symfony` o `NestJS`. `FastAPI` només s'hauria d'obrir com a via avançada o excepcional quan hi haja marc docent clar per sostenir-la.

**Idea central**

Reconstrucció del projecte en framework amb base operativa real, persistència mínima real i primers fluxos funcionals verificables.

**Producte principal del repte**

Una aplicació en framework operativa que incloga, com a mínim:

- entorn `Docker` funcional
- projecte base en framework arrancable
- configuració mínima i `.env`
- rutes reals
- controladors o equivalents
- vistes, plantilles o mecanisme de resposta segons l'stack
- models, entitats, esquemes o capa equivalent de dades
- base de dades real connectada a l'aplicació
- migracions o mecanisme equivalent de l'stack per crear l'estructura de dades
- fixtures/seeders o script equivalent per carregar dades inicials reproduïbles
- almenys `2` casos d'ús end-to-end
- almenys `1` cas d'ús migrat des de `R2`
- validació i tractament bàsic d'errors
- proves mínimes
- documentació tècnica curta d'arrencada i ús

**Context professional simulat o realista**

L'equip té una aplicació inicial funcional, però encara no disposa d'una base de framework preparada per créixer amb persistència, proves, `API` i integració. En un context professional, abans d'ampliar funcionalitats o publicar serveis, cal reconstruir una base sòlida: entorn reproduïble, estructura del framework, model de dades inicial, dades de demostració, fluxos troncals funcionant i verificació mínima.

**Relació amb el projecte global del curs**

`R3` és el pont entre la base funcional de `R2` i la publicació d'`API` de `R4`. Si `R3` queda en discurs arquitectònic, `R4` només exposarà rutes sobre una base fràgil. Si `R3` deixa una aplicació en framework amb dades reals i dos fluxos funcionals, `R4` pot centrar-se en contracte, consum i qualitat de servei.

---

## 2. Relació amb resultats d'aprenentatge

**Resultat d'aprenentatge principal**

- **RA5**: desenvolupa aplicacions web identificant i aplicant mecanismes per a separar el codi de presentació de la lògica de negoci

**Resultats d'aprenentatge de suport**

- **RA6**: desenvolupa aplicacions web d'accés a magatzems de dades, aplicant mesures per a mantindre la seguretat i la integritat de la informació
- **RA8**: desenvolupa aplicacions web dinàmiques amb frameworks servidor, vistes o plantilles, formularis i generació de respostes HTML renderitzades en servidor

**Justificació curricular**

La programació vigent situa l'arquitectura MVC o equivalent com a **SA3** vinculada principalment a **RA5**, i reserva un pes més fort i específic d'**RA6** per a **SA4**. Per això, en `R3` el nucli continua sent **RA5**: usar el framework per ordenar entrada HTTP, coordinació, lògica, presentació i responsabilitats.

Ara bé, `RA6` queda ja fortament preparada i parcialment activada: no es pot parlar d'una base real en framework sense base de dades, migracions o mecanisme equivalent, fixtures/seeders o càrrega reproduïble, lectura i escriptura mínimes, validació i errors vinculats a dades. No s'inventa normativa nova ni es trasllada tot `RA6` a este repte, però sí es demana una persistència mínima real i verificable perquè el pas a `R4` no siga artificial.

`RA8` queda integrat explícitament en `R3` perquè el repte construeix pàgines dinàmiques amb framework servidor: s'usen vistes o plantilles, es processen formularis o interaccions en el servidor i el framework participa en la generació de la resposta HTML. Per això, almenys un dels `2` casos d'ús de `R3` ha de ser **server-rendered** i no només una resposta d'API o una consulta de dades.

En `R3M1`, l'alumnat no sols posa en marxa un framework: compara opcions, justifica la tria i identifica per què separar ruta, controlador, vista o resposta i model millora la base funcional heretada de `R2`. En `R3M2`, la informació recuperada des de la BBDD no queda com una consulta aïllada: es tracta com a conjunt de dades útil per alimentar llistats, detalls, filtres o respostes reals del projecte.

---

## 3. Criteri didàctic del repte

La frontera amb `R2` ha de quedar clara:

- en `R2` es construeix una base funcional comuna en `PHP`
- en `R3` entra el framework com a base principal del projecte
- en `R3` no es migra tota l'aplicació heretada
- en `R3` sí es reconstrueix una base real en framework
- en `R3` sí es migren o implementen almenys `2` fluxos end-to-end
- almenys `1` flux ha de ser heretat de `R2`
- el segon flux pot ser heretat o una ampliació funcional xicoteta, però no cosmètica

L'objectiu no és dominar tot el framework. L'objectiu és entendre com el framework aporta estructura, persistència, eines, convencions, mantenibilitat i verificació. Per això cal usar eines pròpies de l'stack: generació de projecte, sistema de rutes, controladors, plantilles, ORM o capa de dades, migracions o equivalent, fixtures/seeders o càrrega reproduïble, validació, proves i configuració d'entorn.

La nomenclatura concreta depén de l'stack. En este repte es valoren criteris comuns, no noms Laravel:

| Criteri comú | Laravel | Symfony | NestJS |
|---|---|---|---|
| Ruta | route | route | controller route |
| Controlador | controller | controller | controller |
| Vista/resposta | Blade/view | Twig/Response | template/response o resposta server-rendered equivalent |
| Model/capa de dades | Eloquent model | Doctrine entity/repository | Prisma/TypeORM entity, schema o service |
| Migració d'esquema | migration | Doctrine migration | Prisma/TypeORM migration o equivalent |
| Dades inicials | seeder | fixture | seed script o seeder |
| Validació | Form Request/validator | Validator/Form | DTO + class-validator o equivalent |
| Configuració | `.env` | `.env` | `.env` |

No es considera suficient:

- parlar d'`MVC` sense producte executable
- crear carpetes amb noms correctes però sense fluxos reals
- moure fitxers de `R2` dins del framework sense adaptar responsabilitats
- usar una base de dades només decorativa
- carregar dades a mà sense mecanisme reproduïble
- presentar una demo que no es puga arrancar des de zero

## 3.1 Seqüència interna i límit de càrrega

Per evitar que `R3` es convertisca en un repte monstre, la seqüència interna recomanada és:

- primer, base en framework arrancable amb `Docker`, `.env` i rutes mínimes
- després, persistència mínima real amb migracions/fixtures/seeders o script equivalent i conjunt de dades usable
- després, primer flux heretat de `R2` amb resposta **server-rendered**
- finalment, segon flux o ampliació curta, proves mínimes, `README` i backlog del que queda fora

Si apareix tensió de calendari, no s'ha de retallar la base tècnica ni el primer flux **server-rendered**. El que es reduïx és l'ambició funcional del segon flux, no la verificabilitat del repte.

---

## 4. Paper de la IA en este repte

La IA es pot usar per a:

- comparar convencions bàsiques de `Laravel`, `Symfony`, `NestJS` o una via excepcional autoritzada
- suggerir passos d'arrencada del projecte
- ajudar a dissenyar un model de dades inicial
- proposar migracions, fixtures/seeders o scripts equivalents, DTO, formularis, validacions o proves segons l'stack
- detectar incoherències entre rutes, controladors, models i vistes
- ajudar a redactar documentació tècnica i decisions

L'alumnat no pot delegar:

- la decisió de quins `2` casos d'ús entren en `R3`
- la justificació de quin cas d'ús ve de `R2`
- la comprovació real de Docker, BBDD, migracions o equivalent i càrrega reproduïble de dades
- la defensa de com circula una petició pel framework
- la verificació que les dades es lliguen i s'escriuen realment
- la decisió sobre què queda fora de la migració total

El risc principal és acceptar una estructura generada que parega professional però que no arranque, no use dades reals o no resolga cap flux complet. Les mesures de control són `AI log` quan corresponga, commits revisables, execució en directe, proves mínimes, preguntes de transferència i contrast entre `README`, codi i comportament observat.

---

## 5. Estructura del repte

### 5.1 Nucli del repte

**Objectiu del nucli**

Construir una nova base en framework, reproduïble i operativa, amb persistència mínima real i `2` casos d'ús end-to-end verificables.

**Lliurable principal**

Aplicació en framework que incloga:

- `Docker` i instruccions d'arrencada
- projecte base del framework arrancable
- configuració `.env` documentada
- base de dades creada per migracions o mecanisme equivalent de l'stack
- dades inicials creades per fixtures/seeders o script equivalent
- `2` casos d'ús funcionals de punta a punta
- almenys `1` cas d'ús migrat de `R2`
- almenys `1` cas d'ús renderitzat en servidor amb vista o plantilla
- validació i errors mínims
- proves mínimes
- documentació tècnica curta
- mapa o backlog del que quedaria per migrar després

**Criteris d'avaluació principals del nucli**

- CA de **RA5** vinculats a estructura del framework, separació de responsabilitats, rutes, controladors, vistes o equivalents i mantenibilitat del flux
- CA de **RA6** vinculats a connexió, recuperació, persistència, integritat bàsica, verificació i tractament d'errors sobre dades reals
- CA de **RA8** vinculats a ús de framework servidor, generació dinàmica de pàgines, vistes o plantilles, formularis i resposta HTML renderitzada en servidor

**Evidències obligatòries del nucli**

- repositori actualitzat
- issue principal de `R3` i microtasques
- seqüència de commits significativa
- un commit rellevant comentat sobre la migració d'un flux o una decisió d'estructura
- aplicació arrancant amb Docker
- `.env.example` o instruccions equivalents
- migracions o mecanisme equivalent executable
- fixtures/seeders o script de càrrega executable
- captura o registre d'arrencada i càrrega de dades
- demo dels `2` casos d'ús end-to-end
- almenys `1` cas d'ús migrat des de `R2`
- evidència d'un cas d'ús server-rendered amb vista o plantilla que rep dades reals
- proves mínimes executades
- nota tècnica de decisió o justificació breu de migració
- README tècnic actualitzat i centrat en decisions
- mini defensa tècnica als checkpoints `CP-R3A` i `CP-R3B`
- AI log quan hi haja ús d'IA

---

## 6. Microprojectes i microtasques del repte

> **Norma del repte**
>
> - Els microprojectes han de produir software executable, no només diagnosi o discurs.
> - Cap microprojecte apareix sense el camp **“RA avaluat, CA avaluats i RA de context”**.
> - No es demana migrar tota l'aplicació de `R2`.
> - Sí es demana una base real en framework i almenys `2` fluxos end-to-end.
> - El framework s'ha d'usar amb eines pròpies, no com a decorat.

### Microrepte R3M1 — Arrencada del nou projecte

**Tipus**

Microprojecte d'infraestructura i decisió tècnica.

**Objectiu**

Triar l'stack, crear el projecte base en framework, preparar Docker i demostrar que l'entorn arranca de manera reproduïble.

**Tasca**

L'equip ha de:

- triar `Laravel`, `Symfony`, `NestJS` o via excepcional autoritzada
- comparar el framework triat amb almenys una altra opció viable per a este repte
- justificar per què el framework triat ajuda a separar millor ruta, controlador, vista o resposta i model o equivalents
- identificar quins avantatges aporta eixa separació respecte a la base funcional heretada de `R2`
- crear o reorganitzar el projecte base del framework
- preparar `Docker` i serveis necessaris
- configurar `.env` i documentar variables mínimes
- definir primeres rutes mínimes
- comprovar arrencada real de l'aplicació
- obrir issue principal de `R3` amb microtasques
- declarar quins `2` casos d'ús es treballaran i quin ve de `R2`

**Relació amb el producte principal**

Sense una base arrancable i reproduïble, la resta del repte queda convertida en fragments no verificables.

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA5**
- **CA avaluats**: **RA5.a**, **RA5.b**, **RA5.c**, **RA5.d**, **RA5.e**
- **RA de context**: **RA8.c**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat identifica avantatges concrets de separar presentació, entrada, coordinació i lògica respecte a la base de `R2`.
- L'alumnat compara mecanismes o frameworks i justifica la tria segons les seues característiques principals.
- L'alumnat identifica l'estructura del framework triat i les responsabilitats bàsiques.
- L'alumnat obri una primera entrada real al framework servidor amb ruta i resposta generada.
- L'alumnat prepara una base tècnica coherent per separar entrada, control, lògica i presentació.
- L'alumnat justifica un abast viable de migració sense convertir `R3` en una reescriptura total.

**Paper de la IA**

La IA pot suggerir comandos d'arrencada, estructura inicial o riscos d'instal·lació, però l'alumnat ha de comprovar l'execució real en el seu entorn.

**Evidències obligatòries**

- projecte base del framework al repositori
- nota comparativa curta del framework triat amb almenys una alternativa
- esquema abans/després entre la base de `R2` i la nova estructura en framework
- justificació breu dels avantatges de separar presentació i lògica
- `Dockerfile`, `compose.yaml` o equivalent funcional
- `.env.example` o instruccions de configuració
- ruta inicial o `healthcheck`
- primera resposta generada pel framework, preferentment HTML o vista mínima quan l'stack ho permeta
- registre d'arrencada
- issue principal amb els `2` casos d'ús declarats

**Instrument d'avaluació**

Checklist d'arrencada tècnica i revisió de repositori.

**Indicadors d'assoliment**

- l'aplicació arranca amb instruccions reproduïbles
- el framework no és un esquelet buit: ja té rutes mínimes
- l'abast de `R3` està acotat i inclou `2` fluxos

**Riscos habituals**

- perdre sessions en instal·lació sense producte
- no documentar `.env`
- no declarar quin cas d'ús ve de `R2`
- confondre arrencada del framework amb repte complet

**Verificació del treball real**

- execució en directe de l'arrencada
- pregunta oral sobre serveis de Docker i punt d'entrada del framework

**Pes orientatiu dins del repte**

12%

---

### Microrepte R3M2 — Model de dades i persistència mínima

**Tipus**

Microprojecte procedimental de dades.

**Objectiu**

Crear l'esquema de dades inicial, connectar-lo amb l'aplicació i deixar dades de prova reproduïbles.

**Tasca**

L'equip ha de:

- definir l'esquema mínim de dades per als fluxos triats
- crear migracions o mecanisme equivalent
- configurar connexió a la base de dades
- crear fixtures/seeders o script equivalent
- carregar dades de demostració reproduïbles
- comprovar lectura real des de l'aplicació o consola del framework
- recuperar un conjunt de dades real des de la BBDD
- tractar eixe conjunt de dades de manera estructurada dins del framework
- preparar-lo perquè alimente una vista, llistat, detall, filtre o resposta equivalent
- documentar com reiniciar BBDD i dades

**Relació amb el producte principal**

La base del framework ha de treballar amb una BBDD real des del començament. La persistència no pot aparéixer al final com un afegit decoratiu.

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA6**
- **CA avaluats**: **RA6.a**, **RA6.b**, **RA6.c**, **RA6.d**, **RA6.e**
- **RA de context**: **RA5.f**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat connecta l'aplicació a un magatzem de dades real.
- L'alumnat crea i evoluciona l'estructura de dades amb eines del framework.
- L'alumnat deixa dades inicials que permeten provar els fluxos sense preparació manual.
- L'alumnat recupera un conjunt de dades i el tracta de manera ordenada perquè alimente un flux funcional.

**Paper de la IA**

La IA pot ajudar a proposar camps, relacions, migracions, fixtures/seeders o scripts equivalents, però l'alumnat ha de validar que el model serveix als casos d'ús triats i que les dades es creen realment.

**Evidències obligatòries**

- fitxers de migració o mecanisme equivalent
- fitxers de fixtures/seeders o script equivalent
- BBDD creada des de zero
- dades inicials carregades
- comprovació de lectura real
- consulta real que retorne un conjunt de dades
- ús del conjunt de dades en un llistat, filtre, detall o resposta equivalent
- demostració o prova que la informació recuperada arriba correctament al flux funcional
- instruccions de reset o recàrrega de dades

**Instrument d'avaluació**

Rúbrica de persistència mínima i dades reproduïbles.

**Indicadors d'assoliment**

- l'esquema no és genèric: respon als fluxos de `R3`
- les dades es poden regenerar
- l'aplicació llig dades reals, no arrays o valors incrustats
- el conjunt de dades recuperat arriba a una vista, resposta o flux funcional amb estructura comprensible

**Riscos habituals**

- crear taules que no s'usen en cap flux
- carregar dades manualment sense mecanisme reproduïble
- usar persistència simulada
- no saber explicar la relació entre model i cas d'ús

**Verificació del treball real**

- esborrar o reiniciar BBDD i tornar a executar migracions i càrrega inicial reproduïble
- mostrar una lectura real des de l'aplicació i el seu ús dins d'un flux

**Pes orientatiu dins del repte**

18%

---

### Microrepte R3M3 — Primer cas d'ús complet

**Tipus**

Microprojecte procedimental de migració funcional.

**Objectiu**

Migrar o reconstruir dins del framework el primer cas d'ús complet, obligatòriament heretat de `R2`.

**Tasca**

L'equip ha de implementar el flux amb:

- ruta
- controlador o equivalent
- model, servei o capa de dades
- vista o plantilla server-rendered sempre que siga possible; com a mínim una resposta HTML generada pel servidor en un dels casos d'ús de `R3`
- lectura real des de BBDD
- dades passades des del controlador a la vista o plantilla
- formulari, paràmetre o interacció processada pel framework quan el flux ho permeta
- validació mínima si escau
- error bàsic controlat
- prova o verificació mínima del recorregut

**Relació amb el producte principal**

Este microprojecte demostra que el pas al framework no ha trencat el projecte anterior i que la migració és funcional, no només estructural.

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA8**
- **CA avaluats**: **RA8.d**, **RA8.e**, **RA8.g**
- **RA de context**: **RA5.e**, **RA5.f**, **RA5.g**, **RA6.c**, **RA6.d**, **RA6.f**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat separa entrada, coordinació, dades i presentació amb eines del framework.
- L'alumnat conserva o reconstrueix un flux real de `R2` amb persistència real.
- L'alumnat genera una pàgina o resposta HTML dinàmica des del framework amb dades reals.
- L'alumnat processa una interacció d'usuari o formulari i retorna una resposta renderitzada.
- L'alumnat verifica comportament positiu i error mínim.

**Paper de la IA**

La IA pot ajudar a generar esquelets de ruta, controlador, servei, DTO, formulari o plantilla, però l'alumnat ha de comprovar que el flux correspon al cas d'ús real de `R2`.

**Evidències obligatòries**

- identificació del cas d'ús heretat de `R2`
- ruta funcional
- controlador o equivalent
- model/servei/capa de dades implicada
- vista/plantilla/resposta funcional
- pàgina renderitzada pel servidor a partir de dades reals
- dades passades del controlador a la vista o plantilla
- formulari processat pel framework o interacció equivalent amb resposta HTML
- lectura de dades reals
- validació mínima si aplica
- prova o verificació del cas positiu
- evidència d'error controlat

**Instrument d'avaluació**

Rúbrica de flux end-to-end migrat.

**Indicadors d'assoliment**

- el flux s'executa de punta a punta
- almenys este flux o un altre de `R3` és clarament server-rendered
- les dades provenen de BBDD
- les responsabilitats són recognoscibles
- l'equip pot comparar què aportava `R2` i què aporta ara el framework

**Riscos habituals**

- portar només una pantalla sense lògica real
- deixar la lectura de dades simulada
- posar tota la lògica dins del controlador
- no verificar un error mínim

**Verificació del treball real**

- execució en directe del flux
- pregunta oral sobre el recorregut de la petició pel framework

**Pes orientatiu dins del repte**

18%

---

### Microrepte R3M4 — Segon cas d'ús o ampliació funcional

**Tipus**

Microprojecte procedimental d'ampliació controlada.

**Objectiu**

Construir un segon flux end-to-end que complete el mínim funcional del repte i faça visible el valor del framework.

**Tasca**

L'equip ha de implementar una de les dues opcions:

- segon cas d'ús migrat des de `R2`
- ampliació funcional xicoteta i útil sobre el primer flux

En qualsevol cas, ha de ser un flux real, amb recorregut end-to-end, i no un canvi cosmètic. Pot incloure, segons el domini:

- alta, edició, canvi d'estat o filtratge d'un recurs
- vista de detall amb dades relacionades
- operació protegida del domini
- validació més significativa
- ús d'una relació simple entre entitats

**Relació amb el producte principal**

El segon flux evita que `R3` quede reduït a una demo única. Obliga a comprovar que la base del framework suporta creixement mínim.

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA8**
- **CA avaluats**: **RA8.f**, **RA8.g**
- **RA de context**: **RA5.e**, **RA5.f**, **RA5.g**, **RA5.h**, **RA6.c**, **RA6.d**, **RA6.f**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat reutilitza l'estructura del framework per afegir o migrar funcionalitat.
- L'alumnat comprova que la persistència i les capes creades no serveixen només per a un cas aïllat.
- L'alumnat modifica dinàmicament el contingut generat segons dades, paràmetres, estat, filtre o formulari.
- L'alumnat diferencia ampliació funcional real de canvi visual.

**Paper de la IA**

La IA pot suggerir una ampliació viable i proves associades, però l'alumnat ha de justificar per què aporta valor al producte i al framework triat.

**Evidències obligatòries**

- descripció del segon flux
- justificació de si és migració o ampliació
- ruta i controlador o equivalents
- interacció amb BBDD
- canvi visible en el contingut generat segons dades, paràmetres, estat, filtre o formulari
- vista, plantilla o resposta HTML si este és el flux triat com a server-rendered
- validació o error mínim
- prova o verificació mínima
- demo end-to-end

**Instrument d'avaluació**

Checklist de segon flux funcional i revisió de valor.

**Indicadors d'assoliment**

- el segon flux és executable
- no és només una vista nova o canvi d'estil
- aprofita estructura, validació, dades o convencions del framework
- amplia la base sense duplicar codi sense criteri

**Riscos habituals**

- afegir una pàgina estàtica
- duplicar el primer flux canviant noms
- obrir una funcionalitat massa gran
- perdre estabilitat del primer cas d'ús

**Verificació del treball real**

- execució en directe dels dos fluxos
- pregunta oral sobre què ha fet més fàcil o més ordenat el framework

**Pes orientatiu dins del repte**

12%

---

### Microrepte R3M5 — Autenticació, autorització i middleware

**Tipus**

Microprojecte procedimental de seguretat aplicada al framework.

**Objectiu**

Traslladar l'autenticació treballada en `R2` a les eines pròpies del framework i protegir una acció significativa amb autorització mínima.

**Tasca**

L'equip ha de:

- implementar login o mecanisme d'autenticació amb eines del framework
- implementar logout o invalidació de sessió/token
- crear o documentar un usuari demo reproduïble
- protegir una ruta o acció significativa del domini
- usar middleware, guard, voter, policy o equivalent segons l'stack
- definir una regla d'autorització mínima: rol, propietari del recurs, estat o permís simple
- provar accés sense autenticar
- provar accés autoritzat
- provar accés denegat
- documentar com verificar la protecció

**Relació amb el producte principal**

`R3` no pot quedar com una reconstrucció pública de fluxos que en `R2` ja eren protegits. El valor del framework és usar les seues peces de seguretat per fer explícita la diferència entre autenticació, autorització i protecció de ruta.

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA5**
- **CA avaluats**: **RA5.f**, **RA5.g**, **RA5.h**
- **RA de context**: **RA6.f**, **RA8.g**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat usa mecanismes del framework per controlar accés.
- L'alumnat diferencia estar autenticat de tindre permís.
- L'alumnat verifica comportament autoritzat i denegat.
- L'alumnat evita proteccions només visuals.

**Paper de la IA**

La IA pot ajudar a comparar middleware, guard, voter o policy, però l'alumnat ha de decidir quina acció protegir i demostrar que el control està en servidor.

**Evidències obligatòries**

- login o mecanisme d'autenticació funcional
- logout o invalidació
- usuari demo reproduïble
- ruta o acció protegida
- middleware, guard, voter, policy o equivalent
- regla d'autorització mínima vinculada al domini
- cas autoritzat i cas denegat
- error o resposta controlada quan no hi ha permisos
- instruccions de prova

**Instrument d'avaluació**

Rúbrica d'autenticació, autorització i middleware.

**Indicadors d'assoliment**

- la protecció està en servidor
- l'acció protegida té valor real dins del projecte
- hi ha diferència observable entre usuari autoritzat i no autoritzat
- les credencials demo no exposen secrets reals
- la solució usa convencions del framework triat

**Riscos habituals**

- ocultar botons però deixar la ruta accessible
- fer login sense autorització
- crear rols que no protegeixen cap acció
- no provar el cas denegat
- versionar secrets o contrasenyes personals

**Verificació del treball real**

- accedir a la ruta protegida sense autenticar
- fer login amb usuari autoritzat
- provar l'acció protegida
- provar denegació amb usuari sense permís o estat no vàlid
- fer logout i repetir l'accés

**Pes orientatiu dins del repte**

15%

---

### Microrepte R3M6 — Qualitat i estabilització

**Tipus**

Microprojecte procedimental de qualitat mínima.

**Objectiu**

Estabilitzar la base reconstruïda perquè no siga només una demo funcional, sinó un punt de partida mantenible per a `R4`.

**Tasca**

L'equip ha de:

- revisar estructura de rutes, controladors, serveis i models o equivalents
- eliminar duplicacions evidents
- netejar controladors massa carregats
- reforçar validació mínima
- tractar errors bàsics
- afegir proves bàsiques dels fluxos
- comprovar dades de demostració reproduïbles
- revisar que migracions i fixtures/seeders o equivalent continuen funcionant

**Relació amb el producte principal**

La qualitat mínima és el que separa una reconstrucció productiva d'un prototip fràgil.

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA5**
- **CA avaluats**: **RA5.g**, **RA5.h**
- **RA de context**: **RA6.f**, **RA6.g**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat ajusta responsabilitats i evita que el framework s'use de forma desordenada.
- L'alumnat prova els fluxos principals i controla errors mínims.
- L'alumnat manté coherència entre estructura, dades i comportament.

**Paper de la IA**

La IA pot suggerir casos de prova, detectar duplicacions o proposar missatges d'error, però les proves i correccions s'han d'executar i entendre.

**Evidències obligatòries**

- proves mínimes executables o verificacions registrades
- cas positiu i cas negatiu dels fluxos principals
- tractament visible d'errors
- revisió de controladors/responsabilitats
- comprovació de migracions/fixtures/seeders o script equivalent
- incidències detectades i corregides

**Instrument d'avaluació**

Checklist de qualitat mínima i proves.

**Indicadors d'assoliment**

- els dos fluxos continuen funcionant després de la neteja
- les validacions i errors són observables
- les proves no són fictícies
- l'estructura és explicable sense recórrer a frases genèriques

**Riscos habituals**

- proves manuals no reproduïbles
- errors sense tractament
- controladors que acumulen tota la lògica
- trencar migracions o càrrega inicial en refactoritzar

**Verificació del treball real**

- execució en directe de proves o checklist verificable
- provocació d'un error i revisió de la resposta del sistema

**Pes orientatiu dins del repte**

12%

---

### Microrepte R3M7 — Tancament tècnic

**Tipus**

Microprojecte de tancament i defensa.

**Objectiu**

Deixar el projecte en framework documentat, reproduïble i preparat per decidir què s'exposarà com a `API` en `R4`.

**Tasca**

L'equip ha de:

- actualitzar `README`
- explicar instruccions d'arrencada
- documentar migracions/fixtures/seeders o mecanisme equivalent i dades inicials
- descriure els `2` casos d'ús implementats
- documentar la ruta o acció protegida i la regla d'autorització
- registrar decisions tècniques principals
- preparar una demostració curta
- deixar backlog o mapa del que quedaria per migrar de `R2`
- identificar què podria convertir-se en recurs o endpoint de `R4`

**Relació amb el producte principal**

El tancament tècnic fa visible que `R3` no és una migració total, sinó una reconstrucció acotada i verificable que deixa una base de continuïtat.

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA5**
- **CA avaluats**: **RA5.f**, **RA5.g**
- **RA de context**: **RA6.g**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat documenta una arquitectura real i no una intenció.
- L'alumnat explica com arrancar, provar i continuar el projecte.
- L'alumnat identifica què queda fora sense ocultar-ho com a deute invisible.

**Paper de la IA**

La IA pot ajudar a ordenar la documentació, però el contingut ha de correspondre exactament al projecte real i a les decisions preses.

**Evidències obligatòries**

- `README` tècnic actualitzat
- instruccions d'arrencada amb Docker
- instruccions de BBDD, migracions/fixtures/seeders o mecanisme equivalent
- resum dels `2` casos d'ús
- decisions tècniques breus
- backlog del que quedaria per migrar
- demostració final

**Instrument d'avaluació**

Rúbrica de documentació i defensa tècnica.

**Indicadors d'assoliment**

- una altra persona pot arrancar el projecte
- el README coincideix amb el codi
- queda clar què s'ha migrat, què s'ha ampliat i què queda fora
- el pas a `R4` està justificat

**Riscos habituals**

- documentació embellida però no executable
- ocultar que només s'han migrat parts del projecte
- no explicar decisions tècniques
- no deixar mapa de continuïtat

**Verificació del treball real**

- seguir el README per arrancar el projecte
- defensa curta sobre els `2` fluxos, la BBDD i el backlog

**Pes orientatiu dins del repte**

13%

---

## 7. Taula resum de microprojectes i criteris d'avaluació

| Microprojecte | Tipus | Producte o lliurable | RA avaluat | CA avaluats | RA de context | Evidències principals | Instrument | Pes orientatiu |
|---|---|---|---|---|---|---|---|---:|
| R3M1 | Infraestructura / decisió tècnica | Projecte en framework arrancable amb Docker | RA5 | RA5.a, RA5.b, RA5.c, RA5.d, RA5.e | RA8.c | comparativa de stack, esquema abans/després, Docker, `.env`, ruta inicial, resposta generada, issue i abast de 2 fluxos | checklist | 12% |
| R3M2 | Persistència mínima | Model de dades inicial amb migracions/fixtures/seeders o mecanisme equivalent i conjunt de dades usable | RA6 | RA6.a, RA6.b, RA6.c, RA6.d, RA6.e | RA5.f | BBDD creada, dades carregades, consulta de conjunt de dades i ús en flux | rúbrica | 18% |
| R3M3 | Migració funcional | Primer cas d'ús complet heretat de R2 | RA8 | RA8.d, RA8.e, RA8.g | RA5.e, RA5.f, RA5.g, RA6.c, RA6.d, RA6.f | ruta, controlador, model/servei, vista/plantilla server-rendered, formulari o interacció, prova | rúbrica | 18% |
| R3M4 | Ampliació funcional | Segon flux end-to-end o ampliació útil | RA8 | RA8.f, RA8.g | RA5.e, RA5.f, RA5.g, RA5.h, RA6.c, RA6.d, RA6.f | segon flux, BBDD, canvi dinàmic de resposta, validació/error i demo | checklist | 12% |
| R3M5 | Seguretat de framework | Autenticació, autorització i middleware | RA5 | RA5.f, RA5.g, RA5.h | RA6.f, RA8.g | login, acció protegida, cas autoritzat i denegat | rúbrica | 15% |
| R3M6 | Qualitat | Estabilització, validació, errors i proves | RA5 | RA5.g, RA5.h | RA6.f, RA6.g | proves, cas positiu/negatiu, errors, neteja i protecció intacta | checklist | 12% |
| R3M7 | Tancament | README, decisions, demo i backlog de migració | RA5 | RA5.f, RA5.g | RA6.g | documentació, demo, mapa del que queda i acció protegida | rúbrica | 13% |

---

## 8. Evidències globals del repte

**Evidències mínimes comunes**

- repositori actualitzat
- issue principal amb microtasques
- seqüència de commits significativa
- aplicació en framework operativa
- Docker funcional
- configuració mínima i `.env.example` o equivalent
- rutes, controladors i vistes/plantilles/respostes segons l'stack
- models, entitats, esquemes o capa equivalent de dades
- BBDD real
- migracions o mecanisme equivalent
- fixtures/seeders o script equivalent
- dades de demostració reproduïbles
- `2` casos d'ús end-to-end
- almenys `1` cas d'ús migrat des de `R2`
- almenys `1` cas d'ús server-rendered amb vista o plantilla
- autenticació amb eines del framework
- acció protegida amb middleware, guard, voter, policy o equivalent
- cas autoritzat i cas denegat
- validació i errors mínims
- proves mínimes
- documentació tècnica curta
- backlog o mapa del que quedaria per migrar
- AI log quan hi haja ús d'IA

**Evidències opcionals d'ampliació**

- més de `2` casos d'ús migrats
- relacions de dades més riques
- més cobertura de proves
- millor gestió d'errors
- autenticació més integrada amb el framework si el grup ja té base sòlida
- primer esborrany de contracte d'`API` per a `R4`

---

## 9. Duració orientativa i organització

Duració orientativa:

- `8` a `10` sessions
- recomanació preferent: `10` sessions de `3` hores, incloent el taller de portabilitat entre frameworks

Seqüència recomanada:

| Tram | Sessions | Microprojectes principals | Sentit docent |
|---|---:|---|---|
| Arrencada | `1` | `R3M1` | triar stack, Docker, projecte base i rutes mínimes |
| Persistència inicial | `2` | `R3M2` | model de dades, migracions/fixtures/seeders o mecanisme equivalent i BBDD real |
| Taller de portabilitat | `2B` | reforç `R3M1-R3M2` | equivalències entre frameworks i auditoria abans del primer flux |
| Primer flux | `3-4` | `R3M3` | migrar el primer cas d'ús heretat de `R2` |
| Segon flux | `5` | `R3M4` | completar un segon flux o ampliació funcional útil |
| Seguretat de framework | `6` | `R3M5` | autenticació, autorització i middleware |
| Qualitat | `7-8` | `R3M6` | validació, errors, proves i neteja d'estructura |
| Tancament | `9` | `R3M7` | README, demo, decisions i backlog de migració |

Si el calendari obliga a compactar, no s'ha de retallar l'exigència dels `2` fluxos, Docker, BBDD, migracions o equivalent i dades inicials reproduïbles. El que es pot reduir és l'abast funcional de cada flux.

---

## 10. Orientacions per itinerari

**Laravel**

- rutes en `routes/web.php` o `routes/api.php` si escau
- controladors amb responsabilitat limitada
- `Request` o validació pròpia de Laravel
- models Eloquent
- migracions/fixtures/seeders o mecanisme equivalent
- Blade o resposta equivalent
- proves amb l'eina de testing del projecte

**Symfony**

- rutes amb atributs o configuració
- controladors
- serveis
- entitats i repositoris amb Doctrine
- migracions
- fixtures com a mecanisme de dades inicials en Symfony
- Twig o resposta equivalent
- proves bàsiques amb l'eina del projecte

**NestJS**

- mòduls
- controladors
- serveis
- DTO i validació
- entitats/esquemes segons ORM o ODM triat
- migracions o mecanisme equivalent de l'eina de dades
- seeders o script reproduïble de càrrega inicial
- proves bàsiques amb l'eina del projecte

La nomenclatura pot variar, però el criteri no: base arrancable, dades reals, dos fluxos end-to-end i responsabilitats defensables.

---

## 11. Errors habituals que invaliden o debiliten el repte

- migrar només fitxers sense adaptar-los al framework
- deixar una base de framework que arranca però no té fluxos
- fer només un cas d'ús
- no garantir que almenys un flux ve de `R2`
- crear BBDD sense migracions o mecanisme equivalent
- carregar dades manualment sense fixtures/seeders o script equivalent
- no tractar errors
- no poder reiniciar l'entorn des de zero
- escriure documentació que no coincideix amb el projecte
- confondre ampliació funcional amb canvi visual

---

## 12. Condició de tancament del repte

`R3` es considera tancat quan es pot demostrar:

- l'aplicació en framework arranca amb Docker
- la BBDD es crea amb migracions o mecanisme equivalent
- les dades inicials es carreguen amb fixtures/seeders o script equivalent
- hi ha `2` casos d'ús end-to-end funcionals
- almenys `1` cas d'ús ve de `R2`
- almenys `1` cas d'ús genera resposta HTML renderitzada en servidor amb vista o plantilla
- hi ha validació i errors mínims
- hi ha proves mínimes o verificacions reproduïbles
- el README permet arrancar i provar el projecte
- queda documentat què s'ha migrat i què queda pendent
- el projecte està preparat per decidir recursos i contracte d'`API` en `R4`

El repte no queda tancat si només hi ha arquitectura explicada, si només hi ha esquelet del framework o si la persistència no es pot reconstruir des de zero.

---

## 13. Ampliació 9→10

**Finalitat**

Aprofundir `R3` amb una millora tècnica real sobre mantenibilitat del flux, qualitat arquitectònica, proves o operativitat del backend en framework.

**Condició prèvia**

El nucli obligatori del repte ha d'estar complet, funcional i validat.

**Opcions d’ampliació**

- afegir paginació, filtrat o cerca amb criteri de mantenibilitat i documentació clara del flux
- reforçar proves, autorització o refactorització `MVC` amb justificació tècnica breu sobre per què la nova versió és millor

**Ampliació proposada per l’alumne/a**

També es pot proposar una ampliació pròpia si està alineada amb el repte i es valida prèviament amb el professorat.

**Paper de la IA**

La IA es pot usar per contrastar enfocaments d'arquitectura, proves o refactorització, però l'alumnat ha d'aportar decisió, validació i defensa pròpia.

**Evidències**

- commit o branca identificable
- nota tècnica de decisió o justificació tècnica breu
- prova funcional o demo
- README tècnic actualitzat si l'ampliació afecta el flux
- rastre de l'ús de la IA, si n'hi ha hagut
- mini defensa tècnica o preguntes de contrast

**Instruments de verificació**

- checklist curta d'ampliació
- revisió de repositori
- prova funcional guiada
- mini defensa tècnica als checkpoints o al tancament

**Perquè compute com a 9→10**

- el nucli està ben resolt
- l’ampliació aporta mantenibilitat, qualitat o robustesa reals
- es pot explicar i defensar
- no és ornamental
- no hi ha delegació excessiva en IA
