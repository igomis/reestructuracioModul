# Repte 5. Aplicació web híbrida i integració de serveis externs

## Fitxa canònica del repte

- **Funció didàctica principal**: síntesi amb nucli mínim obligatori de `RA9` i ampliació avançada opcional.
- **Objectiu**: integrar fonts o serveis externs dins del projecte base per generar una funcionalitat híbrida amb valor real.
- **Producte esperat**: integració funcional amb consum extern, transformació de dades, tractament mínim d'errors i documentació tècnica.
- **Evidències**: demo del flux complet, proves o verificacions d'integració, documentació tècnica, mapping de dades, comparativa font externa / transformació / resultat final i traçabilitat de treball.
- **Paper de la IA**: ús assistit per IA permés per explorar fonts, connectors o transformacions; els límits i la delegació excessiva depenen de [us-ia-professorat-i-alumnat.md](../us-ia-professorat-i-alumnat.md).
- **Relació amb el projecte base**: obri el projecte base a l'exterior i tanca la seqüència de construcció abans de la defensa tècnica.
- **Checkpoint de control**: selecció justificada de la font externa abans de construir la integració i demo final amb cas positiu, cas d'error, contrast del mapa d'integració i mini defensa.
- **Instrument dominant**: checklist d'integració híbrida amb valor de producte.
- **Instrument de comprensió**: mini defensa tècnica sobre contracte extern, mapping i aportació real al producte.
- **Instrument de control de delegació excessiva**: revisió de commit rellevant comentat, contrast amb `AI log` i prova guiada sobre la transformació o l'orquestració.
- **Instrument de recuperació o millora**: reducció d'abast a una sola font externa, un cas d'ús híbrid i una nova demo completa.

## Justificació docent

- **Evidència principal**: flux híbrid complet amb font externa, transformació i valor observable dins del producte.
- **Evidències secundàries**: mapping de dades, prova d'error, documentació final, traçabilitat de treball i mini defensa.
- **Mínim suficient**: una connexió vistosa o un workflow aïllat no compta; cal integració útil, reproduïble i defensable.
- **Feedback previst**: validació de la font abans de construir i demo final amb cas positiu, fallada rellevant i defensa curta.

## 1. Visió general del repte

**Finalitat del repte**

Construir una funcionalitat híbrida del projecte que combine recursos propis amb serveis, dades o codi de tercers per generar valor nou i útil dins del producte.

Este repte no s’entén com una simple connexió a una API externa ni com una demostració superficial de consum de dades alienes. El seu sentit és integrar informació o serveis heterogenis de manera crítica, transformada i documentada, perquè el sistema faça alguna cosa nova que abans no podia fer.

**Producte principal del repte**

Una funcionalitat híbrid integrada en el projecte, amb:

- consum real d’una o més fonts externes
- tractament o transformació de la informació rebuda
- combinació amb dades o serveis propis del projecte quan siga pertinent
- generació d’una funcionalitat nova amb valor real
- tractament mínim d’errors i incidències d’integració
- proves mínimes o verificacions registrades
- documentació tècnica de la integració

**Context professional simul·lat o realista**

L’equip ja disposa d’un backend funcional, estructurat i capaç d’exposar serveis propis.

Ara ha de demostrar una competència molt habitual en entorns professionals: reutilitzar serveis, fonts de dades o components externs per ampliar el valor del sistema sense reconstruir-ho tot des de zero.

**Relació amb el projecte global del curs**

Este repte reutilitza el sistema construït fins ara i l’obri a l’exterior.

En el Repte 4, el sistema aprenia a exposar serveis propis.

En el Repte 5, el sistema aprén a consumir, integrar, transformar i reaprofitar informació o serveis externs per generar una aplicació híbrida amb sentit.

---

## 2. Relació amb resultats d'aprenentatge

**Resultat d'aprenentatge principal**

- **RA9**: desenvolupa aplicacions web híbrides seleccionant, integrant i transformant fonts o serveis externs de manera útil i verificable.

**Resultats d'aprenentatge de suport**

- **RA7**: només quan la integració reutilitza, consumeix o orquestra serveis web propis o externs.
- **RA8**: quan la integració modifica una resposta dinàmica, una vista o un flux renderitzat en servidor.
- **RA6**: només si la integració requereix persistir, consultar o protegir dades pròpies vinculades al flux híbrid.

**Justificació curricular**

`R5` ha de mantindre `RA9` com a centre. El valor del repte no està en cridar una API externa, sinó en seleccionar una font adequada, entendre'n el contracte, transformar la resposta i integrar-la dins d'una funcionalitat real del projecte.

Els criteris de `RA7`, `RA8` i `RA6` només apareixen com a suport quan fan falta per demostrar la integració. No han de substituir el nucli del repte ni convertir `R5` en una repetició de l'API de `R4` o de la persistència de `R3`.

---

## 3. Microprojectes i criteris d'avaluació

> **Norma del repte**
>
> - Cap microprojecte apareix sense el camp **RA avaluat, CA avaluats i RA de context**.
> - Cada microprojecte ha de deixar una evidència verificable de la integració.
> - El mínim obligatori és una sola integració híbrida completa, útil i defensable.
> - Les integracions múltiples o orquestracions avançades són ampliació, no substitució del nucli.

### Microrepte R5M1 — Selecció de font externa i disseny de la integració

**Tipus**

Microtasca d'investigació i decisió tècnica.

**Objectiu**

Triar una font, servei extern o repositori heterogeni que aporte valor real al producte i definir com s'integrarà.

**Tasca**

L'equip concreta:

- quina font o servei extern usarà
- quin problema del producte resol o millora
- quin contracte, format o mecanisme d'accés té
- quines dades es necessiten i quines es descarten
- quins riscos hi ha: límits, errors, permisos, dependència externa o qualitat de dades
- quin flux híbrid es construirà

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA9**
- **CA avaluats**: **RA9.a**, **RA9.b**
- **RA de context**: **RA7.a**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat identifica fonts externes o repositoris heterogenis útils per al projecte.
- L'alumnat compara opcions i justifica la tria segons valor funcional, viabilitat i risc.
- L'alumnat entén el contracte extern abans de construir la integració.

**Evidències obligatòries**

- comparativa curta de fonts o serveis
- mapa inicial d'integració
- justificació de la font triada
- llista de riscos i límits

**Instrument d'avaluació**

Checklist de selecció i viabilitat.

**Pes orientatiu dins del repte**

15%

### Microrepte R5M2 — Connexió amb la font externa i recuperació real

**Tipus**

Microprojecte procedimental.

**Objectiu**

Implementar una connexió funcional amb la font externa i demostrar que es recuperen dades reals o resposta real del servei.

**Tasca**

L'equip implementa:

- connector, client HTTP, consulta, webhook o mecanisme equivalent
- configuració mínima necessària
- cas positiu de recuperació
- cas d'error o indisponibilitat
- registre de què s'ha rebut realment

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA9**
- **CA avaluats**: **RA9.c**, **RA9.f**
- **RA de context**: **RA7.d**, **RA7.e**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat accedeix a una font externa de manera funcional i verificable.
- L'alumnat tracta errors bàsics de connexió, resposta buida o resposta inesperada.
- L'alumnat pot explicar què ve de fora i què pertany al sistema propi.

**Evidències obligatòries**

- codi del connector o integració
- demo de recuperació real
- registre o captura de resposta
- prova d'error controlat

**Instrument d'avaluació**

Rúbrica de connexió i robustesa mínima.

**Pes orientatiu dins del repte**

20%

### Microrepte R5M3 — Transformació, mapping i valor afegit

**Tipus**

Microprojecte procedimental.

**Objectiu**

Transformar la informació externa perquè tinga sentit dins del domini del projecte.

**Tasca**

L'equip defineix i implementa:

- mapping entre dades externes i dades internes
- filtrat, normalització o enriquiment
- criteris per descartar dades no útils
- comparativa entre resposta externa i resultat integrat
- justificació del valor afegit

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA9**
- **CA avaluats**: **RA9.d**, **RA9.e**
- **RA de context**: **RA6.c**, **RA6.d**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat no es limita a mostrar dades externes: les adapta al producte.
- L'alumnat justifica quines transformacions fa i per què.
- L'alumnat manté coherència entre font externa, model intern i ús final.

**Evidències obligatòries**

- taula o esquema de mapping
- codi de transformació
- comparativa font externa / resultat final
- demo del valor generat

**Instrument d'avaluació**

Rúbrica de transformació i valor funcional.

**Pes orientatiu dins del repte**

20%

### Microrepte R5M4 — Integració de la funcionalitat híbrida en el producte

**Tipus**

Microprojecte procedimental.

**Objectiu**

Integrar el resultat transformat en una funcionalitat real del projecte.

**Tasca**

L'equip connecta la integració amb:

- una pantalla, flux, endpoint, procés o automatització del producte
- dades pròpies quan siga pertinent
- resposta visible o efecte funcional observable
- restriccions bàsiques d'ús o control d'accés si cal

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA9**
- **CA avaluats**: **RA9.e**, **RA9.f**
- **RA de context**: **RA8.f**, **RA7.f**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat integra la font externa dins del producte i no com a demo aïllada.
- L'alumnat mostra un resultat funcional nou o millor respecte a l'estat anterior.
- L'alumnat pot demostrar el flux complet de punta a punta.

**Evidències obligatòries**

- funcionalitat híbrida integrada
- demo completa
- comparativa abans/després
- commit rellevant comentat

**Instrument d'avaluació**

Rúbrica d'integració híbrida.

**Pes orientatiu dins del repte**

25%

### Microrepte R5M5 — Prova, documentació i defensa de la integració

**Tipus**

Microprojecte de tancament i verificació.

**Objectiu**

Fer reproduïble, verificable i defensable la integració construïda.

**Tasca**

L'equip prepara:

- proves o verificacions del cas positiu
- proves o verificacions d'error
- documentació tècnica de la font, configuració i flux
- límits coneguts
- mini defensa del contracte extern, mapping i valor aportat

**RA avaluat, CA avaluats i RA de context**

- **RA avaluat**: **RA9**
- **CA avaluats**: **RA9.g**, **RA9.h**
- **RA de context**: **RA7.h**
- **Criteri de qualificació**: només els CA avaluats generen nota en este microrepte; el context no es pondera ací.

**Descripció dels CA en llenguatge docent**

- L'alumnat prova i documenta la integració amb criteri professional.
- L'alumnat identifica limitacions reals i dependències externes.
- L'alumnat defensa l'autoria i les decisions preses, especialment si ha usat IA.

**Evidències obligatòries**

- registre de proves
- documentació tècnica
- mapa final d'integració
- AI log quan corresponga
- mini defensa tècnica

**Instrument d'avaluació**

Checklist de tancament i defensa.

**Pes orientatiu dins del repte**

20%

---

## 4. Taula resum de microprojectes i criteris d'avaluació

| Microprojecte | Tipus | Producte o lliurable | RA avaluat | CA avaluats | RA de context | Evidències principals | Instrument | Pes orientatiu |
|---|---|---|---|---|---|---|---|---:|
| R5M1 | Investigació / decisió | Font externa triada i mapa d'integració | RA9 | RA9.a, RA9.b | RA7.a | comparativa, justificació, mapa inicial, riscos | checklist | 15% |
| R5M2 | Procedimental | Connexió funcional amb font externa | RA9 | RA9.c, RA9.f | RA7.d, RA7.e | connector, resposta real, cas d'error | rúbrica | 20% |
| R5M3 | Procedimental | Mapping i transformació útil | RA9 | RA9.d, RA9.e | RA6.c, RA6.d | esquema de mapping, transformació, comparativa | rúbrica | 20% |
| R5M4 | Integració | Funcionalitat híbrida integrada | RA9 | RA9.e, RA9.f | RA8.f, RA7.f | demo completa, abans/després, commit comentat | rúbrica | 25% |
| R5M5 | Tancament / verificació | Proves, documentació i defensa | RA9 | RA9.g, RA9.h | RA7.h | registre de proves, documentació, mapa final, defensa | checklist | 20% |

---

## 5. Criteri de superació

El repte es considera superat quan:

- hi ha una font externa triada amb criteri;
- la connexió o integració recupera resposta real;
- la informació externa es transforma o adapta al domini;
- el resultat queda integrat en una funcionalitat real del producte;
- hi ha prova positiva i prova d'error;
- la documentació permet entendre la font, la configuració i el flux;
- l'alumnat pot defensar què ve de fora, què transforma el sistema i quin valor nou aporta.
