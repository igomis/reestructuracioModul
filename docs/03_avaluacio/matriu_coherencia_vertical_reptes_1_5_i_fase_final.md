# Matriu de coherència vertical dels reptes 1-5 i de la fase final integradora

## Finalitat del document

Esta matriu servix per revisar la coherència vertical de tota la seqüència principal del mòdul:

- Reptes 1-5
- fase final integradora de tancament, verificació i defensa

No substituïx la planificació detallada de cada repte o fase. La seua funció és ajudar a comprovar:

- la progressió real de dificultat
- la distribució dels resultats d’aprenentatge
- la relació entre producte evolutiu i focus d’avaluació
- la visibilitat dels criteris d’avaluació
- els solapaments útils
- els solapaments problemàtics
- les fronteres entre reptes i fase final
- la coherència del tancament global del mòdul

---

## Criteri de lectura

Esta matriu s’ha de llegir amb estes claus:

- el producte del curs pot continuar sent el mateix, però l’objecte principal d’avaluació ha de canviar d’un repte a l’altre
- un mateix cas d’ús pot reaparéixer en més d’una fase si el focus curricular canvia
- hi ha solapaments desitjables quan una funcionalitat ja construïda es reutilitza per a avaluar una competència nova
- hi ha solapaments problemàtics quan un repte torna a fer pràcticament el mateix sense augment clar de complexitat ni canvi real de focus
- la fase final integradora no introduïx un bloc temàtic nou central, sinó que reactiva, consolida i verifica el producte i l’aprenentatge real acumulat

---

## Lectura sintètica de la seqüència completa

### Repte 1

Obri el projecte, fixa base tècnica, criteri inicial d’arquitectura, traçabilitat i primera funcionalitat mínima en servidor.

### Repte 2

Amplia eixa base amb processament de dades, lògica bàsica, estat, autenticació i una primera operació protegida del domini.

### Repte 3

Reutilitza una funcionalitat ja existent per professionalitzar-la: separació de responsabilitats, arquitectura més mantenible i persistència suficient sobre un cas d’ús real.

### Repte 4

Exposa una funcionalitat ja estructurada com a servei reusable, consumible i documentat, amb contracte clar, autenticació en context d’API i verificació real del consum.

### Repte 5

Integra una o més fonts externes dins del projecte per crear una funcionalitat híbrida amb valor real, transformació de dades i verificació del flux complet.

### Fase final integradora

Tanca el producte amb una mirada professional de manteniment, estabilització, prova, documentació, automatització mínima i defensa tècnica amb evidències d’autoria.

---

## Matriu de coherència vertical

| Fase | Microprojecte o focus | RA principal | CA o bloc de CA | Evidència dominant | Instrument dominant | Risc de solapament | Judici de coherència | Observació docent |
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
| Repte 5 | Selecció de fonts externes i disseny de la integració | RA9 | RA9.a, RA9.b | comparativa de fonts, esquema del flux, defensa | rúbrica | Baix | Molt coherent | Canvia el focus de “exposar” a “reutilitzar i integrar” |
| Repte 5 | Connexió amb la font externa i recuperació real | RA9 | RA9.c, RA9.f | connector, dades reals, demo, error | rúbrica | Mitjà | Coherent | Correcte si no es queda en consum superficial sense valor afegit |
| Repte 5 | Transformació, mapping i valor afegit | RA9 | RA9.d, RA9.e | transformació observable, mapping, demo | rúbrica | Baix | Molt coherent | Ací està el cor del repte: crear valor nou a partir d’allò extern |
| Repte 5 | Integració de la funcionalitat híbrida | RA9 | RA9.e, RA9.f | demo completa, integració, commits | rúbrica | Mitjà | Coherent | No ha de quedar com una demo externa aïllada del producte |
| Repte 5 | Prova, depuració i documentació del flux híbrid | RA9 | RA9.g, RA9.h | proves, errors, documentació, defensa | rúbrica | Baix | Molt coherent | Tanca el repte amb lectura professional i mantingable |
| Fase final integradora | Auditoria final del producte | Reactiva RA5, RA6, RA7, RA9 | síntesi de problemes, riscos i prioritats | informe d’auditoria, taula d’incidències | rúbrica | Baix | Molt coherent | No és un nou bloc tècnic, sinó una lectura global del producte |
| Fase final integradora | Pla de millora i tancament | Reactiva RA5, RA6, RA7, RA9 | priorització, justificació i acotació | pla de tancament, mapa de decisions | checklist | Baix | Molt coherent | Fa visible criteri tècnic i no només execució |
| Fase final integradora | Estabilització i correccions prioritàries | Reactiva RA5, RA6, RA7, RA9 | correcció, coherència i manteniment | commits, issues tancades, demo abans/després | rúbrica | Mitjà | Coherent | Correcte si no es convertix en refactorització oberta sense límit |
| Fase final integradora | Prova final i verificació del sistema | Reactiva RA6, RA7, RA9 | prova funcional, regressió i estabilitat | registre de proves, casos positius i negatius | checklist | Mitjà | Molt coherent | És la capa final de verificació global, no una repetició del Repte 2 |
| Fase final integradora | Documentació final i operació mínima | Reactiva RA5, RA7, RA9 | documentació real d’ús i manteniment | README final, documentació, checklist d’operació | rúbrica | Baix | Molt coherent | Tanca el producte amb mirada professional |
| Fase final integradora | Automatització o procediment útil | Reactiva RA5, RA7, RA9 | operació, manteniment i utilitat real | script, automatització, demo | checklist | Mitjà | Coherent | És bona capa final si no es torna bloc nou independent |
| Fase final integradora | Defensa tècnica final i autoria | Reactiva RA5, RA6, RA7, RA9 | síntesi, autoria, justificació i transferència | presentació, demo, AI log, traçabilitat | rúbrica | Baix | Molt coherent | Clau per verificar aprenentatge real en context d’IA |

---

## Solapaments desitjables

### 1. Reaparició del mateix producte al llarg de tota la seqüència

És un solapament bo perquè l’objecte material continua sent el mateix producte, però la pregunta curricular canvia:

- en **Repte 1**: pot arrancar i mostrar un primer flux mínim
- en **Repte 2**: pot processar i protegir una operació real
- en **Repte 3**: pot mantindre’s millor i persistir de manera suficient
- en **Repte 4**: pot exposar-se com a servei reusable
- en **Repte 5**: pot integrar informació o serveis externs
- en **fase final**: pot tancar-se, verificar-se, documentar-se i defensar-se professionalment

### 2. Proves i verificació en totes les fases

És un solapament desitjable si el focus canvia:

- **Repte 2**: prova funcional bàsica
- **Repte 3**: regressió i persistència després de refactorització
- **Repte 4**: prova i consum del servei
- **Repte 5**: prova del flux híbrid i de la dependència externa
- **fase final**: verificació global del sistema i de les correccions aplicades

### 3. Documentació com a evidència transversal

També és un solapament bo perquè la documentació evoluciona:

- base tècnica i arrencada
- comportament funcional
- decisions arquitectòniques
- contracte i consum de serveis
- integració externa
- documentació final de lliurament, ús i manteniment

---

## Solapaments a vigilar

### 1. Fase final convertida en “nou Repte 3”

És un risc clar.

Si la fase final es dedica sobretot a refactoritzar indefinidament o a “netejar” arquitectura sense límit, es menja el sentit específic del Repte 3.

**Decisió recomanada**

La fase final ha d’estar acotada per incidències i millores prioritzades, no per refactorització oberta.

### 2. Fase final convertida en “nou Repte 4 o 5”

També és un risc.

Si la fase final es dedica sobretot a crear nous endpoints o a afegir noves integracions externes, es desplaça el focus cap a nova construcció en lloc de síntesi i tancament.

**Decisió recomanada**

La fase final ha de treballar principalment sobre estabilització, prova, documentació, operació mínima i defensa.

### 3. Defensa final desconnectada del producte real

És el risc metodològic més important.

Una defensa oral sense contrast amb codi, proves, commits i canvis reals no verifica prou l’aprenentatge.

**Decisió recomanada**

Mantindre obligatòries:

- demo real
- revisió d’evidències
- contrast amb repositori
- i, quan siga viable, canvi menut en directe o pregunta de transferència

---

## Buits o ajustos recomanats

### Ajust 1. Fer explícita la frontera Repte 5 → fase final

Convé incloure a la fase final una frase de límit com esta:

> La fase final no amplia el producte amb un nou bloc temàtic principal, sinó que reactiva, estabilitza, verifica i defensa el producte construït en els reptes anteriors.

### Ajust 2. Fer visible que la fase final exigix canvis reals

Convé reforçar una idea com esta:

> La fase final no es considera superada amb una simple presentació del producte; ha d’existir auditoria, correcció o millora real, prova mínima, documentació final i defensa tècnica.

### Ajust 3. Acotar l’automatització

Convé recordar que la peça d’automatització o procediment operatiu ha de ser útil i proporcionada, sense convertir la fase final en un bloc nou massa orientat a infraestructura.

---

## Judici global sobre la seqüència completa

La seqüència actual es pot llegir així:

- **Repte 1**: arrencada professional i primer flux mínim
- **Repte 2**: processament complet fins a acció protegida
- **Repte 3**: professionalització arquitectònica i persistència suficient
- **Repte 4**: exposició del cas d’ús com a servei reusable i consumible
- **Repte 5**: integració de fonts externes per generar funcionalitat híbrida
- **fase final integradora**: tancament professional, verificació global i defensa d’autoria

És una seqüència coherent, escalable i curricularment defensable si es mantenen clares les fronteres entre:

- construcció inicial
- funcionalitat completa
- mantenibilitat interna
- interoperabilitat pròpia
- interoperabilitat externa
- síntesi, tancament i defensa

---

## Decisions de control final

Abans de donar la seqüència per tancada, convé revisar:

- si cada repte canvia realment l’objecte principal d’avaluació
- si la fase final no reobri blocs ja tancats
- si el pes de la defensa final està equilibrat amb evidències tècniques reals
- si la verificació d’autoria està distribuïda al llarg de la seqüència i no sols al final
- si la seqüència completa es pot explicar de manera senzilla a alumnat, departament i inspecció

---

## Ús recomanat del document

Este document es pot usar per a:

- revisió interna global del disseny del mòdul
- coordinació docent
- comprovació final de solapaments i fronteres
- justificació curricular i metodològica
- revisió de la matriu d’avaluació general
- preparació de la programació d’aula i de la defensa del redisseny del mòdul

---
