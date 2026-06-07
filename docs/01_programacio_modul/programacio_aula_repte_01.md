# R1. Programació d'aula - Kickoff backend

## Finalitat

El `Repte 1` inicia el treball de backend amb una base tècnica mínima, executable i explicable. L'objectiu no és construir encara un producte complet, sinó entendre el model client/servidor, prendre una primera decisió tècnica guiada i deixar un repositori que arranque amb un primer punt d'entrada funcional.

El repte queda organitzat en `2` microreptes, un per sessió ordinària:

| Sessió | Microrepte | Duració | Pes | Focus |
|---|---|---:|---:|---|
| `R1S1` | `R1M1. Model client/servidor i elecció guiada de stack` | `3h` | `25%` | Comprensió del model d'execució i decisió tècnica inicial. |
| `R1S2` | `R1M2. Entorn executable, punt d'entrada i tancament de R1` | `3h` | `75%` | Entorn executable, resposta mínima del backend, documentació i checkpoint. |

## Encaix dins del repte

`R1M1` dona el criteri: què s'executa al navegador, què s'executa al servidor i quin stack inicial té sentit per al projecte. `R1M2` transforma eixa decisió en una base executable real, amb una resposta mínima servida pel backend i documentació suficient per poder continuar en `R2`.

Els antics blocs de treball d'entorn executable, primer punt d'entrada i verificació final queden unificats dins de `R1M2`. No són microreptes separats: són parts de la mateixa sessió de tancament del kickoff.

## Relació amb RA, CA i criteris de treball

| Microrepte | RA i CA treballats | Criteris de treball |
|---|---|---|
| `R1M1` | `RA1a`, `RA1b`, `RA1c`, `RA1g` | Diferenciar client i servidor, identificar el paper del backend, reconéixer el servidor d'aplicacions i justificar una tecnologia inicial. |
| `R1M2` | `RA1b`, `RA1c`, `RA1d`, `RA1e`, `RA1f`, `RA1g` | Posar en marxa l'entorn, explicar els serveis, generar una primera resposta del servidor, verificar el funcionament i documentar decisions. |

## R1S1 / R1M1. Model client/servidor i elecció guiada de stack

### Producte esperat

Una fitxa breu d'exploració tècnica inicial amb:

- esquema client/servidor aplicat al producte propi;
- exemples de què fa el client i què fa el servidor;
- comparació curta de dues o tres opcions tècniques;
- decisió inicial de stack i alternativa descartada;
- dubtes o límits que encara queden oberts.

### Preparació prèvia del professorat

- Tindre localitzats els materials d'arquitectura web, client/servidor, backend i llenguatges/frameworks.
- Preparar un exemple docent de producte senzill per modelar la fitxa.
- Preparar una pregunta oral curta per comprovar comprensió individual.

### Continguts a explicar

- Petició HTTP, resposta i paper del navegador.
- Diferència entre codi que s'executa en client i codi que s'executa en servidor.
- Paper del servidor web, runtime de servidor i backend.
- Diferència entre triar una tecnologia amb criteri i triar-la per moda.
- Ús acceptable de la IA per explorar opcions, sempre amb reformulació pròpia.

### Seqüenciació

| Temps | Activitat |
|---:|---|
| `0:00-0:15` | Presentació del repte, producte esperat i relació amb `R2`. |
| `0:15-0:35` | Explicació guiada del flux client/servidor amb un exemple concret. |
| `0:35-0:55` | Modelatge docent de la fitxa d'exploració tècnica. |
| `0:55-1:35` | Treball individual: esquema, exemples i primera comparació tècnica. |
| `1:35-2:00` | Contrast per parelles i detecció d'incoherències. |
| `2:00-2:30` | Tancament de la decisió inicial de stack. |
| `2:30-2:50` | Posada en comú curta i correcció de confusions habituals. |
| `2:50-3:00` | Checkpoint `CP-R1.1`: revisió ràpida i pregunta oral. |

### Tasques concretes de l'alumnat

- Escriure quin producte vol iniciar i quin paper tindrà el backend.
- Dibuixar o descriure el flux client/servidor.
- Escriure tres exemples del projecte: acció del client, acció del servidor i resposta.
- Comparar de manera breu dues o tres opcions tècniques del marc docent.
- Tancar una decisió inicial i una alternativa descartada.
- Registrar un dubte tècnic real.

### Evidències mínimes

- Fitxa d'exploració tècnica inicial.
- Esquema client/servidor aplicat al producte.
- Decisió tècnica inicial justificada.
- Dubte o límit tècnic registrat.

### Criteris d'èxit

- La fitxa parla del producte concret i no només de tecnologies genèriques.
- L'alumnat pot explicar què passa al navegador i què passa al servidor.
- La decisió tècnica és coherent amb el curs i amb el pas a `R1M2`.

### Què no és suficient

- Llistar frameworks sense explicar per a què servixen.
- Copiar una resposta d'IA sense entendre-la.
- Dir "usarem Laravel perquè és popular" sense relació amb el projecte.
- Confondre backend amb base de dades.

### Ús de la IA

La IA pot ajudar a comparar opcions i aclarir conceptes, però la fitxa ha d'estar escrita amb llenguatge propi. El control es farà amb una pregunta oral i amb la coherència entre fitxa, decisió i projecte.

### Suport per a alumnat amb dificultat

- Donar una plantilla de quatre caixes: navegador, servidor web, codi de servidor i dades.
- Reduir la comparació a dues opcions.
- Demanar una resposta curta de cinc línies abans de completar tota la fitxa.

### Ampliació per a alumnat avançat

- Afegir una mini ADR de decisió tècnica.
- Comparar la mateixa funcionalitat en `PHP` pla i en un framework.
- Explicar què canviaria si el client fora una app mòbil.

### Checklist de tancament

- [ ] La fitxa està completa.
- [ ] Hi ha esquema client/servidor.
- [ ] Hi ha decisió tècnica i alternativa descartada.
- [ ] Hi ha dubte tècnic registrat.
- [ ] L'alumne pot respondre una pregunta oral curta.

### Connexió amb el microrepte posterior

`R1M2` parteix de la decisió tècnica de `R1M1` i la converteix en un repositori executable. Si la decisió no està clara, l'entorn posterior quedarà com una còpia sense criteri.

## R1S2 / R1M2. Entorn executable, punt d'entrada i tancament de R1

### Producte esperat

Un repositori que permeta:

- arrancar un entorn amb `Docker` o equivalent;
- executar `PHP` darrere d'un servidor web;
- disposar de base de dades i phpMyAdmin quan corresponga al model docent;
- obrir una URL, ruta, vista, endpoint o healthcheck servit pel backend;
- seguir un `README` executable;
- localitzar la documentació i decisions del repte;
- entendre què queda preparat per a `R2`.

### Preparació prèvia del professorat

- Preparar un model mínim d'entorn executable, sense convertir-lo en solució final tancada.
- Tindre un error controlat per modelar lectura de logs.
- Preparar una checklist de revisió: arrencada, serveis, punt d'entrada, README i documentació.

### Continguts a explicar

- Estructura mínima d'un repositori backend.
- Paper de `docker-compose.yml`, servidor web, `PHP`, base de dades i phpMyAdmin.
- Diferència entre infraestructura i funcionalitat.
- Ruta o punt d'entrada mínim servit pel backend.
- README executable, documentació tècnica i evidències.
- Verificació abans de passar a `R2`.

### Seqüenciació

| Temps | Activitat |
|---:|---|
| `0:00-0:15` | Recuperació de `R1M1` i confirmació de la base tècnica triada. |
| `0:15-0:35` | Modelatge docent de l'entorn mínim i dels serveis. |
| `0:35-1:10` | Creació o adaptació del repositori, estructura i configuració d'arrencada. |
| `1:10-1:40` | Arrencada, lectura d'errors, ajustos de ports o serveis i prova del servidor web. |
| `1:40-2:05` | Creació del primer punt d'entrada funcional del backend. |
| `2:05-2:25` | README amb requisits, arrencada, parada, URL i comprovacions. |
| `2:25-2:45` | Documentació del repte: fitxa de `R1M1`, decisió tècnica, incidències i evidències. |
| `2:45-3:00` | Checkpoint `CP-R1.2`: demo curta, pregunta tècnica i pas a `R2`. |

### Tasques concretes de l'alumnat

- Crear o netejar el repositori del projecte.
- Obrir issue mare de `R1` amb tasques de `R1M2`.
- Crear o adaptar la configuració d'entorn.
- Arrancar serveis o documentar l'error amb hipòtesi i pròxima acció.
- Crear una resposta mínima del backend connectada amb el producte.
- Fer un microcanvi i comprovar que la resposta canvia.
- Escriure el `README` amb passos reals.
- Guardar fitxa, decisió, incidències i evidències dins del repositori.
- Fer commits significatius.

### Evidències mínimes

- Repositori usable.
- Configuració Docker o equivalent.
- README executable.
- Punt d'entrada funcional o error documentat amb pla de correcció.
- Evidència de prova: URL, captura, log o demo.
- Documentació localitzable dins del repositori.
- Justificació tècnica curta o ADR inicial.
- AI log quan hi haja ús rellevant d'IA.

### Criteris d'èxit

- El projecte arranca o el bloqueig està documentat amb precisió tècnica.
- El README permet repetir els passos sense informació oral oculta.
- La resposta mínima ve del backend i està connectada amb el producte.
- L'alumnat pot explicar què fa cada servei i quin fitxer respon a la petició.
- La documentació de `R1` està dins del repositori i prepara el pas a `R2`.

### Què no és suficient

- Entregar una carpeta copiada que no es pot explicar.
- Tindre Docker definit però no comprovar cap servei.
- Crear una pàgina estàtica sense execució de servidor.
- Escriure un README genèric que no arranca el projecte real.
- Deixar la fitxa de `R1M1` o les decisions fora del repositori.

### Ús de la IA

La IA pot ajudar a diagnosticar errors de configuració, explicar logs o revisar el README. Cada proposta s'ha de verificar en execució. Es penalitza incloure instruccions generades que no funcionen en el repositori real.

### Suport per a alumnat amb dificultat

- Reduir l'objectiu a serveis mínims i una ruta `/health`.
- Treballar amb una taula "servei, per a què servix, com el comprove".
- Acceptar temporalment un error documentat si inclou log, hipòtesi i pròxima acció concreta.

### Ampliació per a alumnat avançat

- Afegir una ADR inicial sobre l'estructura triada.
- Incorporar una prova manual documentada més completa.
- Preparar un endpoint d'estat que mostre versió o configuració no sensible.
- Deixar una issue preparada per al primer formulari de `R2`.

### Checklist de tancament

- [ ] El repositori té estructura clara i commits significatius.
- [ ] L'entorn arranca o l'error està ben documentat.
- [ ] Hi ha punt d'entrada funcional del backend.
- [ ] El README permet arrancar, parar i comprovar.
- [ ] La documentació de `R1` està dins del repositori.
- [ ] Hi ha decisió tècnica o ADR curta.
- [ ] L'alumnat pot fer una defensa breu.

### Connexió amb el microrepte posterior

`R2M1` partirà d'esta base per introduir entrada de dades i validació bàsica en servidor. Per això `R1M2` ha de tancar un entorn executable i un punt d'entrada comprensible, sense avançar encara formularis, sessions, login ni persistència funcional.

## Evidències globals del Repte 1

- Fitxa breu d'exploració tècnica inicial.
- Explicació del model client/servidor aplicada al producte.
- Decisió tècnica inicial.
- Repositori usable i amb commits significatius.
- Entorn executable amb `Docker`, `PHP`, servidor web, BBDD i phpMyAdmin quan corresponga.
- README executable.
- Primer punt d'entrada funcional del backend.
- Documentació localitzable dins del repositori.
- Justificació tècnica breu o ADR inicial.
- AI log quan hi haja ús rellevant d'IA.
- Defensa tècnica breu o checkpoint.

## Criteri pràctic de tancament

`R1` queda preparat quan el professorat pot veure una decisió tècnica guiada, una base executable adaptada, un primer punt d'entrada funcional del backend i una documentació suficient per continuar cap a `R2` sense tornar a començar.
