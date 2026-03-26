# Repte 4. Publicació i consum d'API

## Finalitat

Convertir el backend ja funcional i estructurat dels reptes anteriors en un servei publicable i consumible, amb endpoints documentats, validació d'entrades, tractament coherent d'errors i proves de consum reals.

Este repte és el pas de "backend usable per l'equip" a "backend integrable per tercers". A partir de la base construïda en el [Repte 3. Migració a MVC i persistència segura](repte_03_mvc_i_persistencia.md), l'alumnat ha de publicar una primera API clara, verificable i preparada per a la integració híbrida del [Repte 5. Integració híbrida, automatització i manteniment](repte_05_integracio_hibrida_n8n.md).

No és un repte de tècnica aïllada. Obrir rutes, generar `Swagger` o retornar JSON no és suficient si l'API no exposa casos d'ús reals del producte amb contracte clar, consum verificat i defensa tècnica del flux complet.

## Relació amb resultats d'aprenentatge

- **RA7 (principal):** dissenyar, publicar i consumir APIs documentades sobre un producte backend real.
- **RA6 (reforç):** mantindre coherència entre endpoints, model de dades, persistència i accés segur a la informació.
- **RA8 (reforç):** aplicar validació, tractament d'errors, debugging, proves i criteris mínims de qualitat sobre l'API publicada.

Contribució curricular esperada:

- exposar casos d'ús prioritaris del producte com a endpoints amb contracte clar
- documentar l'API perquè puga ser utilitzada per altres membres de l'equip o per serveis externs
- demostrar consum real de l'API amb col·lecció de proves, client o integració controlada
- deixar la capa de servei preparada per al Repte 5, on l'API passarà a formar part d'un escenari d'integració híbrida

## Context professional

Després del Repte 3, l'equip ja disposa d'un backend amb arquitectura més mantenible, persistència coherent i qualitat tècnica mínima. Però encara falta un pas clau perquè el producte tinga valor professional complet: definir una interfície externa estable i consumible.

En un entorn real, publicar API implica molt més que obrir rutes:

- cal definir contractes de petició i resposta
- cal documentar com s'autentica, què retorna i com gestiona errors
- cal comprovar que un consumidor extern pot usar l'API sense dependre del coneixement intern del codi
- cal deixar una base fiable per a futures integracions, automatitzacions i manteniment
- cal assegurar que allò que es publica correspon a funcionalitat real del producte i no a endpoints ornamentals o de demostració

## Problema o encàrrec inicial

**Encàrrec:** "Publiqueu una primera versió usable de l'API del producte backend del curs, documenteu-ne els endpoints prioritaris, verifiqueu-ne el consum i entregueu evidències que el contracte és clar, funcional i mantingut amb criteri tècnic."

Restriccions del repte:

- l'API ha d'eixir del producte real del curs, no d'un mock desconnectat
- no es tracta de publicar tots els casos d'ús, sinó un conjunt prioritari i ben resolt
- la documentació ha de correspondre exactament amb el comportament real de l'endpoint
- les respostes, errors i codis d'estat han de ser coherents i justificables
- el consum s'ha de demostrar amb execució real i no només amb captures o descripcions
- la IA es pot usar com a suport, però tota proposta ha d'estar validada amb proves i revisió tècnica
- obrir rutes sense valor funcional o documentar una API que no representa un cas d'ús real no es considera suficient

## Producte final

El lliurable mínim del Repte 4 ha d'incloure:

- una API funcional que expose operacions clau i no trivials del producte backend
- definició clara d'endpoints, mètodes, paràmetres, autenticació i estructures de resposta
- tractament coherent d'errors, validacions i codis d'estat
- documentació tècnica d'API usable per tercers
- col·lecció de proves d'endpoint o equivalent
- una evidència real de consum de l'API des d'un client, script o servei auxiliar sobre un flux funcional complet
- proves mínimes o verificacions registrades dels fluxos principals i dels casos d'error
- documentació actualitzada de posada en marxa, prova i consum

## Compatibilitat amb el producte base i itineraris

Este repte s'alinea directament amb [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md), perquè consolida dos components obligatoris del producte evolutiu:

- **API publicada i consumible**
- **documentació tècnica operativa (README, decisions i contractes API)**

A més:

- reutilitza la base arquitectònica i de persistència consolidada al Repte 3
- transforma funcionalitats internes del producte en una interfície externa clara i versionable
- deixa la infraestructura conceptual i tècnica preparada per al [Repte 5. Integració híbrida, automatització i manteniment](repte_05_integracio_hibrida_n8n.md), on l'API serà consumida en un flux més ampli
- és compatible amb els itineraris **PHP + Laravel**, **Node.js + Express o Nest** i **Python + FastAPI**
- manté equivalència docent entre stacks: canvia la implementació concreta, no els objectius ni les evidències exigides

## Seqüència de treball

1. **Seleccionar casos d'ús publicables**
   Decidir quines operacions del producte passen a API i quin valor tenen per a consum intern o extern.

2. **Definir el contracte d'API**
   Concretar rutes, verbs HTTP, autenticació, camps d'entrada, estructura de resposta, errors i criteri de versionat si correspon.

3. **Implementar endpoints i serialització**
   Publicar els endpoints prioritaris i assegurar coherència entre el model intern i la resposta exposada.

4. **Aplicar validació, errors i control d'accés**
   Gestionar dades invàlides, credencials, permisos i casos excepcionals amb comportament previsible.

5. **Documentar i provar el consum**
   Preparar documentació d'API, col·leccions de prova i una evidència real de consum sobre un cas d'ús funcional complet.

6. **Verificar i preparar la transició**
   Comprovar que la documentació reflectix la realitat i deixar l'API preparada per a integració al Repte 5.

## Activitats o microtasques

- crear la issue principal del Repte 4 i dividir-la en microtasques de publicació i consum
- seleccionar endpoints prioritaris segons el domini del producte
- definir el contracte mínim de petició/resposta per a cada endpoint
- establir convencions de codis d'estat i errors d'API
- implementar validació d'entrada i serialització de resposta
- protegir endpoints que requerisquen autenticació o control d'accés
- preparar documentació d'API en format usable per l'equip
- construir una col·lecció de proves amb eines d'API o equivalent
- demostrar el consum real amb un client, script o servei extern controlat sobre una funcionalitat real del producte
- revisar discrepàncies entre documentació, resposta real i necessitats del futur Repte 5

## Materials i apunts associats

- [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md): fixa que el producte del curs ha de tindre API publicada i consumible, documentació tècnica operativa i capacitat d'integració.
- [Mapa de materials actuals -> transformació operativa](../04_materials/mapa_materials_actuals.md): situa els **Blocs 6a i 6b. APIs** com a nucli del repte, amb reforç del **Bloc 5. Seguretat i reactivitat** i suport dels **Blocs 3 i 4** per coherència de model i persistència.
- [Repte 3. Migració a MVC i persistència segura](repte_03_mvc_i_persistencia.md): aporta l'estructura mantenible i la persistència segura sobre les quals es publiquen els endpoints.
- [Repte 5. Integració híbrida, automatització i manteniment](repte_05_integracio_hibrida_n8n.md): serà el següent pas, on l'API publicada ací s'integrarà amb serveis externs o automatitzacions.
- [Seqüenciació general](../01_programacio_modul/seqüenciacio_general.md): reforça que el Repte 4 exposa i consumix funcionalitats procedents del model consolidat al Repte 3 i prepara el pas al Repte 5.

## Paper de la IA

La IA es pot usar com a assistent de treball per:

- proposar esborranys de contracte API o d'especificació OpenAPI
- suggerir col·leccions de prova, casos límit i matrius d'errors
- ajudar a detectar incoherències entre endpoint, documentació i consumidor
- generar esquelets inicials de client de consum o scripts de prova
- donar suport en debugging de respostes inesperades o desacoblaments entre productor i consumidor

Condicions d'ús:

- l'equip ha de comprendre i poder justificar el contracte final que publica
- tota aportació de IA s'ha de validar amb execució real d'endpoints i consum
- la documentació generada o revisada amb IA s'ha de contrastar amb el comportament real del backend
- si hi ha ús de IA, ha d'existir traça verificable del procés i de la verificació posterior

## Evidències d'aprenentatge

Evidències mínimes i autèntiques del repte:

- issue principal amb microtasques i estat de resolució
- seqüència de commits que mostre l'evolució de la publicació i el consum d'API
- endpoints operatius sobre el producte real del curs i associats a casos d'ús recognoscibles
- documentació tècnica d'API alineada amb el comportament real
- col·lecció de proves API, client de consum o evidència equivalent d'ús extern
- proves o verificacions registrades de casos positius, errors i validacions
- documentació actualitzada de posada en marxa i ús de l'API
- AI log o registre equivalent quan s'haja utilitzat IA

## Instruments d'avaluació

- [Rúbrica base de reptes](../03_avaluacio/rubrica_base_reptes.md) adaptada al pes principal de RA7 i al reforç de RA6 i RA8
- checklist específica de contracte API, documentació, codis d'estat i errors
- revisió de col·leccions de prova, scripts de consum o evidències equivalents
- revisió de validació d'entrada, control d'accés i coherència de resposta
- demostració funcional del productor i del consumidor sobre el mateix contracte
- defensa tècnica breu centrada en decisions de disseny, trade-offs i preparació per al Repte 5

## Riscos d'ús inadequat de la IA

- acceptar contractes d'API suggerits per IA que no corresponen al domini ni al model real del producte
- documentar endpoints inexistents o amb respostes diferents de les implementades
- copiar codis d'estat o estructures d'error sense entendre quan aplicar-los
- generar un client de consum aparentment funcional però no connectat amb l'API real
- confondre una demo de prova puntual amb una verificació real del contracte publicat

## Mesures de verificació

- execució en directe d'endpoints prioritaris amb casos correctes i incorrectes sobre un flux real del producte
- contrast entre documentació d'API i resposta real del backend
- comprovació de validació d'entrada, errors i codis d'estat en diversos escenaris
- prova real del consumidor contra l'API publicada o l'entorn de treball definit
- revisió dirigida de commits i artefactes per comprovar evolució real del repte
- contrast entre AI log, documentació, proves i resultat funcional
- preguntes tècniques breus sobre decisions de contracte, serialització i consum

## Entorn professional

Marc mínim de treball del repte:

- repositori Git/GitHub amb issues, commits i branques de treball coherents
- entorn local o de prova reproduïble per publicar i consumir l'API
- eina de prova d'API com Postman, Insomnia, curl o equivalent segons l'itinerari
- documentació tècnica orientada a onboarding i ús per tercers
- registre d'incidències de contracte, errors, validació i consum
- dinàmica de treball per reptes amb evidències autèntiques i verificables

## Definition of done del repte

El Repte 4 es considera completat quan:

- existixen endpoints prioritaris publicats sobre el producte real del curs i lligats a casos d'ús no trivials
- la documentació d'API descriu correctament peticions, respostes, errors i condicions d'ús
- hi ha validació d'entrada, tractament coherent d'errors i codis d'estat justificables
- el consum de l'API queda demostrat amb una evidència real i reproduïble
- el repositori aporta evidències autèntiques de treball: issues, commits, proves i documentació
- l'ús de IA, si n'hi ha, queda registrat i validat
- l'API resultant encaixa amb el [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md) i deixa preparada la base tècnica per al [Repte 5. Integració híbrida, automatització i manteniment](repte_05_integracio_hibrida_n8n.md)
- una API formada per rutes soltes, documentació ornamental o consum fictici no es considera suficient
