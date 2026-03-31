# Matriu de coherència vertical dels reptes 1-4

## Finalitat del document

Esta matriu servix per revisar la coherència vertical dels quatre primers reptes del mòdul.

No substituïx la planificació detallada de cada repte. La seua funció és ajudar a comprovar:

- la progressió real de dificultat
- la distribució dels resultats d’aprenentatge
- la visibilitat dels criteris d’avaluació
- la relació entre producte evolutiu i focus d’avaluació
- els solapaments útils
- els solapaments problemàtics
- les fronteres entre reptes
- els punts de control abans de continuar amb el Repte 5

---

## Criteri de lectura

Esta matriu s’ha de llegir amb estes claus:

- el producte del curs pot continuar sent el mateix, però l’objecte principal d’avaluació ha de canviar d’un repte a l’altre
- un mateix cas d’ús pot reaparéixer en més d’un repte si el focus curricular també canvia
- hi ha solapaments bons quan un repte reutilitza un producte anterior per a avaluar una competència nova
- hi ha solapaments problemàtics quan un repte torna a fer pràcticament el mateix sense augment clar de complexitat o canvi real de focus
- la coherència es juga tant en els criteris d’avaluació com en el tipus d’evidència i en els instruments de verificació

---

## Lectura sintètica de la seqüència 1-4

### Repte 1

Obri el projecte, fixa base tècnica, criteri inicial d’arquitectura, traçabilitat i primera funcionalitat mínima en servidor.

### Repte 2

Amplia eixa base amb processament de dades, lògica bàsica, estat, autenticació i una primera operació protegida del domini.

### Repte 3

Reutilitza una funcionalitat ja existent per professionalitzar-la: separació de responsabilitats, arquitectura més mantenible i persistència suficient sobre un cas d’ús real.

### Repte 4

Exposa una funcionalitat ja estructurada com a servei reusable, consumible i documentat, amb contracte clar, autenticació en context d’API i verificació real del consum.

---

## Matriu de coherència vertical

| Repte | Microprojecte o focus | RA principal | CA o bloc de CA | Evidència dominant | Instrument dominant | Risc de solapament | Judici de coherència | Observació docent |
|---|---|---|---|---|---|---|---|---|
| Repte 1 | Decisió tècnica inicial i ADR | RA1 | RA1b, RA1c, RA1g | comparativa, ADR, defensa | rúbrica breu | Baix | Coherent com a obertura del projecte | No convertir-ho en debat teòric desconnectat del producte |
| Repte 1 | Entorn executable i estructura base | RA1 | RA1c, RA1d, RA1e, RA1f | repositori, README, arrencada | checklist + revisió | Mitjà | Coherent si després no es torna a avaluar només l’arrencada | Açò prepara el treball posterior, però no substituïx RA5 |
| Repte 1 | Primera funcionalitat mínima | RA1 | RA1b, RA1e, RA1f | landing o equivalent, formulari, validació, registre mínim | rúbrica funcional | Mitjà | Coherent perquè en Repte 2 escala a flux complet | És un primer flux, no encara el nucli funcional complet del domini |
| Repte 2 | Formulari base i recuperació de dades | RA3 | RA3.e, RA3.f, RA3.g | formulari, recuperació, comentaris | checklist | Mitjà | Solapament bo amb Repte 1 | En Repte 1 és evidència mínima; ací és objecte d’avaluació explícit |
| Repte 2 | Processament bàsic en servidor | RA2 | RA2.c, RA2.d, RA2.e, RA2.f, RA2.g, RA2.h | codi executable, variables, directives | rúbrica breu | Baix | Molt coherent | Fa visible el bloc bàsic de SA2 i evita saltar massa ràpid a autenticació |
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
| Repte 4 | Disseny del contracte del servei | RA7 | RA7.a, RA7.b, RA7.c, RA7.d | mapa d’endpoints, taula request/response, defensa | rúbrica | Baix | Molt coherent | Canvia el focus des d’arquitectura interna a interoperabilitat |
| Repte 4 | Implementació del primer endpoint funcional | RA7 | RA7.d, RA7.e + suport RA6.c, RA6.d | endpoint, resposta, dades reals, demo | rúbrica | Mitjà | Coherent | Correcte si no reobre un nou bloc general de persistència |
| Repte 4 | Autenticació i control d’accés de l’API | RA7 | RA7.e, RA7.f | peticions autoritzades i denegades | rúbrica | Mitjà | Coherent | No ha de repetir la lògica del Repte 2, sinó adaptar-la a context de servei |
| Repte 4 | Consum del servei | RA7 | RA7.f, RA7.g | consumidor mínim, demo, error controlat | checklist | Baix | Molt coherent | És la prova real que el servei és reusable |
| Repte 4 | Documentació i prova del servei | RA7 / RA6 | RA7.f, RA7.h, RA6.g | documentació, proves, incidències, defensa | rúbrica + checklist | Baix | Molt coherent | Fa visible que una API usable no és només codi d’endpoints |

---

## Solapaments desitjables

### 1. Reaparició del mateix cas d’ús entre Repte 2, Repte 3 i Repte 4

És un solapament bo perquè la pregunta curricular canvia en cada fase:

- en **Repte 2**: el cas d’ús funciona i està protegit
- en **Repte 3**: el cas d’ús està millor estructurat i és més mantenible
- en **Repte 4**: el cas d’ús es pot exposar i consumir com a servei reusable

Este tipus de reaparició reforça la idea de projecte evolutiu.

### 2. Proves i verificació al llarg de la seqüència

També és un solapament bo si el focus no és el mateix:

- en **Repte 2**: prova funcional bàsica
- en **Repte 3**: prova de regressió i estabilitat després de la refactorització
- en **Repte 4**: prova i consum del servei des de fora

### 3. Documentació al llarg dels reptes

És un solapament desitjable perquè la documentació va canviant de naturalesa:

- en **Repte 1**: README i arrencada
- en **Repte 2**: documentació de comportament funcional i errors
- en **Repte 3**: decisions arquitectòniques i deute tècnic
- en **Repte 4**: contracte i ús del servei per tercers

---

## Solapaments a vigilar

### 1. Persistència massa forta entre Repte 3 i Repte 4

És el risc principal de la seqüència 1-4.

Si el Repte 4 torna a entrar massa en connexió, model de dades, operacions de persistència o tractament intern, el focus d’API es pot desdibuixar.

**Decisió recomanada**

En el Repte 4, RA6 ha d’aparéixer només com a suport per servir dades reals i coherents des de l’API.

No ha de convertir-se en un nou repte de capa de dades.

### 2. Repetició de l’autenticació del Repte 2 dins del Repte 4

També és un risc clar.

En el Repte 2 l’autenticació està al servei d’una operació del domini dins del backend.

En el Repte 4 l’autenticació ha de reaparéixer només en la mesura necessària per protegir un servei web.

**Decisió recomanada**

En el Repte 4 no s’ha de tornar a avaluar “fer login” com a novetat, sinó adaptar el control d’accés al context d’API.

### 3. API ornamental sense consum real

És un risc específic del Repte 4.

Una seqüència de endpoints pot semblar moderna o professional, però si ningú la consumix realment, el repte queda incomplet.

**Decisió recomanada**

Mantindre el microprojecte de consum del servei com a part obligatòria i no com a ampliació opcional.

---

## Buits o ajustos recomanats

### Ajust 1. Fer explícita la frontera Repte 3 → Repte 4

Convé incloure al Repte 4 una frase de límit com esta:

> El Repte 4 reutilitza una funcionalitat ja estructurada i persistent del projecte, però canvia l’objecte principal d’avaluació: ara es valora sobretot la capacitat d’exposar-la com a servei reusable, consumible i documentat.

### Ajust 2. Acotar el paper de RA6 en Repte 4

Convé incloure també una frase de límit com esta:

> La persistència en este repte només es treballa en la mesura necessària per alimentar el servei amb dades reals i coherents.

### Ajust 3. Fer visible que el consum és part del repte

Convé reforçar al Repte 4 que una API sense consumidor verificat no es considera evidència suficient.

---

## Judici global sobre la seqüència 1-4

La seqüència actual es pot llegir així:

- **Repte 1**: arrencada professional i primer flux mínim
- **Repte 2**: processament complet fins a acció protegida
- **Repte 3**: professionalització arquitectònica i persistència suficient
- **Repte 4**: exposició del cas d’ús com a servei reusable i consumible

És una seqüència coherent, curricularment defensable i metodològicament forta si es mantenen clares les fronteres entre:

- construcció inicial
- funcionalitat completa
- mantenibilitat interna
- interoperabilitat externa

---

## Decisions de control abans de redactar el Repte 5

Abans de continuar amb el Repte 5, convé revisar:

- si **RA7** ha quedat realment al centre del Repte 4
- si **RA6** no s’ha desbordat massa entre Repte 3 i Repte 4
- si el consum del servei és realment obligatori i verificable
- si la documentació del servei és usable per tercers
- si el Repte 5 ha d’anar cap a integració externa, desplegament, automatització, manteniment avançat o traçabilitat ampliada sense trencar la progressió construïda

---

## Ús recomanat del document

Este document es pot usar per a:

- revisió interna de la seqüència de reptes
- coordinació docent
- comprovació de solapaments
- justificació curricular i metodològica
- preparació del Repte 5
- revisió de la matriu d’avaluació del mòdul

---
