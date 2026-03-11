# Repte 1. Kickoff tècnic d’un servei web backend

## Finalitat
Iniciar un servei web backend en condicions professionals reals i deixar una base tècnica robusta per al conjunt del curs. Este repte fixa la manera de treballar de l’equip (organització, traçabilitat, documentació i validació) i garanteix que el projecte arranca amb criteri tècnic defensable.

## Relació amb resultats d’aprenentatge
- **RA1 (principal):** selecció d’arquitectura, configuració d’entorn i justificació de decisions tècniques inicials.
- **RA5 (inici):** primera estructuració del projecte amb criteris de mantenibilitat (organització de carpetes, convencions de codi i pauta de creixement).

Contribució esperada del repte:
- l’alumnat demostra que pot arrencar un projecte backend des de zero amb criteri professional
- la base creada és reutilitzable i escalable per als reptes 2-5

## Context professional
Un equip backend rep l’encàrrec de posar en marxa un nou servei. No es demana encara funcionalitat de negoci completa, sinó preparar una base fiable perquè el desenvolupament posterior siga ràpid, segur i mantenible.

El client intern vol garanties mínimes abans de continuar:
- que el projecte arranca en local de manera reproductible
- que la decisió arquitectònica està argumentada
- que el repositori i la documentació permeten treball en equip

## Problema o encàrrec inicial
**Encàrrec:** “Deixeu operativa la primera versió tècnica del servei backend i entregueu evidències que permeten començar el desenvolupament funcional en el repte següent.”

Restriccions de l’encàrrec:
- no prioritzar quantitat de codi sobre qualitat de base
- documentar decisions des del primer dia
- establir un flux Git/GitHub clar (issues, commits, branques)
- incorporar IA com a suport, però sempre amb verificació tècnica

## Producte final
El lliurable del repte ha d’incloure, com a mínim:
- repositori inicial funcional amb estructura coherent
- README tècnic de posada en marxa (instal·lació, execució i comprovació)
- ADR curt amb la decisió d’arquitectura principal i alternatives descartades
- primera validació tècnica executada i registrada
- historial de treball traçable (issues i commits significatius)

## Seqüència de treball
1. **Anàlisi inicial del context**
   - entendre requisits mínims, restriccions i objectiu del kickoff.
2. **Decisió tècnica inicial**
   - comparar 2-3 alternatives d’stack o enfocament i triar-ne una.
3. **Arrencada del projecte**
   - inicialitzar repositori, estructura base i configuració d’entorn.
4. **Definició de normes de treball**
   - establir convencions de branques, missatges de commit i ús d’issues.
5. **Validació tècnica mínima**
   - executar el servei i comprovar resposta esperada.
6. **Documentació i tancament**
   - completar README, ADR i síntesi de decisions per a transició a Repte 2.

## Activitats o microtasques
- crear una issue mare de kickoff i descompondre-la en microtasques
- preparar `README` amb prerequisits, passos d’arrancada i troubleshooting bàsic
- definir estructura de carpetes i convencions de nom
- redactar ADR (context, decisió, alternatives, conseqüències)
- fer primera execució verificable del servei (amb captures/logs o registre d’eixida)
- documentar incidències inicials i com s’han resolt
- preparar mini defensa tècnica final (5-7 minuts)

## Materials i apunts associats
- bloc 1 d’arquitectures web (criteris de tria i justificació)
- introducció a entorn de treball backend (configuració i eines)
- guia Git/GitHub del curs (issues, branques, commits, revisió)
- orientacions de documentació tècnica (README i ADR)

## Paper de la IA
La IA s’empra com a eina de suport per:
- explorar alternatives d’arquitectura i trade-offs
- proposar esquelets inicials de projecte
- revisar claredat i completesa del README
- suggerir llistes de comprovació de validació tècnica

Criteri d’ús:
- la IA orienta, però no decideix
- tota proposta s’ha d’adaptar al context del repte
- qualsevol contribució de la IA s’ha de poder explicar i verificar

## Evidències d’aprenentatge
Evidències mínimes obligatòries:
- issue de kickoff amb microtasques i estat de resolució
- seqüència de commits amb missatges que reflectisquen decisions i evolució
- README tècnic executable per tercers
- ADR de decisió arquitectònica
- registre de validació tècnica inicial
- AI log quan hi haja ús de IA

## Instruments d’avaluació
- rúbrica base de reptes adaptada al Repte 1
- checklist de revisió de repositori (traçabilitat i qualitat mínima)
- revisió tècnica de README i ADR
- defensa tècnica breu centrada en decisions, verificació i continuïtat

## Riscos d’ús inadequat de la IA
- copiar configuracions sense comprendre impacte tècnic
- acceptar documentació generada sense comprovar executable real
- generar una arquitectura incoherent amb el context del mòdul
- no poder justificar per què s’ha triat una alternativa concreta

## Mesures de verificació
- prova en directe d’arrancada del projecte seguint únicament el README
- preguntes tècniques sobre alternatives descartades a l’ADR
- contrast entre AI log, commits i resultat efectiu del repositori
- microcanvis en viu per comprovar autoria i domini tècnic
- revisió de coherència entre estructura, documentació i validació reportada

## Entorn professional
Marc mínim de treball professional del repte:
- Git/GitHub com a entorn central de col·laboració
- gestió del treball amb issues i tancament traçable de tasques
- branques de treball i integració controlada
- debugging inicial de configuració/arrancada
- documentació tècnica orientada a onboarding de l’equip

## Definition of done del repte
El Repte 1 queda completat quan es compleixen **totes** les condicions següents:
- el servei arranca en local seguint el README, sense passos ocults
- existeix ADR amb decisió arquitectònica clara i alternatives justificades
- el repositori mostra traçabilitat real (issues + commits coherents)
- s’ha registrat una validació tècnica mínima amb resultat verificable
- l’alumnat pot defensar oralment què ha fet, per què i com prepara el pas al Repte 2
