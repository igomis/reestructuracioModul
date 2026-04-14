# Matriu de coherència vertical dels reptes 1-3

## Finalitat del document

Esta matriu servix per comprovar la coherència vertical entre els tres primers reptes del mòdul.

No substituïx la planificació detallada de cada repte. La seua funció és ajudar a revisar:

- la progressió real de dificultat
- la distribució dels resultats d’aprenentatge
- la visibilitat dels criteris d’avaluació
- els possibles solapaments útils
- els possibles solapaments problemàtics
- les evidències dominants de cada fase
- la frontera entre allò que s’introduïx, allò que es consolida i allò que es reutilitza

---

## Criteri de lectura

Esta matriu s’ha de llegir amb estes claus:

- un mateix element pot reaparéixer en més d’un repte, però no necessàriament amb el mateix valor curricular
- hi ha solapaments desitjables quan un repte reutilitza una funcionalitat anterior per a avaluar una competència nova
- hi ha solapaments problemàtics quan un repte torna a avaluar el mateix sense augment real de complexitat
- la coherència no depén només del producte final, sinó del tipus d’evidència, del tipus d’instrument i del focus dels criteris d’avaluació

---

## Lectura sintètica de la seqüència

### Repte 1

Obri el projecte, fixa base tècnica, documentació mínima, decisió d’arquitectura i primera funcionalitat de servidor.

### Repte 2

Amplia la base tècnica amb processament bàsic, formularis, lògica, estat, autenticació i una primera operació protegida del domini.

### Repte 3

Transforma una funcionalitat ja existent en una peça més mantenible i més professional, amb separació de responsabilitats i persistència suficient aplicada a un cas d’ús real.

---

## Matriu de coherència vertical

| Repte | Microprojecte o focus | RA principal | CA o bloc de CA | Evidència dominant | Instrument dominant | Risc de solapament | Judici de coherència | Observació docent |
|---|---|---|---|---|---|---|---|---|
| Repte 1 | Decisió tècnica inicial i ADR | RA1 | RA1b, RA1c, RA1g | comparativa, ADR, defensa | rúbrica breu | Baix | Coherent com a obertura del projecte | No convertir-ho en debat teòric desconnectat del producte |
| Repte 1 | Entorn executable i estructura base | RA1 | RA1c, RA1d, RA1e, RA1f | repositori, README, arrencada | checklist + revisió | Mitjà | Coherent si després no es torna a avaluar només l’arrencada | Açò prepara el treball posterior, però no substituïx RA5 |
| Repte 1 | Primera funcionalitat mínima | RA1 | RA1b, RA1e, RA1f | landing o equivalent, formulari, validació, registre mínim | rúbrica funcional | Mitjà | Coherent perquè en Repte 2 escala a flux complet | És un primer flux, no encara el nucli funcional complet del domini |
| Repte 2 | Formulari base i recuperació de dades | RA3 | RA3.e, RA3.f, RA3.g | formulari, recuperació, comentaris | checklist | Mitjà | Solapament bo amb Repte 1 | En Repte 1 és evidència mínima; ací és objecte d’avaluació explícit |
| Repte 2 | Processament bàsic en servidor | RA2 | RA2.a, RA2.b, RA2.c, RA2.d, RA2.e, RA2.f, RA2.g, RA2.h | codi executable, codi embegut, variables, directives | rúbrica breu | Baix | Molt coherent | Fa visible el bloc bàsic de SA2 i evita saltar massa ràpid a autenticació |
| Repte 2 | Decisions, arrays i funcions | RA3 | RA3.a, RA3.b, RA3.c, RA3.d | lògica observable | rúbrica | Baix | Coherent i necessari | És la baula entre formulari i comportament de domini |
| Repte 2 | Estat, sessió i/o cookies | RA4 | RA4.a, RA4.b, RA4.c | demo d’estat | checklist | Baix | Molt coherent | Convindria no deixar-ho diluït dins del login |
| Repte 2 | Autenticació i operació protegida | RA4 | RA4.d, RA4.e | login, cas autoritzat, cas denegat | rúbrica | Mitjà | Coherent si en Repte 3 es reutilitza com a cas d’ús, no com a novetat | El valor està en protegir una operació real, no en login/logout a soles |
| Repte 2 | Prova, depuració i documentació | RA4 | RA4.f | proves, incidències, documentació | checklist + defensa | Mitjà | Coherent | En Repte 3 la prova ha de passar a ser de regressió i manteniment |
| Repte 3 | Diagnosi del codi actual i pla de migració | RA5 | RA5.c, RA5.d | diagnosi, pla, issues | rúbrica | Baix | Molt coherent | Marca clarament el canvi de focus cap a mantenibilitat |
| Repte 3 | Migració del primer cas d’ús | RA5 | RA5.e, RA5.f | abans/després, commits | rúbrica | Mitjà | Coherent | Reutilitza el cas d’ús del Repte 2 però canvia l’objecte d’avaluació |
| Repte 3 | Consolidació de capes i rols tècnics | RA5 | RA5.g, RA5.h | estructura final, justificació | checklist | Baix | Molt coherent | Prepara bé el pas a serveis o API |
| Repte 3 | Persistència segura aplicada | RA6 | RA6.a, RA6.b, RA6.c, RA6.d | lectura, escriptura, demo | rúbrica | Mitjà-alt | Coherent si es manté acotada al cas d’ús prioritari | No hauria d’esgotar tot el bloc d’accés a dades del mòdul |
| Repte 3 | Validacions, errors i regressió mínima | RA6 | RA6.f, RA6.g | proves, incidències, demo | checklist | Mitjà | Coherent | El focus ací és regressió després de refactorització, no prova funcional bàsica |
| Repte 3 | Documentació i preparació del Repte 4 | RA5 / RA6 | RA5.f, RA5.g, RA6.g | README, decisions, defensa | rúbrica + checklist | Baix | Coherent | Fa de pont amb el repte següent |

---

## Solapaments desitjables

### 1. Formulari i entrada de dades entre Repte 1 i Repte 2

És un solapament acceptable perquè el valor curricular no és el mateix.

En el Repte 1 apareix com a primera evidència funcional mínima. En el Repte 2 passa a ser una peça explícita de treball sobre formulari, recuperació de dades i processament.

### 2. El mateix cas d’ús entre Repte 2 i Repte 3

És un solapament desitjable perquè no es reavalua exactament el mateix.

En el Repte 2 la pregunta és: “funciona i està protegit?”.

En el Repte 3 la pregunta és: “està millor estructurat, és més mantenible i persistix de manera més fiable?”.

### 3. Proves i verificació entre Repte 2 i Repte 3

També és un bon solapament si es diferencia bé l’objecte de prova:

- en Repte 2: prova funcional bàsica
- en Repte 3: prova de regressió, persistència i qualitat del refactor

---

## Solapaments a vigilar

### 1. Persistència massa forta en Repte 3

Si el Repte 3 desplega massa profundament RA6, es pot debilitar la progressió del repte o situació posterior centrada més específicament en accés a dades, seguretat o exposició de serveis.

**Decisió recomanada**

Acotar la persistència del Repte 3 al cas d’ús prioritari i evitar que es convertisca en una explotació exhaustiva de tota la capa de dades.

### 2. Lectura massa forta de mantenibilitat en Repte 1

El Repte 1 pot preparar hàbits de treball ordenat, però no hauria d’interpretar-se com el lloc on ja s’avalua de manera plena la separació de responsabilitats pròpia de RA5.

**Decisió recomanada**

Mantindre en Repte 1 una formulació de “base tècnica ben organitzada” o “preparació del terreny”, però reservar la lectura forta de RA5 per al Repte 3.

### 3. Estat i sessió diluïts dins de l’autenticació en Repte 2

És fàcil que el professorat o l’alumnat identifiquen massa ràpidament “estat = login”, i així es perda una comprensió més fina del bloc.

**Decisió recomanada**

Mantindre un microprojecte propi de “estat, sessió i/o cookies” i verificar-lo com a capa específica abans del bloc d’autenticació.

---

## Buits o ajustos recomanats

### Ajust 1. Fer explícita la frontera Repte 1 → Repte 3

Convé afegir al Repte 1 una frase de límit com esta:

> La primera organització del projecte prepara el treball posterior de mantenibilitat, però no substituïx el treball específic de separació de responsabilitats i arquitectura del Repte 3.

### Ajust 2. Reforçar la lectura pròpia de l’estat en Repte 2

Convé recordar dins del Repte 2 que estat, sessió i cookies no apareixen només com a abansala del login, sinó com a contingut amb valor formatiu propi.

### Ajust 3. Fer explícit el límit de la persistència en Repte 3

Convé afegir al Repte 3 una frase de límit com esta:

> La persistència d’este repte es desplega sobre el cas d’ús prioritari i no pretén esgotar tot el bloc d’accés a dades del mòdul.

---

## Judici global sobre la seqüència 1-3

La seqüència actual es pot llegir així:

- **Repte 1**: arrencada professional i primer flux mínim
- **Repte 2**: flux complet de servidor fins a operació protegida
- **Repte 3**: professionalització arquitectònica i persistència suficient sobre un cas d’ús real

Esta progressió és coherent i curricularment defensable si es mantenen clares les fronteres entre:

- allò que s’introduïx
- allò que es consolida
- allò que es reutilitza per a ser avaluat amb un altre focus

---

## Decisions de control abans de redactar el Repte 4

Abans de continuar amb el Repte 4, convé revisar:

- si algun CA de RA4 està reapareixent en Repte 3 sense necessitat
- si RA6 en Repte 3 està quedant massa ampli
- si la funcionalitat protegida del Repte 2 és prou bona com per servir de cas d’ús prioritari del Repte 3
- si els instruments de verificació estan realment canviant d’un repte a l’altre
- si la defensa oral o tècnica té preguntes específiques per a cada focus i no repetides

---

## Ús recomanat del document

Este document es pot usar per a:

- revisió interna del disseny dels reptes
- coordinació de departament
- comprovació de solapaments
- justificació metodològica davant inspecció o revisió
- revisió de la matriu d’avaluació
- preparació de futurs reptes o ajustos de seqüència

---
