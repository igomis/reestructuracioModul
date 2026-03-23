# Repte 2. Sessions, autenticació i primera funcionalitat de negoci

## Finalitat
Construir la primera funcionalitat de negoci real i autenticada del producte backend del curs: identificar usuaris, validar entrades, iniciar i tancar sessió i protegir operacions del domini triat amb un comportament coherent.

El registre, el login i el logout són només la infraestructura mínima del repte. El Repte 2 no es considera complet si l’alumnat només resol autenticació aïllada: ha d’existir almenys un flux de domini amb valor real, sotmés a rols, restriccions o regles d’accés.

Este repte transforma la base tècnica del Repte 1 en un mòdul usable, verificable i connectat amb necessitats professionals reals. Al mateix temps, deixa preparada una base funcional de sessions, autenticació i validació que el [Repte 3. Migració a MVC i persistència segura](repte_03_mvc_i_persistencia.md) haurà de reorganitzar i consolidar arquitectònicament.

## Relació amb resultats d'aprenentatge
- **RA2 (principal):** desenvolupar lògica de servidor per processar peticions, formularis, validacions i respostes amb control d'errors.
- **RA3 (principal):** implementar gestió d'estat, sessions i autenticació d'usuaris amb criteri funcional i control d'accés.
- **RA4 (principal):** construir funcionalitat web dinàmica orientada a un cas d'ús real del producte, no a exercicis aïllats.

Contribució curricular esperada:
- posar en marxa un flux complet de registre, login, logout i comprovació de sessió
- demostrar una primera funcionalitat de negoci autenticada amb restriccions d’accés o de rol
- demostrar validació del costat servidor i tractament consistent d'errors habituals i casos límit
- convertir els continguts del Bloc 2 en una seqüència de producte real, tal com marca el [Mapa de materials actuals -> transformació operativa](../04_materials/mapa_materials_actuals.md)
- preparar el codi i les decisions perquè el Repte 3 puga refactoritzar esta funcionalitat a MVC o arquitectura equivalent

## Context professional
Després del kickoff, l'equip ja disposa d'un repositori funcional, però encara no pot gestionar identitat d'usuari ni protegir operacions reals del producte. En qualsevol backend professional, este és el primer llindar de credibilitat funcional: abans d'ampliar el domini o publicar APIs, cal demostrar que el sistema sap qui és l'usuari, què pot fer i com respon davant dades incorrectes.

En un context de producte real, este repte és crític perquè:
- evita construir funcionalitat de negoci sobre fluxos d'accés improvisats
- obliga a definir regles de validació i respostes d'error comprensibles
- genera evidències observables del comportament real del backend
- deixa clar quin codi funciona i quin s'haurà de reestructurar més avant
- força a demostrar que el sistema ja resol una operació real del domini i no només un mòdul d'accés aïllat

## Problema o encàrrec inicial
**Encàrrec:** "Partint del producte backend base del curs, implementeu la primera funcionalitat de negoci autenticada del producte. El client intern necessita un flux mínim de registre i autenticació, però també una operació real del domini sotmesa a control d'accés, restriccions o rols, amb evidències verificables que el comportament és correcte."

Restriccions del repte:
- s'ha de treballar sobre el projecte base iniciat en el Repte 1, no sobre un exercici desconnectat
- la prioritat és la coherència funcional del flux d'accés, no l'acumulació de funcionalitats secundàries
- la validació s'ha de fer al servidor i ha de produir errors interpretables
- qualsevol decisió provisional de codi o estructura ha de quedar prou clara per poder-se refactoritzar al Repte 3
- la IA es pot usar com a suport, però mai com a substitut de comprensió, execució i verificació
- un formulari de login, registre i logout sense funcionalitat de domini no es considera suficient
- el repte ha d'incloure una operació real, per exemple inventari amb rols, incidències amb rols o reserves amb restriccions

## Producte final
El lliurable mínim del Repte 2 ha d'incloure:
- mòdul funcional d'usuaris integrat en el producte backend del curs
- registre o alta d'usuari amb validacions bàsiques i missatges d'error coherents
- login i logout operatius
- comprovació d'usuari autenticat o de sessió activa
- almenys una funcionalitat de domini no trivial protegida per control d'accés
- una regla de rol o restricció de negoci aplicada sobre eixa funcionalitat
- tractament consistent d'errors de validació, credencials incorrectes i accés no autoritzat
- proves mínimes o verificacions registrades de casos positius i negatius
- documentació tècnica actualitzada per a ús de l'equip

Exemples orientatius de mínim funcional acceptable:
- inventari amb rols: només cert perfil pot donar d'alta o modificar recursos
- incidències amb rols: un usuari crea incidències i un altre les gestiona o canvia d'estat
- reserves amb restriccions: només es pot reservar si hi ha disponibilitat o segons franges vàlides

## Compatibilitat amb el producte base
Este repte s'executa sobre el marc definit en [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md). Això implica que:
- no és una activitat aïllada, sinó la primera implementació funcional d'un producte evolutiu únic durant el curs
- cobrix una dimensió obligatòria del projecte base: **model d'usuaris i mecanisme d'autenticació**
- és compatible amb qualsevol domini proposat en el projecte base (gestor d'incidències, sistema de reserves o gestor intern de recursos), perquè tots necessiten control d'identitat i accés
- reutilitza els artefactes del Repte 1: repositori, convencions, README, traçabilitat i criteri de treball professional
- deixa identificats els punts que el [Repte 3. Migració a MVC i persistència segura](repte_03_mvc_i_persistencia.md) haurà de consolidar: separació de responsabilitats, persistència més robusta, validacions encapsulades i arquitectura mantenible
- no es considera vàlid un mòdul d'autenticació desacoblat d'un primer cas d'ús de negoci recognoscible

## Seqüència de treball
1. **Aterrar el cas d'ús dins del producte**
   Definir com encaixa l'accés d'usuaris en el domini triat i quina primera funcionalitat real quedarà protegida.
2. **Dissenyar el flux d'accés**
   Concretar registre, login, logout, persistència bàsica de l'usuari, comprovació de sessió i matriu bàsica de rols o restriccions.
3. **Definir la funcionalitat de negoci autenticada**
   Fixar l'operació real del domini, les condicions d'accés i els casos correctes i incorrectes que l'afecten.
4. **Definir validacions i errors**
   Establir camps obligatoris, restriccions mínimes, casos d'error i format esperat de resposta o feedback.
5. **Implementar el mòdul funcional**
   Construir la lògica de sessions i autenticació i connectar-la amb una primera necessitat real del producte.
6. **Verificar comportament i casos límit**
   Comprovar tant camins correctes com errors de credencials, accessos sense permís, rols incorrectes i dades invàlides.
7. **Documentar i preparar la transició**
   Registrar decisions, incidències, proves i punts de deute tècnic que passaran a refactorització en el Repte 3.

## Activitats o microtasques
- crear la issue principal del Repte 2 i descompondre-la en microtasques funcionals
- concretar l'escenari d'usuari que dona sentit al mòdul d'accés dins del producte base
- definir quin primer cas d'ús de negoci queda condicionat per autenticació, rol o restricció
- definir camps mínims d'usuari i matriu de validacions del costat servidor
- implementar registre o alta d'usuari
- implementar login, logout i comprovació d'usuari autenticat
- protegir almenys una ruta, acció o operació del domini triat amb valor real
- aplicar almenys una restricció de rol, permís o regla de negoci sobre eixa operació
- definir respostes d'error consistents per validació, autenticació i autorització bàsica
- provar casos positius, casos negatius i casos límit
- actualitzar README o documentació operativa amb instruccions de prova del mòdul
- deixar anotats els punts que en el Repte 3 hauran de passar a capes, serveis o persistència més segura

## Materials i apunts associats
- [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md): fixa el marc del producte evolutiu i identifica l'autenticació i el control d'accés com a component comú obligatori.
- [Mapa de materials actuals -> transformació operativa](../04_materials/mapa_materials_actuals.md): situa el **Bloc 2. PHP** com a nucli del repte i el **Bloc 5. Seguretat i reactivitat** com a reforç de qualitat, debugging i control.
- [Repte 3. Migració a MVC i persistència segura](repte_03_mvc_i_persistencia.md): reutilitza el codi funcional generat ací per separar responsabilitats, consolidar persistència i ampliar qualitat tècnica.
- [Repte 1. Kickoff funcional d'un servei web backend](repte_01_kickoff_backend.md): aporta la base de repositori, documentació i traçabilitat sobre la qual s'executa este repte.
- [Seqüenciació general](../01_programacio_modul/seqüenciacio_general.md): recorda que el Repte 2 hereta el Repte 1 i prepara explícitament el Repte 3 dins del producte únic del curs.

## Paper de la IA
La IA es pot usar com a assistent de treball per:
- proposar esquelets de fluxos de registre, login i control de sessió
- suggerir matrius de validació i casos de prova
- ajudar a interpretar errors de formulari, sessió o control d'accés
- revisar claredat de missatges d'error i completitud de comprovacions

Condicions d'ús:
- l'equip ha de comprendre i poder explicar qualsevol fragment proposat per IA
- tota aportació s'ha de validar amb execució real, proves i revisió de codi
- el resultat final ha de ser coherent amb el context del producte i amb el nivell del repte
- si hi ha ús de IA, ha d'existir traça verificable de què s'ha demanat, què s'ha acceptat i com s'ha comprovat

## Evidències d'aprenentatge
Evidències mínimes i autèntiques del repte:
- issue principal amb microtasques i estat de resolució
- seqüència de commits que mostre evolució real del mòdul d'usuaris i sessions
- demostració funcional de registre, login, logout i accés a una funcionalitat real protegida
- evidència d'una regla de rol o restricció de negoci aplicada sobre el flux principal
- evidència de validacions d'entrada i d'errors controlats
- proves mínimes executades o registre de verificació funcional de casos clau
- documentació tècnica actualitzada del mòdul
- AI log o registre equivalent quan s'haja utilitzat IA

## Instruments d'avaluació
- [Rúbrica base de reptes](../03_avaluacio/rubrica_base_reptes.md) adaptada al pes principal de RA2, RA3 i RA4
- [Checklist de revisió de repositori](../03_avaluacio/checklist_revisio_repo.md) per comprovar traçabilitat, qualitat mínima i coherència documental
- checklist específica de funcionalitat d'autenticació, control de sessió i validació
- revisió de proves mínimes i del registre d'incidències o debugging
- defensa tècnica breu centrada en decisions, errors trobats, verificació i preparació per al Repte 3

## Riscos d'ús inadequat de la IA
- copiar fluxos d'autenticació sense entendre què guarda la sessió, com es valida l'entrada o què protegix una ruta
- assumir com a correctes respostes genèriques de IA que confonen sessió, cookie, token o autorització
- acceptar validacions incompletes perquè "sembla que funciona" en el cas feliç
- fabricar proves o captures que no corresponen al comportament real del repositori
- no saber justificar per què una solució és suficient per al Repte 2 però encara necessita refactorització al Repte 3

## Mesures de verificació
- execució en directe de casos positius i negatius: registre correcte, registre invàlid, login correcte, login incorrecte, accés autoritzat i accés denegat
- comprovació de l'estat de sessió abans i després del logout
- demostració del flux funcional complet del domini: autenticació, operació real, restricció o rol i error quan no es complix la condició
- revisió de coherència entre validacions definides, dades acceptades i errors retornats
- contrast entre AI log, commits i resultat funcional observat
- preguntes tècniques breus per comprovar autoria, comprensió i capacitat de mantindre el codi
- revisió final dels punts de deute tècnic que es traslladen explícitament al Repte 3

## Entorn professional
Marc mínim de treball del repte:
- repositori Git/GitHub amb issues, commits i branques de treball coherents
- entorn local executable i reproduïble per a qualsevol membre de l'equip
- eina de prova funcional del backend segons l'stack triat
- registre d'incidències de validació, autenticació i sessió
- documentació orientada a onboarding i continuïtat del projecte
- dinàmica de treball per reptes, amb entrega basada en producte funcional i evidències autèntiques

## Definition of done del repte
El Repte 2 es considera completat quan:
- existix un flux funcional complet d'usuari amb registre o alta, login, logout i comprovació de sessió
- almenys una operació del producte queda protegida per autenticació i forma part d'un cas d'ús real del domini
- existix com a mínim una regla de rol, permís o restricció de negoci aplicada i verificable
- la validació d'entrades i el tractament d'errors són coherents, visibles i verificables
- el repositori aporta evidències autèntiques de treball: issues, commits, proves i documentació
- l'ús de IA, si n'hi ha, queda registrat i validat
- el mòdul resultant encaixa amb el [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md) i deixa preparada la migració del [Repte 3. Migració a MVC i persistència segura](repte_03_mvc_i_persistencia.md) sense haver de reconstruir la funcionalitat des de zero
- un mòdul limitat a login, registre o logout sense una funcionalitat de negoci autenticada no es considera suficient
