# Repte 5. Integració híbrida, automatització i manteniment

## Finalitat
Tancar el producte backend del curs demostrant que ja no és només un servei funcional, sinó una base integrable, automatitzable i mantenible en un entorn professional realista.

Este repte culmina la seqüència iniciada al Repte 1 i reutilitza directament l'API publicada en el [Repte 4. Publicació i consum d'API](repte_04_api_i_consum.md) per integrar-la amb serveis externs, fluxos híbrids i automatitzacions. Quan siga pertinent, la integració es pot materialitzar amb `n8n` o amb una eina equivalent, sempre que el valor tècnic i docent siga verificable.

## Relació amb resultats d'aprenentatge
- **RA9 (principal):** integrar serveis externs i automatitzacions en una solució backend híbrida orientada a un cas d'ús real.
- **RA7 (reforç):** reutilitzar l'API pròpia com a contracte estable dins d'un escenari d'integració.
- **RA8 (reforç):** aplicar qualitat, debugging, verificació, seguretat bàsica i criteri de manteniment sobre el flux integrat.

Contribució curricular esperada:
- demostrar que l'API del producte es pot consumir dins d'un procés híbrid complet
- connectar backend, servei extern i automatització amb un flux verificable de negoci
- evidenciar manteniment real: incidències, traçabilitat, punts de fallada i correccions
- tancar el producte evolutiu del curs amb una entrega professional defensable

## Context professional
En un context real, un backend no acaba quan publica la seua API. El valor operatiu apareix quan eixa API s'integra amb altres serveis, processos interns, notificacions, automatitzacions o eines d'orquestració.

Després del Repte 4, l'equip ja disposa d'un servei documentat i consumible. El pas següent és demostrar que pot:
- connectar-se amb un sistema extern o una eina d'automatització
- gestionar intercanvi de dades i possibles errors d'integració
- mantindre traçabilitat del flux i capacitat de revisió
- prendre decisions de manteniment amb criteri, no només fer una demo puntual

## Problema o encàrrec inicial
**Encàrrec:** "Integreu el backend del curs en un flux híbrid realista que combine l'API pròpia amb una automatització o servei extern, documenteu el procés i entregueu evidències que la solució es pot provar, mantindre i defensar tècnicament."

Restriccions del repte:
- la integració ha de nàixer de l'API publicada al Repte 4, no d'un prototip desconnectat
- no es tracta de fer una automatització ornamental, sinó un flux amb valor funcional clar
- la integració amb `n8n` és recomanable quan aporte valor docent i verificable, però es pot usar una alternativa equivalent si està justificada
- cal demostrar què passa quan el flux funciona i què passa quan falla
- l'equip ha de documentar decisions de manteniment, incidències i punts de risc
- la IA es pot usar com a suport, però qualsevol proposta s'ha de validar amb execució real i revisió tècnica

## Producte final
El lliurable mínim del Repte 5 ha d'incloure:
- un flux híbrid funcional que reuse l'API del producte backend
- integració amb `n8n` o equivalent quan siga pertinent, o amb un servei extern justificat
- automatització o orquestració d'un cas de negoci recognoscible
- tractament bàsic d'errors, reintents o control de fallada segons el cas triat
- evidència de consum real del backend dins del flux integrat
- documentació tècnica del procés, del recorregut de dades i dels punts crítics
- registre de proves, incidències i ajustos de manteniment
- proposta mínima de continuïtat o millora del sistema integrat

## Compatibilitat amb el producte base i itineraris
Este repte s'alinea amb [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md), perquè completa dues dimensions obligatòries del producte evolutiu:
- **integracions amb serveis externs o fluxos híbrids**
- **manteniment evolutiu (correccions, millores, regressions i traçabilitat)**

A més:
- reutilitza l'API publicada i consumida al [Repte 4. Publicació i consum d'API](repte_04_api_i_consum.md)
- posa a prova la robustesa real del backend més enllà del seu ús intern
- és compatible amb els itineraris **PHP + Laravel**, **Node.js + Express o Nest** i **Python + FastAPI**
- permet usar `n8n` o una eina equivalent d'orquestració, automatització o integració si s'ajusta millor al cas d'ús
- manté el criteri del repositori: canvien les eines concretes, però no els objectius, les evidències ni la verificació exigida

## Seqüència de treball
1. **Seleccionar el cas d'integració**
   Definir quin procés de negoci del producte es vol automatitzar o connectar amb un servei extern.
2. **Dissenyar el flux híbrid**
   Identificar productor, consumidor, automatització, dades d'entrada i eixides esperades.
3. **Preparar l'API i els punts de connexió**
   Verificar quins endpoints del Repte 4 intervenen, quina autenticació requereixen i quins límits o errors poden aparéixer.
4. **Implementar l'automatització o orquestració**
   Construir el flux amb `n8n` o equivalent i connectar-lo amb el backend i, si escau, amb un servei extern.
5. **Validar, depurar i mantindre**
   Provar camins correctes, fallades, dades incorrectes i problemes de sincronització o format.
6. **Documentar i defensar**
   Registrar decisions, incidències, proves, limitacions i millores futures del sistema integrat.

## Activitats o microtasques
- crear la issue principal del Repte 5 i descompondre-la en microtasques d'integració i manteniment
- seleccionar un cas d'ús de negoci que tinga sentit integrar o automatitzar
- mapar dades d'entrada, transformacions i resultats esperats del flux
- revisar quins endpoints del Repte 4 participen en la integració
- definir com es gestionaran autenticació, secrets, errors i reintents
- implementar el workflow en `n8n` o eina equivalent quan siga pertinent
- connectar el flux amb un servei extern, webhook o procés automatitzat justificat
- provar camins correctes, errors d'API, errors externs i casos de dades problemàtiques
- documentar troubleshooting, incidències i decisions de manteniment
- preparar una demostració tècnica centrada en valor real, no només en l'efecte visual del flux

## Materials i apunts associats
- [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md): fixa que el producte ha de cobrir integracions externes o fluxos híbrids i mantindre traçabilitat de millores i correccions.
- [Mapa de materials actuals -> transformació operativa](../04_materials/mapa_materials_actuals.md): situa el **Bloc 7. Webs híbrides** com a nucli del repte, amb suport dels **Blocs 6a i 6b. APIs** i del **Bloc 5. Seguretat i reactivitat**.
- [Repte 4. Publicació i consum d'API](repte_04_api_i_consum.md): aporta el contracte API que ara s'integra dins d'un procés híbrid real.
- [Integració de n8n](../05_projectes_tecnics/integracio_n8n.md): proposa la ubicació recomanada del cas d'ús i exemples de workflow verificable.
- [Integració API](../05_projectes_tecnics/integracio_api.md): recorda el paper de l'exposició i el consum d'APIs dins del mòdul.
- [Seqüenciació general](../01_programacio_modul/seqüenciacio_general.md): fixa el Repte 5 com a tancament del producte evolutiu amb automatització i serveis externs.

## Paper de la IA
La IA es pot usar com a assistent de treball per:
- proposar escenaris d'integració plausibles i seqüències d'automatització
- ajudar a mapar payloads, transformacions i punts de fallada
- suggerir estratègies de reintents, validació i observabilitat bàsica
- donar suport en debugging de desacoblaments entre API, workflow i servei extern
- revisar documentació tècnica del flux i dels incidents detectats

Condicions d'ús:
- l'equip ha de comprendre i poder explicar el flux final de punta a punta
- tota proposta de IA s'ha de validar amb execució real del backend i del procés integrat
- qualsevol configuració suggerida per IA sobre `n8n` o eines equivalents s'ha de contrastar amb el comportament real del workflow
- si hi ha ús de IA, ha d'existir traça verificable de què s'ha acceptat, què s'ha descartat i com s'ha comprovat

## Evidències d'aprenentatge
Evidències mínimes i autèntiques del repte:
- issue principal amb microtasques i estat de resolució
- seqüència de commits que mostre la construcció i l'ajust del flux híbrid
- workflow exportat o artefacte equivalent de l'automatització
- evidència d'integració entre API pròpia i servei extern o eina d'orquestració
- proves registrades de casos correctes i de fallada
- documentació tècnica del flux, dels punts crítics i del manteniment aplicat
- registre d'incidències, debugging i correccions
- AI log o registre equivalent quan s'haja utilitzat IA

## Instruments d'avaluació
- [Rúbrica base de reptes](../03_avaluacio/rubrica_base_reptes.md) adaptada al pes principal de RA9 i al reforç de RA7 i RA8
- checklist específica d'integració híbrida, automatització i manteniment
- revisió del workflow, webhook o artefacte equivalent i de la seua connexió amb l'API del curs
- revisió de proves de flux, errors i capacitat de recuperació o diagnòstic
- demostració funcional del procés complet, des de l'entrada fins al resultat integrat
- defensa tècnica breu centrada en decisions, riscos, mantenibilitat i valor real de la integració

## Riscos d'ús inadequat de la IA
- generar fluxos d'automatització que semblen plausibles però no corresponen al comportament real de l'API
- copiar configuracions de `n8n` o d'altres eines sense entendre credencials, webhooks, transformacions o errors
- simular integracions sense demostrar un recorregut complet de dades
- presentar un workflow visualment atractiu però tècnicament fràgil o no mantingut
- no saber justificar per què s'ha triat una eina o un servei extern concret

## Mesures de verificació
- execució en directe del flux híbrid complet amb dades reals o de prova controlada
- comprovació de consum efectiu de l'API del Repte 4 dins de l'automatització
- validació de camins correctes, errors d'API, errors externs i respostes inesperades
- contrast entre workflow exportat, documentació i comportament real observat
- revisió de commits i registre d'incidències per comprovar manteniment real
- contrast entre AI log, configuració final i defensa tècnica
- preguntes tècniques breus sobre payloads, punts de fallada, secrets i decisions d'orquestració

## Entorn professional
Marc mínim de treball del repte:
- repositori Git/GitHub amb issues, commits i branques de treball coherents
- entorn local o de prova reproduïble per executar backend, API i automatització
- eina d'orquestració com `n8n` o equivalent quan el cas d'ús ho requerisca
- documentació tècnica orientada a onboarding, manteniment i recuperació d'incidències
- registre d'incidents, errors d'integració i correccions aplicades
- dinàmica de treball per reptes amb evidències autèntiques, verificables i defensables

## Definition of done del repte
El Repte 5 es considera completat quan:
- existix una integració híbrida funcional basada en l'API del producte del curs
- el flux automatitzat aporta un cas d'ús recognoscible i justificable
- la integració amb `n8n` o equivalent, quan s'usa, està documentada i verificada
- hi ha evidència de proves sobre casos correctes i sobre fallades rellevants del procés
- el repositori aporta evidències autèntiques de treball: issues, commits, artefactes d'integració, proves i documentació
- l'ús de IA, si n'hi ha, queda registrat i validat
- el resultat final encaixa amb el [Projecte backend base del curs](../05_projectes_tecnics/projecte_base_backend.md) i tanca el producte evolutiu del mòdul amb criteri professional de manteniment i integració
