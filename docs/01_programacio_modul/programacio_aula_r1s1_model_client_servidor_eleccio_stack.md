# R1S1. Model client/servidor i elecció guiada de stack

## Finalitat de la sessió

Esta sessió obri el `Repte 1` i treballa el microrepte `R1M1` amb una primera comprensió operativa del model client/servidor. L'objectiu no és triar una tecnologia per intuïció o per moda, sinó entendre què s'executa al navegador, què s'executa al servidor i quin stack inicial té sentit per al producte que l'alumnat vol construir.

Al final de la sessió, cada alumne o parella ha de poder explicar el paper del backend en el seu producte, representar un flux mínim client/servidor i justificar una primera decisió tècnica amb una alternativa descartada.

També ha de quedar resolt el punt operatiu inicial: cada alumne ha d'haver acceptat l'enllaç de GitHub Classroom, clonat el seu repositori individual i fet un primer `push`. Eixe repositori serà el repositori de treball de tot el curs.

## Encaix dins del Repte 1

- **Repte**: `R1. Kickoff backend`
- **Microrepte**: `R1M1`
- **Sessió**: `R1S1`
- **Duració orientativa**: `3 hores`
- **Focus**: model client/servidor, paper del backend, comparació guiada de stacks i decisió tècnica inicial
- **No entra encara**: entorn complet, formularis, sessions, login, persistència funcional o arquitectura definitiva del producte

## Relació amb RA i criteris de treball

| Element | Concreció en el microrepte |
|---|---|
| `RA1a` | identificació dels elements bàsics d'una aplicació web i del paper del servidor |
| `RA1b` | diferenciació entre execució en client i execució en servidor |
| `RA1c` | reconeixement del servidor d'aplicacions, runtime i tecnologia backend |
| `RA1g` | justificació inicial de la tecnologia triada i dels seus límits |
| Evidència central | repositori Classroom clonat, primer `push` i fitxa d'exploració tècnica inicial aplicada al producte |
| Verificació docent | pregunta oral curta sobre què passa al client, què passa al servidor i per què s'ha triat el stack |

## Producte esperat

Un repositori individual de GitHub Classroom ja creat, clonat i pujat amb un primer canvi en `README.md`, més una fitxa breu d'exploració tècnica inicial amb:

- esquema client/servidor aplicat al producte propi;
- exemples de què fa el client i què fa el servidor;
- comparació curta de dues o tres opcions tècniques;
- decisió inicial de stack i alternativa descartada;
- dubtes o límits que encara queden oberts.

## Preparació prèvia del professorat

- Tindre localitzats els materials d'arquitectura web, client/servidor, backend i llenguatges/frameworks.
- Tindre preparada la presentació inicial del curs per explicar repositori, evidències, avaluació i forma de treball.
- Tindre preparat l'enllaç de GitHub Classroom i comprovar que el repositori base de l'alumnat és el correcte.
- Preparar un exemple docent de producte senzill per modelar la fitxa.
- Preparar una pregunta oral curta per comprovar comprensió individual.
- Tindre clara la frontera de la sessió: encara no es construeix l'entorn executable.

## Continguts a explicar

- Petició HTTP, resposta i paper del navegador.
- Diferència entre codi que s'executa en client i codi que s'executa en servidor.
- Paper del servidor web, runtime de servidor i backend.
- Diferència entre triar una tecnologia amb criteri i triar-la per moda.
- Flux bàsic de treball: acceptar Classroom, clonar repositori, modificar `README.md`, commit i `push`.
- Ús acceptable de la IA per explorar opcions, sempre amb reformulació pròpia.

## Seqüència d'aula de 3 hores

### 0:00-0:15. Presentació del curs, repositori i producte esperat

El professorat presenta el funcionament del curs, el `Repte 1`, el sentit del kickoff backend i la relació amb els reptes posteriors.

També explica que el repositori de GitHub Classroom serà el repositori individual de treball durant tot el curs.

Resultat del tram: l'alumnat sap que la sessió acaba amb repositori creat, clonat i pujat, més una fitxa tècnica breu; no amb un projecte ja implementat.

### 0:15-0:35. Acceptació i clonatge del repositori Classroom

Tasques:

- acceptar l'enllaç de GitHub Classroom;
- obrir el repositori individual creat per Classroom;
- copiar la URL de clonatge;
- clonar el repositori localment;
- executar `git status`.

Resultat del tram: cada alumne té el seu repositori individual en local i sap que no ha de clonar el repositori base directament.

### 0:35-0:55. Model client/servidor amb un exemple concret

El professorat explica el flux bàsic d'una petició web: navegador, servidor, codi de servidor i resposta.

Resultat del tram: l'alumnat pot separar, en un cas senzill, què fa el client i què fa el servidor.

### 0:55-1:15. Modelatge docent de la fitxa i del `README.md` inicial

El professorat mostra una fitxa d'exploració tècnica mínima amb un producte exemple i com deixar en `README.md` el microrepte actual, el producte triat i la primera decisió de treball.

Resultat del tram: l'alumnat veu el nivell de concreció esperat i evita llistes genèriques de frameworks.

### 1:15-1:55. Treball individual o per parelles

Tasques:

- escriure quin producte vol iniciar;
- dibuixar o descriure el flux client/servidor;
- escriure tres exemples del projecte: acció del client, acció del servidor i resposta;
- iniciar una comparació breu de dues o tres opcions tècniques.

Resultat del tram: cada equip té una primera fitxa amb producte, flux i opcions tècniques.

### 1:55-2:20. Contrast per parelles

Una altra persona revisa si la fitxa diferencia realment client, servidor i dades.

Resultat del tram: cada equip detecta una confusió, omissió o decisió massa genèrica.

### 2:20-2:40. Decisió inicial de stack

L'alumnat tanca una decisió tècnica inicial i una alternativa descartada.

Resultat del tram: la decisió queda escrita amb un motiu relacionat amb el producte i amb el marc del curs.

### 2:40-2:55. Commit i `push` inicial

Tasques:

- actualitzar `README.md` amb `R1M1`, projecte base, flux client/servidor i decisió inicial;
- guardar la fitxa o evidència equivalent en `docs/`;
- fer commit amb un missatge comprensible;
- fer `push` a `main`.

Resultat del tram: GitHub mostra el primer canvi i el professorat pot comprovar que el repositori queda operatiu.

### 2:55-3:00. Checkpoint docent

Cada equip mostra el repositori en GitHub, la fitxa i respon una pregunta breu.

Pregunta de tancament: què passa exactament al navegador i què passa al servidor en una acció bàsica del teu producte?

## Tasques concretes de l'alumnat

- Escriure quin producte vol iniciar i quin paper tindrà el backend.
- Acceptar l'enllaç de GitHub Classroom i clonar el repositori individual.
- Identificar `README.md`, `ENTREGA.md`, `docs/` i `evidence/`.
- Dibuixar o descriure el flux client/servidor.
- Escriure tres exemples del projecte: acció del client, acció del servidor i resposta.
- Comparar de manera breu dues o tres opcions tècniques del marc docent.
- Tancar una decisió inicial i una alternativa descartada.
- Registrar un dubte tècnic real.
- Fer un primer commit i `push` a `main`.

## Evidències mínimes

| Evidència | Mínim acceptable |
|---|---|
| Repositori Classroom | acceptat, clonat i amb primer `push` visible |
| `README.md` inicial | indica `R1M1`, projecte base, flux client/servidor i decisió inicial |
| Fitxa d'exploració | parla del producte concret i no només de tecnologies genèriques |
| Esquema client/servidor | diferencia navegador, servidor i resposta |
| Exemples del producte | inclou acció de client, acció de servidor i resposta |
| Decisió tècnica | indica stack inicial i alternativa descartada |
| Dubte o límit | deixa registrat què encara no està clar |

## Criteris d'èxit

El microrepte està aconseguit si:

- el repositori individual està creat, clonat i pujat a GitHub;
- la fitxa parla del producte concret;
- l'alumnat pot explicar què passa al navegador i què passa al servidor;
- la decisió tècnica és coherent amb el curs i amb el pas a `R1M2`;
- hi ha una alternativa descartada amb motiu;
- hi ha un dubte tècnic real registrat.

## Què no és suficient

- Llistar frameworks sense explicar per a què servixen.
- Copiar una resposta d'IA sense entendre-la.
- Dir "usarem Laravel perquè és popular" sense relació amb el projecte.
- Confondre backend amb base de dades.
- Fer una decisió tècnica que no puga orientar la sessió següent.

## Ús de la IA

La IA pot ajudar a comparar opcions i aclarir conceptes, però la fitxa ha d'estar escrita amb llenguatge propi.

Control obligatori:

- l'alumnat ha de poder reformular la comparació sense llegir la resposta de la IA;
- ha d'explicar què ha acceptat, descartat o modificat;
- la coherència es comprova amb una pregunta oral curta.

## Suport per a alumnat amb dificultat

- Donar una plantilla de quatre caixes: navegador, servidor web, codi de servidor i dades.
- Reduir la comparació a dues opcions.
- Demanar una resposta curta de cinc línies abans de completar tota la fitxa.

Frase guia: "Primer explica el viatge d'una petició; després ja decidirem amb quina tecnologia la servirem."

## Ampliació per a alumnat avançat

- Afegir una mini ADR de decisió tècnica.
- Comparar la mateixa funcionalitat en `PHP` pla i en un framework.
- Explicar què canviaria si el client fora una app mòbil.

## Checklist de tancament

- [ ] La fitxa està completa.
- [ ] El repositori Classroom està acceptat i clonat.
- [ ] Hi ha un primer `push` visible en GitHub.
- [ ] El `README.md` identifica `R1M1` i el projecte base.
- [ ] Hi ha esquema client/servidor.
- [ ] Hi ha decisió tècnica i alternativa descartada.
- [ ] Hi ha dubte tècnic registrat.
- [ ] L'alumne pot respondre una pregunta oral curta.

## Connexió amb el microrepte posterior

`R1M2` parteix de la decisió tècnica de `R1M1` i la converteix en un repositori executable. Si la decisió no està clara, l'entorn posterior quedarà com una còpia sense criteri.

## Materials associats per a portar a l'aula

- **Presentació associada**: [MT01. Projecte no CRUD](https://cipfpbatoi.github.io/dwes2627/recursos/Tallers/MT01-Projecte-no-CRUD.pdf)
- **Presentació inicial del curs**: [Benvinguda al curs](https://cipfpbatoi.github.io/dwes2627/recursos/Presentacions/Benvinguda-al-curs.pdf)
- **Teoria o material associat**: [Backend, client-servidor i arquitectura web](https://cipfpbatoi.github.io/dwes2627/recursos/Teoria/Teoria-R1-Backend-client-servidor-i-arquitectura-web.pdf)
- **Guia operativa**: [Com pujar el treball per a l'autocorrecció](https://cipfpbatoi.github.io/dwes2627/04_materials/guia_pujar_treball_autocorreccio/)

## Microtaller associat

- **Microtaller**: `MT01. Projecte no CRUD`
- **Moment recomanat**: abans de tancar la tria de domini i primera orientació del producte.
- **Evidència mínima**: domini amb actors, regles i primer flux que no siga només CRUD.
