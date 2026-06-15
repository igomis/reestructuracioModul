# R1S2. Entorn executable, punt d'entrada i tancament de R1

## Finalitat de la sessió

Esta sessió tanca el `Repte 1` i treballa el microrepte `R1M2` convertint la decisió tècnica inicial en una base executable real. L'objectiu no és avançar funcionalitats de `R2`, sinó deixar un repositori que arranque, servisca una resposta mínima del backend i tinga documentació suficient perquè una altra persona puga repetir l'arrencada.

Al final de la sessió, cada alumne o parella ha de poder ensenyar un entorn executable o un bloqueig tècnic ben documentat, assenyalar quin fitxer respon a una petició i explicar què queda preparat per al primer formulari de `R2`.

## Encaix dins del Repte 1

- **Repte**: `R1. Kickoff backend`
- **Microrepte**: `R1M2`
- **Sessió**: `R1S2`
- **Duració orientativa**: `3 hores`
- **Focus**: entorn executable, serveis mínims, punt d'entrada del backend, README executable, evidències i checkpoint de pas a `R2`
- **No entra encara**: formularis, validació de dades del domini, sessions, autenticació, persistència funcional o arquitectura completa

## Relació amb RA i criteris de treball

| Element | Concreció en el microrepte |
|---|---|
| `RA1b` | comprovació de l'execució en servidor i resposta web |
| `RA1c` | identificació del servidor web, runtime i serveis de suport |
| `RA1d` | configuració mínima de l'entorn de desenvolupament |
| `RA1e` | verificació del funcionament amb URL, log, captura o demo |
| `RA1f` | documentació de passos reals d'arrencada i parada |
| `RA1g` | justificació tècnica curta o ADR inicial |
| Evidència central | repositori executable amb punt d'entrada del backend i README reproduïble |
| Verificació docent | demo curta, pregunta tècnica i revisió del README |

## Producte esperat

Un repositori que permeta:

- arrancar un entorn amb `Docker` o equivalent;
- executar `PHP` darrere d'un servidor web;
- disposar de base de dades i phpMyAdmin quan corresponga al model docent;
- obrir una URL, ruta, vista, endpoint o healthcheck servit pel backend;
- seguir un `README` executable;
- localitzar la documentació i decisions del repte;
- entendre què queda preparat per a `R2`.

## Preparació prèvia del professorat

- Preparar un model mínim d'entorn executable, sense convertir-lo en solució final tancada.
- Tindre un error controlat per modelar lectura de logs.
- Preparar una checklist de revisió: arrencada, serveis, punt d'entrada, README i documentació.
- Tindre clar que un error documentat pot ser acceptable si és precís i té pròxima acció concreta.

## Continguts a explicar

- Estructura mínima d'un repositori backend.
- Paper de `docker-compose.yml`, servidor web, `PHP`, base de dades i phpMyAdmin.
- Diferència entre infraestructura i funcionalitat.
- Ruta o punt d'entrada mínim servit pel backend.
- README executable, documentació tècnica i evidències.
- Verificació abans de passar a `R2`.

## Seqüència d'aula de 3 hores

### 0:00-0:15. Recuperació de R1M1

L'alumnat recupera la decisió tècnica de `R1M1` i confirma quina base construirà.

Resultat del tram: cada equip sap quin entorn intenta arrancar i per què.

### 0:15-0:35. Modelatge docent de l'entorn mínim

El professorat mostra els serveis mínims, com es comproven i on mirar errors.

Resultat del tram: el grup té una referència clara de què vol dir "entorn executable".

### 0:35-1:10. Creació o adaptació del repositori

Tasques:

- crear o netejar el repositori del projecte;
- obrir issue mare de `R1`;
- crear o adaptar la configuració d'entorn;
- ordenar l'estructura inicial.

Resultat del tram: hi ha repositori preparat per arrancar serveis.

### 1:10-1:40. Arrencada i lectura d'errors

L'alumnat arranca l'entorn, revisa ports, serveis i logs, i documenta qualsevol bloqueig.

Resultat del tram: l'entorn arranca o hi ha un error amb log, hipòtesi i pròxima acció.

### 1:40-2:05. Primer punt d'entrada funcional

L'alumnat crea una resposta mínima del backend connectada amb el producte.

Resultat del tram: hi ha URL, ruta, vista, endpoint o healthcheck servit pel backend.

### 2:05-2:25. README executable

Tasques:

- escriure requisits;
- indicar com arrancar i parar;
- indicar URL de comprovació;
- explicar com detectar que funciona.

Resultat del tram: una altra persona podria repetir l'arrencada sense informació oral oculta.

### 2:25-2:45. Documentació i evidències de R1

L'alumnat deixa dins del repositori la fitxa de `R1M1`, la decisió tècnica, incidències i evidències.

Resultat del tram: la documentació de `R1` és localitzable i prepara el pas a `R2`.

### 2:45-3:00. Checkpoint docent

Cada equip fa una demo curta o mostra el bloqueig documentat.

Pregunta de tancament: quin fitxer respon a la petició que estàs ensenyant i quin servei l'executa?

## Tasques concretes de l'alumnat

- Crear o netejar el repositori del projecte.
- Obrir issue mare de `R1` amb tasques de `R1M2`.
- Crear o adaptar la configuració d'entorn.
- Arrancar serveis o documentar l'error amb hipòtesi i pròxima acció.
- Crear una resposta mínima del backend connectada amb el producte.
- Fer un microcanvi i comprovar que la resposta canvia.
- Escriure el `README` amb passos reals.
- Guardar fitxa, decisió, incidències i evidències dins del repositori.
- Fer commits significatius.

## Evidències mínimes

| Evidència | Mínim acceptable |
|---|---|
| Repositori | estructura clara i commits significatius |
| Entorn | arranca o documenta un bloqueig amb log, hipòtesi i pròxima acció |
| Punt d'entrada | URL, ruta, vista, endpoint o healthcheck servit pel backend |
| README | inclou requisits, arrencada, parada, URL i comprovació |
| Evidència de prova | captura, log, URL o demo |
| Documentació | fitxa, decisió tècnica, incidències i evidències localitzables |
| Ús d'IA | AI log quan hi haja ús rellevant |

## Criteris d'èxit

El microrepte està aconseguit si:

- el projecte arranca o el bloqueig està documentat amb precisió tècnica;
- el README permet repetir els passos sense informació oral oculta;
- la resposta mínima ve del backend i està connectada amb el producte;
- l'alumnat pot explicar què fa cada servei i quin fitxer respon a la petició;
- la documentació de `R1` està dins del repositori i prepara el pas a `R2`.

## Què no és suficient

- Entregar una carpeta copiada que no es pot explicar.
- Tindre Docker definit però no comprovar cap servei.
- Crear una pàgina estàtica sense execució de servidor.
- Escriure un README genèric que no arranca el projecte real.
- Deixar la fitxa de `R1M1` o les decisions fora del repositori.
- Avançar formularis o login sense haver tancat l'entorn base.

## Ús de la IA

La IA pot ajudar a diagnosticar errors de configuració, explicar logs o revisar el README.

Control obligatori:

- cada proposta s'ha de verificar en execució;
- s'ha de registrar l'ús rellevant en l'AI log;
- es penalitza incloure instruccions generades que no funcionen en el repositori real.

## Suport per a alumnat amb dificultat

- Reduir l'objectiu a serveis mínims i una ruta `/health`.
- Treballar amb una taula "servei, per a què servix, com el comprove".
- Acceptar temporalment un error documentat si inclou log, hipòtesi i pròxima acció concreta.

Frase guia: "No afegis funcionalitat fins que pugues arrancar, comprovar i explicar una resposta mínima del backend."

## Ampliació per a alumnat avançat

- Afegir una ADR inicial sobre l'estructura triada.
- Incorporar una prova manual documentada més completa.
- Preparar un endpoint d'estat que mostre versió o configuració no sensible.
- Deixar una issue preparada per al primer formulari de `R2`.

## Checklist de tancament

- [ ] El repositori té estructura clara i commits significatius.
- [ ] L'entorn arranca o l'error està ben documentat.
- [ ] Hi ha punt d'entrada funcional del backend.
- [ ] El README permet arrancar, parar i comprovar.
- [ ] La documentació de `R1` està dins del repositori.
- [ ] Hi ha decisió tècnica o ADR curta.
- [ ] L'alumnat pot fer una defensa breu.

## Connexió amb el microrepte posterior

`R2M1` partirà d'esta base per introduir entrada de dades i validació bàsica en servidor. Per això `R1M2` ha de tancar un entorn executable i un punt d'entrada comprensible, sense avançar encara formularis, sessions, login ni persistència funcional.
## Microtaller associat

- **Microtaller**: `MT02. README executable i commit defensable`
- **Presentació**: [MT02. README executable i commit defensable](../07_presentacions/microtallers/mt02_readme_commit_defensable.md)
- **Moment recomanat**: després de comprovar que l'entorn arranca i abans del commit de tancament de `R1`.
- **Evidència mínima**: README amb arrencada real, primer punt funcional verificat i commit explicable.
