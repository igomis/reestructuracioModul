# Repte 2. Mòdul de gestió d’usuaris i sessions

## Finalitat
Construir la primera base funcional del producte backend amb gestió d’usuaris, autenticació i sessions, aplicant validació d’entrades i tractament controlat d’errors.

Este repte transforma el kickoff tècnic en funcionalitat real de negoci i deixa el projecte preparat per a la refactorització arquitectònica del Repte 3.

## Relació amb resultats d’aprenentatge
- **RA2 (principal):** implementar lògica de servidor per processar peticions, dades i respostes.
- **RA3 (principal):** gestionar sessions i autenticació amb control d’accés coherent.
- **RA4 (principal):** construir funcionalitat dinàmica usable en context de producte real.

Contribució esperada del repte:
- flux funcional complet d’accés d’usuari (alta/login/logout/sessió)
- validació i errors controlats en casos habituals i casos límit
- base estable per escalar a MVC/persistència del Repte 3

## Context professional
Després del kickoff, l’equip ha de demostrar que el servei backend pot gestionar usuaris reals amb garanties mínimes de seguretat i traçabilitat.

En un entorn professional, este pas és crític perquè:
- valida que l’aplicació gestiona estat i identitat d’usuari
- evita que el creixement posterior es faça sobre fluxos inestables
- aporta evidències funcionals abans d’afrontar una reestructuració més profunda

## Problema o encàrrec inicial
**Encàrrec:** “Implementeu el mòdul d’usuaris i sessions del producte base, amb autenticació funcional, validacions consistents i evidències verificables de qualitat mínima.”

Restriccions del repte:
- no avançar funcionalitats secundàries si la base d’autenticació no és estable
- evitar acoblar lògica de negoci i lògica de sessió sense criteri
- registrar decisions i incidències de manera traçable
- usar IA només com a suport verificable

## Producte final
El lliurable mínim del Repte 2 ha d’incloure:
- registre o alta d’usuari amb validacions bàsiques
- inici i tancament de sessió operatius
- control d’accés a recursos protegits
- tractament d’errors d’autenticació i validació
- proves mínimes de flux funcional i casos d’error
- documentació tècnica actualitzada del mòdul

## Compatibilitat amb el producte base
Este repte s’alinea directament amb el document [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md), perquè consolida components obligatoris del producte evolutiu:
- backend real amb casos d’ús no trivials
- autenticació i control d’accés
- persistència inicial i validació de dades
- proves i documentació verificables
- reutilització de la base tècnica establida al Repte 1 (repositori, convencions i traçabilitat)

A més, deixa preparada la continuïtat cap al [Repte 3. Migració a MVC i persistència segura](repte_03_mvc_i_persistencia.md), on esta funcionalitat es reestructurarà amb criteris de mantenibilitat.

## Seqüència de treball
1. **Anàlisi funcional del mòdul d’accés**
   - definir fluxos de registre, login, logout i control de sessió.
2. **Disseny de dades i validacions**
   - establir camps, regles de validació i missatges d’error.
3. **Implementació de sessions i autenticació**
   - construir la lògica de control d’accés i persistència associada.
4. **Gestió d’errors i casos límit**
   - cobrir credencials incorrectes, sessions expirades i accessos no autoritzats.
5. **Proves i verificació funcional**
   - executar proves mínimes de casos positius i negatius.
6. **Documentació i transició a Repte 3**
   - deixar traça tècnica del mòdul i de punts de millora arquitectònica.

## Activitats o microtasques
- crear issue principal del Repte 2 i descompondre-la en microtasques
- modelar dades mínimes d’usuari i regles de validació
- implementar alta/registre d’usuari
- implementar login/logout i comprovació de sessió activa
- protegir una o més rutes/operacions per autenticació
- definir respostes d’error consistents per validació i accés
- crear proves bàsiques de flux d’accés i casos límit
- actualitzar README amb instruccions d’ús i validació del mòdul

## Materials i apunts associats
- [Repte 1. Kickoff tècnic d’un servei web backend](repte_01_kickoff_backend.md): base tècnica i artefactes que es reutilitzen en este repte.
- [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md): marc de requisits comuns del producte evolutiu.
- [Mapa de materials actuals -> nova estructura](../04_materials/mapa_materials_actuals.md): connexió del Bloc 2 amb RA2-RA4 i reforços posteriors.
- [Repte 3. Migració a MVC i persistència segura](repte_03_mvc_i_persistencia.md): continuïtat directa del codi funcional cap a arquitectura mantenible.
- materials de sessions/autenticació i validació del bloc de servidor (ús pràctic orientat a producte).

## Paper de la IA
La IA pot ajudar en:
- proposta d’estructura inicial de fluxos d’autenticació
- generació de casos de prova per credencials i sessions
- revisió de validacions i missatges d’error
- suport en debugging de comportaments inesperats

Condició obligatòria:
- tota aportació assistida per IA s’ha de validar amb execució real, proves i justificació tècnica de l’equip.

## Evidències d’aprenentatge
Evidències mínimes i autèntiques del repte:
- issue principal amb microtasques i estat de resolució
- commits coherents amb l’evolució del mòdul d’usuaris/sessions
- demostració funcional de registre, login, logout i control d’accés
- evidència de validacions i gestió d’errors
- proves mínimes executades amb resultat registrat
- documentació tècnica actualitzada i AI log quan corresponga

## Instruments d’avaluació
- [Rúbrica base de reptes](../03_avaluacio/rubrica_base_reptes.md) adaptada al Repte 2 (pes principal en RA2, RA3 i RA4)
- checklist de funcionalitat d’autenticació i gestió de sessió
- checklist de validació d’entrades i tractament d’errors
- revisió de proves mínimes i traçabilitat en repositori
- defensa tècnica breu centrada en decisions i robustesa funcional

## Riscos d’ús inadequat de la IA
- copiar fluxos d’autenticació sense comprendre impacte en seguretat
- acceptar validacions incompletes o incoherents sense revisar
- generar proves artificials que no representen casos reals
- no poder justificar decisions aplicades a sessions i control d’accés

## Mesures de verificació
- execució en directe de casos positius i negatius (login correcte/incorrecte, accés autoritzat/no autoritzat)
- comprovació de comportament de sessió en diferents escenaris
- revisió de coherència entre validacions definides i errors retornats
- contrast entre AI log, commits i resultat funcional real
- preguntes tècniques breus per comprovar autoria i comprensió

## Entorn professional
Marc mínim de treball del repte:
- Git/GitHub amb issues, commits i branques de treball traçables
- entorn local executable amb configuració reproduïble
- registre d’incidències i correccions de validació/autenticació
- proves funcionals mínimes integrades en el flux de desenvolupament
- documentació tècnica orientada a ús d’equip i continuïtat

## Definition of done del repte
El Repte 2 es considera completat quan:
- existeix un flux funcional complet d’usuaris i sessions (registre/login/logout/control d’accés)
- la validació d’entrades i el tractament d’errors són coherents i verificables
- hi ha evidència de proves mínimes sobre casos crítics i casos límit
- la documentació reflecteix l’estat real del mòdul implementat
- el codi i les decisions queden preparats per iniciar la migració arquitectònica del Repte 3
