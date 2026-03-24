# Enunciat base del projecte del curs

## Finalitat del projecte
Desenvolupar durant el curs un producte backend realista, evolutiu i defensable que servisca com a fil conductor dels reptes del mòdul i permeta generar evidències autèntiques d'aprenentatge.

El projecte no s'entén com una pràctica aïllada ni com una demo puntual. Ha de funcionar com un encàrrec professional progressiu: comença amb una base operativa, creix per reptes i acaba amb una solució capaç de persistir dades, publicar API, integrar-se amb serveis externs i deixar rastre verificable del treball realitzat.

## Context professional
L'equip rep l'encàrrec de construir el backend base d'un producte intern o de servei que una organització podria posar en producció després d'una fase inicial de validació.

El client o l'àrea promotora no demana una maqueta acadèmica, sinó una base tècnica que permeta:
- treballar amb usuaris autenticats i casos d'ús recognoscibles
- persistir dades de manera segura i coherent
- exposar funcionalitat mitjançant una API consumible
- integrar el sistema amb processos externs o automatitzacions
- mantindre el producte amb criteris de qualitat, proves i traçabilitat

L'entorn de treball s'ha d'aproximar a un context professional realista: repositori amb historial coherent, issues o tasques, documentació tècnica útil, decisions justificades i evidències que es puguen revisar.

## Encàrrec base
Cada equip ha de seleccionar un domini admés i construir sobre ell un backend funcional que evolucione al llarg del curs. El resultat ha de ser prou concret per poder-se executar, provar i revisar, però també prou extensible per incorporar els reptes del mòdul sense haver de reiniciar el projecte.

L'objectiu no és fer el producte més gran possible, sinó arribar a una base sòlida i verificable amb valor tècnic clar.

Com a concretització operativa dels dominis admesos, este enunciat es desplega ara en [projectes_base_concretats.md](projectes_base_concretats.md), que fixa tres projectes base ja usables i més tancats per a treball docent, comparabilitat entre itineraris i defensa individual.

Criteri transversal d'exigència:
- cap repte del projecte es pot donar per resolt amb una tècnica aïllada
- cada tram ha d'aportar una funcionalitat professional mínima, recognoscible i defensable del mateix producte
- no es validarà un recorregut basat en esquelets, logins aïllats, APIs decoratives o integracions sense valor funcional

## Dominis admesos
Els únics dominis admesos per al projecte base són:

1. **Gestor d'incidències o tickets**
   Permet treballar amb creació, assignació, prioritat, estat, historial i seguiment d'incidències.
2. **Sistema de reserves o cites**
   Permet treballar amb disponibilitat, franges horàries, confirmacions, conflictes i validacions de negoci.
3. **Gestor intern de recursos o inventari**
   Permet treballar amb altes, baixes, moviments, disponibilitat, responsables i traçabilitat d'actius.

Qualsevol d'estos dominis és vàlid si permet cobrir els objectius tècnics mínims del projecte i sostindre la seqüència de reptes del curs.

La seua concreció operativa recomanada queda fixada així:
- gestor intern de recursos o inventari -> **gestor d'inventari amb rols i token d'operació**
- sistema de reserves o cites -> **sistema de reserves amb tokens de confirmació o cancel·lació**
- gestor d'incidències o tickets -> **gestor d'incidències amb invitació o seguiment extern tokenitzat**

El detall funcional, els actors obligatoris, els casos d'ús i els criteris d'assignació docent es troben en [projectes_base_concretats.md](projectes_base_concretats.md).

## Objectius tècnics mínims
El projecte base ha de cobrir, com a mínim, els objectius següents:

- disposar d'un backend real amb casos d'ús no trivials del domini triat
- fer créixer un mateix producte amb increments funcionals no trivials a cada repte
- tindre estructura mantenible en MVC o arquitectura equivalent, segons l'itinerari triat
- incorporar model de dades persistent amb evolució controlada i operacions segures
- implementar autenticació i control d'accés bàsic sobre usuaris i funcionalitats clau
- publicar una API clara i consumible per als casos d'ús principals del sistema
- incloure validacions d'entrada, tractament d'errors i criteris mínims de qualitat tècnica
- disposar de proves automatitzades mínimes sobre comportaments crítics
- aportar documentació tècnica operativa de posada en marxa, arquitectura i contractes API
- deixar preparat o implementat un punt d'integració amb servei extern, webhook o flux híbrid
- mantindre traçabilitat de l'evolució del producte amb commits, issues o artefactes equivalents

Si el domini triat no permet arribar de manera creïble a estos objectius, no és apte com a projecte base del curs.

## Compatibilitat amb itineraris tecnològics
L'enunciat és compatible amb els itineraris següents:
- **PHP + Laravel**
- **Node.js + Express o Nest**
- **Python + FastAPI**

La compatibilitat s'avalua per objectius, evidències i qualitat de la solució, no per identitat d'implementació interna. Cada itinerari pot resoldre l'encàrrec amb patrons i eines pròpies, sempre que mantinga un nivell equivalent de verificació i mantenibilitat.

## Relació amb els reptes del curs
El projecte base és la peça transversal que dona continuïtat al treball per reptes:

| Repte | Aportació al projecte base |
|---|---|
| Repte 1. Kickoff funcional | prepara el repositori, l'entorn de treball, la primera estructura i una primera peça funcional real del producte |
| Repte 2. Sessions, autenticació i primera funcionalitat de negoci | incorpora identitat, control d'accés i una primera funcionalitat de negoci autenticada |
| Repte 3. Migració a MVC i persistència segura | consolida arquitectura mantenible, persistència i qualitat tècnica sobre eixa funcionalitat real |
| Repte 4. Publicació i consum d'API | exposa casos d'ús principals del producte mitjançant una API documentada i consumible |
| Repte 5. Integració híbrida, automatització i manteniment | connecta el producte amb serveis externs o automatitzacions i demostra manteniment real sobre un flux complet |

Per tant, el projecte no s'entrega com una peça separada dels reptes. Cada repte ha d'aportar una part verificable del producte final.

## Lliurables obligatoris
El projecte base s'ha de poder defensar amb els lliurables mínims següents:

- repositori del projecte amb historial coherent de desenvolupament
- README tècnic amb instruccions de posada en marxa, dependències i execució
- descripció del domini triat, actors principals i casos d'ús prioritaris
- codi font del backend amb autenticació, persistència, API i estructura mantenible
- model de dades, migracions o mecanisme equivalent de persistència
- col·lecció de proves automatitzades mínimes i evidència de la seua execució
- documentació dels endpoints o contractes API rellevants
- registre de decisions tècniques i de canvis significatius
- evidències autèntiques de treball per reptes: issues, commits, tasques o artefactes equivalents
- registre d'ús de IA o AI log quan s'haja utilitzat assistència

## Paper de la IA
La IA es considera una eina de suport vàlida dins del projecte per:
- explorar alternatives de disseny
- proposar estructures inicials o microtasques
- generar esquelets de proves o documentació
- ajudar en debugging, refactorització o revisió de contractes

L'ús de IA només és acceptable si complix estes condicions:
- l'equip entén i pot explicar el resultat final
- tota proposta assistida per IA es verifica amb execució real, proves i revisió tècnica
- queda rastre de què s'ha acceptat, què s'ha descartat i com s'ha comprovat
- la IA no substituïx la defensa tècnica ni la validació del comportament del sistema

La regla del repositori es manté: IA com a eina guiada i verificable, mai com a justificació d'evidència no contrastada.

## Criteris de validació
El projecte base es considerarà vàlid si complix tots els criteris següents:

- el domini triat és un dels dominis admesos i està prou concretat
- el backend funciona sobre un entorn reproduïble i amb documentació útil
- hi ha autenticació, persistència, API i proves mínimes verificables
- la solució mostra una evolució real lligada als reptes del curs
- cada repte aporta una funcionalitat professional mínima i no només una tècnica aïllada
- existixen evidències autèntiques de treball i no només una entrega final compactada
- la documentació i els contractes API reflectixen l'estat real del codi
- l'ús de IA, si existix, és traçable, defensable i contrastat
- el conjunt és compatible amb un entorn professional realista de manteniment

No es validarà com a projecte base una solució que només tinga aparença funcional però no aporte traçabilitat, proves o capacitat real de defensa tècnica. Tampoc es validarà un projecte que reduïsca els reptes a peces trivials o decoratives sense densitat funcional suficient.

## Variant futura o extensió opcional
Com a línia futura, el projecte pot obrir una extensió relacionada amb tokenització, sempre com a evolució opcional i no com a requisit del projecte base.

Esta extensió pot orientar-se, per exemple, a tokens d'accés, invitació, confirmació, recuperació o traçabilitat, sempre que responga a una necessitat real del domini triat. La seua incorporació queda fora dels mínims obligatoris i només s'hauria d'abordar quan la base principal ja estiga consolidada.

En la concretització operativa actual, la tokenització es manté dins d'este mateix sentit funcional útil del backend. No s'entén com a línia `web3` ni com a especialització aliena al curs, sinó com a mecanisme de confirmació, operació, invitació o seguiment quan el domini realment ho demana.

## Definition of done del document
Este document es considera completat quan:
- definix un enunciat base usable i no un placeholder
- explicita la finalitat del projecte i el seu context professional
- fixa de manera inequívoca els dominis admesos
- concreta objectius tècnics mínims compatibles amb el projecte backend base del curs
- deixa clar el criteri transversal de no trivialitat funcional dels reptes
- manté compatibilitat amb Laravel, Express o Nest i FastAPI
- connecta el projecte amb el treball per reptes i amb les evidències autèntiques del repositori
- establix lliurables obligatoris, paper de la IA i criteris de validació
- deixa oberta una extensió futura vinculada a tokenització sense convertir-la en obligatòria
