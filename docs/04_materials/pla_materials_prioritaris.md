# Pla de materials prioritaris del mòdul

## Finalitat del document
Convertir el mapa general de materials del mòdul en un pla de producció real, prioritzat i executable, orientat a crear les peces noves o adaptades que fan falta per donar suport directe als reptes del curs i al projecte base.

Este document no redefineix el currículum ni substituïx el mapa de transformació. La seua funció és baixar un nivell més: decidir què s'ha de produir primer, en quin format, per a quin ús docent i amb quina relació amb els reptes, els itineraris tecnològics i les evidències autèntiques del repositori.

Punt de partida actual:
- el repositori ja disposa de mapa de materials, fitxes de reptes avançades i enunciat base del projecte
- els directoris de `docs/04_materials/` per repte existixen, però encara no hi ha un paquet operatiu de materials nous produït
- el focus real del repositori continua sent connectar reptes, projecte base i materials adaptats prioritaris

## Criteris de priorització
Els materials nous s'han de prioritzar segons estos criteris:

- **impacte immediat sobre els reptes actius**: primer allò que desbloqueja o millora directament els Reptes 2, 3, 4 i 5
- **reutilització transversal**: primer els materials que poden usar tots els equips, dominis i itineraris
- **valor d'entorn professional realista**: prioritat per a materials que generen artefactes com README, ADR, proves, col·leccions API, checklists o AI log
- **capacitat de generar evidències autèntiques**: prioritat per a materials que deixen rastre verificable al repositori
- **dependència del projecte base**: prioritat per a materials que ajuden a cobrir autenticació, persistència, API, integració i manteniment
- **compatibilitat entre itineraris**: prioritat per a bases comunes que després es puguen adaptar a Laravel, Express o Nest i FastAPI
- **ús verificable de la IA**: prioritat per a peces que marquen com usar IA amb rastre, validació i defensa tècnica
- **cost docent assumible**: primer materials que poden produir-se i revisar sense duplicar tota la programació

## Tipologies de materials a produir
El pla distingix tres famílies principals de materials:

### Materials comuns de mòdul
Són peces reutilitzables per a tot el curs, independentment del repte o de l'itinerari tecnològic. Han de fixar criteris compartits de treball, qualitat, documentació i verificació.

Materials comuns mínims:
- guia de Git i flux de treball professional mínim
- plantilla i guia d'ús de README tècnic i ADR
- guia de testing, debugging i registre d'incidències
- guia d'ús verificable de la IA amb AI log mínim

### Materials per repte
Són peces orientades a resoldre el nucli tècnic d'un repte concret. Han d'ajudar a passar de l'enunciat a l'execució del producte i a la generació d'evidències del repte.

Materials nuclears prioritaris:
- materials del Repte 2 sobre sessions, autenticació i validació
- materials del Repte 3 sobre MVC o equivalent, persistència segura i proves
- materials del Repte 4 sobre contracte API, documentació i consum
- materials del Repte 5 sobre integració híbrida, n8n o equivalent i manteniment

### Materials per itinerari
Són peces específiques per stack que no canvien el repte, però sí la manera d'implementar-lo. Han de partir d'una base comuna i oferir traduccions operatives per a cada itinerari autoritzat.

Itineraris a cobrir:
- Laravel
- Express o Nest
- FastAPI

## Materials prioritaris per ordre de producció
L'ordre recomanat de producció dels materials prioritaris és el següent:

| Ordre | Material prioritari | Tipus | Valor principal |
|---|---|---|---|
| 1 | Guia comuna de Git, branques, issues i commits per treball per reptes | comú de mòdul | fixa entorn professional realista i traçabilitat mínima |
| 2 | Plantilla operativa de README tècnic i ADR | comú de mòdul | homogenitza documentació i justificació de decisions |
| 3 | Guia comuna de testing, debugging i registre d'incidències | comú de mòdul | convertix la qualitat en evidència observable |
| 4 | Guia comuna d'ús verificable de la IA i AI log mínim | comú de mòdul | assegura assistència guiada i verificable |
| 5 | Pack nuclear del Repte 2: sessions, autenticació i validació del servidor | per repte | consolida la primera funcionalitat real del producte |
| 6 | Pack nuclear del Repte 3: MVC o equivalent, persistència segura i proves | per repte | resol la transició arquitectònica central del curs |
| 7 | Pack nuclear del Repte 4: contracte API, documentació i consum | per repte | obri el producte a integració i consum extern |
| 8 | Pack nuclear del Repte 5: integració híbrida, n8n o equivalent i manteniment | per repte | tanca el producte evolutiu amb valor professional real |
| 9 | Pack d'itinerari Laravel per a R3-R5 | per itinerari | facilita implementació guiada en PHP + Laravel |
| 10 | Pack d'itinerari Express o Nest per a R3-R5 | per itinerari | facilita implementació guiada en Node.js |
| 11 | Pack d'itinerari FastAPI per a R3-R5 | per itinerari | facilita implementació guiada en Python |

## Proposta inicial de paquets de materials
Es proposen els paquets següents com a primera planificació operativa:

| Paquet | Abast | Peces incloses | Resultat esperat |
|---|---|---|---|
| **P0. Base comuna de mòdul** | materials comuns | Git i workflow, README/ADR, testing/debugging, IA verificable | base única de treball professional i d'evidències autèntiques |
| **P1. R2 Sessions i autenticació** | materials per repte | flux d'usuari, validacions de servidor, control d'accés, casos de prova bàsics | desplegar autenticació funcional i verificable sobre el projecte base |
| **P2. R3 Arquitectura i persistència** | materials per repte | guia de migració a MVC o equivalent, persistència segura, proves mínimes, troubleshooting | estabilitzar la base mantenible del producte |
| **P3. R4 API i consum** | materials per repte | contracte API, documentació d'endpoints, col·lecció de proves, consum controlat | publicar i consumir una API coherent amb el model |
| **P4. R5 Integració i manteniment** | materials per repte | flux híbrid, integració amb servei extern o automatització, incidències, manteniment | tancar el producte amb integració realista i traçabilitat de manteniment |
| **P5. Itinerari Laravel** | materials per itinerari | arrencada guiada, patrons MVC de Laravel, persistència, API i testing de stack | oferir via específica homologable per a PHP + Laravel |
| **P6. Itinerari Express o Nest** | materials per itinerari | estructura de projecte, capes, persistència, API i testing en Node.js | oferir via específica homologable per a Express o Nest |
| **P7. Itinerari FastAPI** | materials per itinerari | estructura bàsica, models i validació, persistència, API i testing en Python | oferir via específica homologable per a FastAPI |

## Formats recomanats
Per evitar materials enciclopèdics i afavorir ús directe en els reptes, es recomanen estos formats:

- guies operatives curtes en `Markdown`
- checklists de lliurament i verificació
- plantilles reutilitzables de README, ADR, AI log i registre d'incidències
- fitxes de troubleshooting i debugging orientades a errors freqüents
- col·leccions de proves API o equivalents
- exemples mínims de projecte o estructura per itinerari
- documents de contracte o convencions d'API
- taules de validació i casos límit per repte

El format s'ha de decidir per valor docent i reutilització, no per aparença. Si una peça no ajuda a executar, provar, documentar o defensar el treball, no és prioritària.

## Distribució entre materials comuns i materials específics
La producció inicial s'hauria d'organitzar així:

| Família de materials | Pes recomanat inicial | Funció |
|---|---|---|
| **Materials comuns de mòdul** | 35% | establir base compartida de treball, documentació, qualitat i IA verificable |
| **Materials per repte** | 40% | resoldre el nucli docent i tècnic dels Reptes 2, 3, 4 i 5 |
| **Materials per itinerari** | 25% | traduir els reptes a Laravel, Express o Nest i FastAPI sense trencar l'equivalència |

Criteri de distribució:
- els materials comuns s'han de produir primer perquè afecten tot el mòdul
- els materials per repte són el nucli de la producció i concentren la major part del valor docent
- els materials per itinerari s'han de construir sobre bases comunes ja estabilitzades, especialment a partir de R3-R5

## Relació amb els reptes i el projecte base
El pla de materials ha de donar servei directe al producte evolutiu del curs:

| Àmbit | Connexió amb reptes | Connexió amb projecte base |
|---|---|---|
| Git i workflow | dona suport transversal a tots els reptes | assegura traçabilitat i entorn professional realista |
| README i ADR | naix en Repte 1 i continua en R2-R5 | sosté documentació tècnica operativa i decisions del producte |
| Testing, debugging i incidències | reforç transversal amb pes especial en R3-R5 | dona suport a qualitat, regressió i manteniment evolutiu |
| IA verificable i AI log | transversal a tots els reptes | manté la IA com a eina guiada i verificable |
| Material nuclear de R2 | centra sessions, autenticació i validació | cobrix model d'usuaris i control d'accés bàsic |
| Material nuclear de R3 | centra arquitectura, capes i persistència | cobrix estructura mantenible i model de dades persistent |
| Material nuclear de R4 | centra publicació i consum d'API | cobrix API publicada, contractes i documentació |
| Material nuclear de R5 | centra integració híbrida i manteniment | cobrix integració externa, automatització i traçabilitat |
| Materials d'itinerari | apliquen sobretot en R3-R5 | garantixen compatibilitat amb Laravel, Express o Nest i FastAPI |

## Ordre recomanat de producció real
La seqüència recomanada de producció no és només temàtica, sinó també dependent del valor que aporta cada peça:

1. **Produir la base comuna de mòdul**
   Git, README/ADR, testing/debugging i IA verificable han d'estar disponibles abans de desplegar paquets més específics.
2. **Produir el paquet nuclear del Repte 2**
   És el primer material de producte funcional i ajuda a connectar la base comuna amb la primera evidència real.
3. **Produir el paquet nuclear del Repte 3**
   És la peça arquitectònica central del curs i el punt on comencen a necessitar-se més fortament els itineraris.
4. **Produir en paral·lel els primers materials d'itinerari per al Repte 3**
   Convindrà obrir primer les guies específiques de Laravel, Express o Nest i FastAPI per MVC o equivalent, persistència i testing.
5. **Produir el paquet nuclear del Repte 4**
   Amb la base arquitectònica consolidada, ja té sentit publicar material específic de contracte API i consum.
6. **Estendre els materials d'itinerari cap al Repte 4**
   Cada stack necessitarà exemples homologables de publicació, autenticació d'API, documentació i proves.
7. **Produir el paquet nuclear del Repte 5**
   Només quan l'API i el manteniment bàsic estiguen madurs té sentit abordar integració híbrida i automatització.
8. **Estendre els materials d'itinerari cap al Repte 5**
   Les adaptacions de stack per integració, serveis externs i testing final s'han de fer ja sobre una base comuna estabilitzada.

## Definition of done del document
Este document es considera completat quan:
- definix un pla de producció de materials i no només un mapa general
- explicita criteris de priorització coherents amb el focus actual del repositori
- distingix clarament materials comuns de mòdul, materials per repte i materials per itinerari
- incorpora com a mínim Git, README/ADR, testing/debugging i ús verificable de la IA com a materials comuns
- incorpora materials nuclears per als Reptes 2, 3, 4 i 5
- incorpora materials específics per Laravel, Express o Nest i FastAPI
- connecta els paquets de materials amb el projecte base i amb les evidències autèntiques del mòdul
- proposa un ordre realista de producció per fases
