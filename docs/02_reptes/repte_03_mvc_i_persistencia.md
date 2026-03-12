# Repte 3. Migració a MVC i persistència segura

## Finalitat
Convertir el backend funcional dels reptes anteriors en una base mantenible i escalable mitjançant MVC (o arquitectura equivalent), amb persistència segura i qualitat tècnica verificable.

Este repte és el punt de pas de “funciona” a “es pot mantindre”, i prepara el producte per a la publicació d’API del Repte 4 i per a la integració híbrida del Repte 5.
S’executa dins del model de treball per reptes del mòdul i amb enfocament d’evidències autèntiques.

## Relació amb resultats d’aprenentatge
- **RA5 (principal):** organitzar el codi per capes/rols tècnics amb criteris de mantenibilitat.
- **RA6 (principal):** consolidar model de dades, persistència i accés segur a BD.
- **Reforç de qualitat tècnica (preparació RA7/RA8):** deixar base sòlida per publicar API, controlar errors i ampliar proves.

Resultat esperat:
- arquitectura més clara
- dades persistents coherents
- validacions i errors gestionats
- proves mínimes que reduïsquen regressions

## Context professional
L’equip ha lliurat una versió inicial funcional (kickoff + sessions), però el codi ha crescut amb dependències acoblades i sense una estructura estable per a evolució.

En un entorn professional real, abans d’obrir serveis a tercers, cal:
- separar responsabilitats de manera explícita
- assegurar persistència i integritat de dades
- establir una base de qualitat mínima per evitar deute tècnic crític

## Problema o encàrrec inicial
**Encàrrec:** “Refactoritzeu el backend actual a MVC o equivalent, consolideu persistència segura i entregueu evidències de qualitat suficients per passar a fase d’API.”

Restriccions:
- no es tracta de reescriure tot el producte des de zero
- cal preservar funcionalitat existent del repte anterior
- cada canvi ha d’estar justificat i verificat
- l’ús de IA és permés, però sempre traçable i validat

## Producte final
En finalitzar el repte, el producte ha d’incloure com a mínim:
- estructura MVC o equivalent aplicada al domini triat
- model de dades persistent amb operacions segures
- validacions d’entrada i tractament d’errors coherent
- proves mínimes executables (unitàries i/o integració)
- documentació tècnica actualitzada de decisions i execució

## Compatibilitat amb itineraris tecnològics
Este repte és compatible amb els itineraris tecnològics guiats del mòdul:
- **PHP + Laravel**
- **Node.js + Express o Nest**
- **Python + FastAPI**

El criteri d’avaluació és equivalent entre itineraris: canvia la implementació, no els objectius docents ni les evidències exigides.

## Seqüència de treball
1. **Diagnosi del codi actual**
   - identificar acoblaments, duplicacions i punts crítics de persistència.
2. **Disseny de refactorització**
   - definir l’estructura MVC/equivalent i pla de migració per iteracions curtes.
3. **Migració de capes i casos d’ús**
   - separar controladors, serveis/casos d’ús i capa de dades.
4. **Consolidació de persistència segura**
   - ajustar model, consultes, validacions i regles de consistència.
5. **Qualitat mínima i regressió**
   - incorporar proves bàsiques i validar fluxos crítics.
6. **Documentació i traspàs a Repte 4**
   - deixar registre de decisions i estat tècnic per a publicació d’API.

## Activitats o microtasques
- auditar el repositori i crear issue de refactorització del repte
- definir convencions d’estructura (MVC/equivalent) i criteris de carpeta
- migrar un primer cas d’ús complet com a patró
- traslladar persistència a capa dedicada (repositori/ORM/servei de dades)
- afegir validacions d’entrada i tractament d’errors de negoci
- revisar consultes i accessos per seguretat i robustesa
- implementar proves mínimes de flux crític i persistència
- actualitzar README tècnic i registre de decisions

## Materials i apunts associats
- [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md): fixa requisits mínims comuns i components base del producte evolutiu.
- [Mapa de materials actuals -> nova estructura](../04_materials/mapa_materials_actuals.md): connecta explícitament els blocs 3 i 4 amb el Repte 3, i el bloc 5 com a reforç de qualitat.
- model d’itineraris tecnològics del mòdul (Laravel / Express-Nest / FastAPI): determina vies guiades equivalents per executar el repte.

## Paper de la IA
La IA es pot usar per:
- proposar estratègies de refactorització per iteracions
- suggerir estructura base de capes o patrons de persistència
- generar tests inicials o casos de validació
- ajudar a detectar punts de risc en gestió d’errors

Condició obligatòria:
- tota proposta assistida per IA s’ha de validar amb execució real, proves i revisió de codi de l’equip.

## Evidències d’aprenentatge
Evidències mínimes i autèntiques del repte:
- issue principal i microtasques resoltes amb traçabilitat
- commits que mostren la migració incremental a MVC/equivalent
- codi amb persistència segura i validacions aplicades
- execució de proves mínimes i resultat registrat
- documentació tècnica actualitzada (README + decisions)
- registre d’ús de IA quan corresponga

## Instruments d’avaluació
- [Rúbrica base de reptes](../03_avaluacio/rubrica_base_reptes.md) adaptada al Repte 3, amb pes principal en RA5 i RA6
- checklist de qualitat de codi i mantenibilitat arquitectònica
- checklist de persistència segura (validacions, errors, coherència de dades)
- revisió de proves executades i cobertura mínima funcional
- defensa tècnica breu centrada en decisions i trade-offs

## Riscos d’ús inadequat de la IA
- aplicar refactoritzacions proposades per IA sense entendre impacte
- introduir capes innecessàries que compliquen el manteniment
- acceptar consultes o codi de persistència insegur sense revisió
- presentar proves generades automàticament sense correspondència real amb el codi

## Mesures de verificació
- demostració de fluxos crítics abans/després de la refactorització
- revisió dirigida de commits per comprovar evolució real i no “còpia final”
- execució en directe de proves mínimes i comprovació de resultats
- contrast entre AI log, canvis aplicats i justificació oral
- revisió puntual de control d’errors i integritat de dades

## Entorn professional
Marc de treball mínim del repte:
- repositori Git/GitHub amb issues, branques i commits coherents
- entorn local reproductible amb base de dades del projecte
- eina de proves i depuració pròpia de cada stack
- documentació tècnica orientada a onboarding i continuïtat d’equip
- registre d’incidències i decisions de manteniment

## Definition of done del repte
El Repte 3 es considera completat quan es compleixen totes les condicions següents:
- el backend està refactoritzat a MVC o arquitectura equivalent, amb responsabilitats separades
- la persistència és funcional i segura en els casos d’ús prioritaris
- hi ha validacions d’entrada i tractament d’errors coherents
- existeixen proves mínimes executades amb evidència verificable
- la documentació reflecteix l’estat real del codi i les decisions tècniques
- la solució queda preparada per iniciar el Repte 4 (API i consum) sense reestructuració crítica addicional
