# R3S2. Persistencia minima amb migrations i seeders

## Finalitat de la sessio

Esta sessio converteix la base arrancable de `R3M1` en una aplicacio amb BBDD real i dades reproduïbles. El centre no és dissenyar tot el model final, sinó crear un esquema minim que servisca als `2` fluxos declarats i que es puga reconstruir amb `migrations` i `seeders` o equivalents.

## Encaix dins del Repte 3

- **Repte**: `R3. Reconstruccio en framework, persistencia real i primers fluxos funcionals`
- **Microrepte**: `R3M2`
- **Sessio**: `R3S2`
- **Duracio orientativa**: `3 hores`
- **Focus**: connexio a BBDD, esquema minim, migracions, seeders, lectura real i conjunt de dades usable
- **No entra encara**: model complet de tot el producte, relacions complexes, optimitzacio, API o permisos avançats

## Relacio amb RA i criteris de treball

| Element | Concrecio en el microrepte |
|---|---|
| `RA6.a` | configura connexio a un magatzem de dades real |
| `RA6.b` | defineix estructura inicial de dades |
| `RA6.c` | recupera dades reals des de l'aplicacio |
| `RA6.d` | tracta dades recuperades de manera ordenada |
| `RA6.e` | deixa dades inicials reproduïbles |
| `RA5.f` | connecta persistencia amb estructura del framework |
| Evidencia central | BBDD reconstruïble amb dades que alimenten un flux |

## Producte esperat

- Connexio de BBDD configurada.
- Migracions executables.
- Seeders, fixtures o script equivalent.
- Dades de prova vinculades als fluxos.
- Lectura real des de l'aplicacio o consola.
- Conjunt de dades preparat per a llistat, detall, filtre o resposta.
- Instruccions per reiniciar BBDD i carregar dades.

## Preparacio previa del professorat

- Preparar exemple de migracio simple.
- Preparar exemple de seeder o fixture.
- Tindre pauta de model minim: camps necessaris, no inventari complet.
- Preparar comprovacio de reset de BBDD.
- Definir exemples de dades suficients per a llistat/detall.

## Continguts a explicar

- Diferencia entre persistencia real i arrays de prova.
- Relacio entre flux, entitat, migracio, model i seeder.
- Per que les dades manuals no són evidència suficient.
- Com recuperar un conjunt de dades i preparar-lo per a una resposta.
- Com documentar comandes de migracio i seed.

## Sequencia d'aula de 3 hores

### 0:00-0:25. Recuperacio de R3M1 i fluxos

Tasques:

- comprovar que el projecte arranca;
- revisar els `2` fluxos declarats;
- identificar entitats o taules minimes;
- descartar camps que no s'usaran.

### 0:25-0:55. Modelatge docent

El professorat mostra:

- una migracio simple;
- un model o entitat;
- un seeder;
- una lectura real;
- reset complet de BBDD.

### 0:55-1:45. Implementacio d'esquema

Tasques:

- configurar connexio;
- crear migracions;
- executar-les;
- revisar estructura creada;
- registrar decisions de camps.

### 1:45-2:25. Dades inicials i lectura

Tasques:

- crear seeders o fixtures;
- carregar dades;
- recuperar un conjunt de dades;
- preparar-lo per a vista, llistat, filtre, detall o resposta.

### 2:25-2:50. Verificacio i documentacio

Tasques:

- reiniciar BBDD;
- executar migracions i seeders;
- documentar comandes;
- registrar evidencies i temps.

### 2:50-3:00. Checkpoint

Cada equip mostra:

- migracions;
- seeders;
- dades carregades;
- lectura real;
- instruccions de reset.

## Tasques concretes de l'alumnat

- Definir esquema minim.
- Configurar connexio.
- Crear i executar migracions.
- Crear seeders o equivalents.
- Recuperar conjunt de dades.
- Preparar eixe conjunt per alimentar un flux.
- Documentar reset i carrega.

## Evidencies minimes

| Evidencia | Minim acceptable |
|---|---|
| BBDD | creada des de migracions |
| Dades | carregades amb seeder o equivalent |
| Lectura | consulta real que retorna conjunt de dades |
| Us | dades preparades per a un flux |
| Documentacio | comandes de migracio i seed |
| Traçabilitat | commits i registre de temps aproximat |

## Criteris d'exit

- La BBDD es pot reconstruir de zero.
- Les taules responen als fluxos triats.
- Les dades no es carreguen manualment.
- La lectura no queda aïllada: alimenta o prepara un flux.
- L'alumnat pot explicar per que ha triat eixos camps.

## Que no és suficient

- Crear taules sense us.
- Fer una BBDD manual fora del repositori.
- Posar dades en arrays.
- No documentar comandes.
- Fer una consulta solta que no arriba a cap flux.

## Us de la IA

La IA pot ajudar amb camps, migracions, seeders i errors de connexio. L'alumnat ha de validar que el model respon al seu domini i que la BBDD es pot reconstruir.

## Suport per a alumnat amb dificultats

- Reduir a una entitat principal i dades minimes.
- Donar exemple de migracio equivalent a l'stack.
- Revisar `.env` i serveis de BBDD.
- Proposar `3-5` registres de prova suficients.

## Ampliacio per a alumnat avançat

- Afegir una relacio simple si aporta valor al flux.
- Crear factory o fixture més completa.
- Afegir comprovacio automatica de migracio i seed.

## Checklist de tancament

- [ ] Connexio configurada.
- [ ] Migracions executades.
- [ ] Seeders o equivalents funcionen.
- [ ] Hi ha lectura real.
- [ ] Les dades alimenten o preparen un flux.
- [ ] Hi ha instruccions de reset.
- [ ] Hi ha commits i temps aproximat.

## Connexio amb el microrepte posterior

`R3M3` utilitzara esta persistencia per reconstruir un primer cas d'us complet heretat de `R2`. Sense dades reals, el flux quedara com una pantalla o demo ficticia.

