# Repte 1. Kickoff funcional d’un servei web backend

## Finalitat
Iniciar un servei web backend en condicions professionals reals i deixar una base tècnica robusta per al conjunt del curs. Este repte fixa la manera de treballar de l’equip (organització, traçabilitat, documentació i validació) i obliga a entregar ja una primera peça funcional real del producte.

El Repte 1 no es considera superat només per triar tecnologia, instal·lar un framework o deixar un esquelet executable. Ha d’existir una primera entrada funcional del producte, per exemple una landing page o equivalent, un formulari útil per arreplegar dades, una validació mínima al servidor i un primer registre o persistència bàsica de la informació.

## Relació amb resultats d’aprenentatge
- **RA1 (principal):** selecció d’arquitectura, configuració d’entorn i justificació de decisions tècniques inicials.
- **RA5 (inici):** primera estructuració del projecte amb criteris de mantenibilitat (organització de carpetes, convencions de codi i pauta de creixement).

Contribució esperada del repte:
- l’alumnat demostra que pot arrencar un projecte backend des de zero amb criteri professional
- la base creada és reutilitzable i escalable per als reptes 2-5

## Context professional
Un equip backend rep l’encàrrec de posar en marxa un nou servei. No es demana encara el producte complet, però sí una base fiable que ja permeta ensenyar una primera interacció real amb el sistema i deixar rastre tècnic verificable del seu comportament.

El client intern vol garanties mínimes abans de continuar:
- que el projecte arranca en local de manera reproductible
- que la decisió arquitectònica està argumentada
- que el repositori i la documentació permeten treball en equip
- que ja existix una primera peça funcional del producte i no només un esquelet tècnic buit

## Problema o encàrrec inicial
**Encàrrec:** “Deixeu operativa la primera versió funcional del servei backend i entregueu evidències que permeten començar el desenvolupament del producte real en el repte següent.”

Restriccions de l’encàrrec:
- no prioritzar quantitat de codi sobre qualitat de base
- documentar decisions des del primer dia
- establir un flux Git/GitHub clar (issues, commits, branques)
- incorporar IA com a suport, però sempre amb verificació tècnica
- triar tecnologia o muntar un esquelet de framework no és suficient
- ha d’existir una primera funcionalitat d’entrada al producte: landing page o equivalent, formulari i registre mínim de dades

## Producte final
El lliurable del repte ha d’incloure, com a mínim:
- repositori inicial funcional amb estructura coherent
- decisió tecnològica justificada i alineada amb el domini triat
- landing page inicial o equivalent d’entrada al producte servida pel backend
- formulari funcional per arreplegar una primera dada útil del domini
- validació mínima al servidor sobre eixe formulari o petició inicial
- registre o persistència mínima de la informació arreplegada, encara que siga bàsica
- README tècnic de posada en marxa (instal·lació, execució i comprovació)
- ADR curt amb la decisió d’arquitectura principal i alternatives descartades
- primera validació tècnica executada i registrada
- historial de treball traçable (issues i commits significatius)

## Seqüència de treball
1. **Anàlisi inicial del context**
   - entendre requisits mínims, restriccions i objectiu del kickoff.
2. **Decisió tècnica inicial**
   - comparar 2-3 alternatives d’stack o enfocament i triar-ne una.
3. **Definició del primer cas d’ús mínim**
   - concretar quina primera interacció real del producte es demostrarà en este repte.
4. **Arrencada del projecte**
   - inicialitzar repositori, estructura base i configuració d’entorn.
5. **Definició de normes de treball**
   - establir convencions de branques, missatges de commit i ús d’issues.
6. **Primera funcionalitat real**
   - implementar landing page o equivalent, formulari funcional, validació i registre mínim de dades.
7. **Validació tècnica mínima**
   - executar el servei, provar el flux inicial i comprovar resposta esperada.
8. **Documentació i tancament**
   - completar README, ADR i síntesi de decisions per a transició a Repte 2.

## Activitats o microtasques
- crear una issue mare de kickoff i descompondre-la en microtasques
- definir quin és el primer flux mínim del producte que s’executarà en este repte
- preparar `README` amb prerequisits, passos d’arrancada i troubleshooting bàsic
- definir estructura de carpetes i convencions de nom
- redactar ADR (context, decisió, alternatives, conseqüències)
- construir una landing page o equivalent d’entrada al producte
- implementar un formulari funcional per arreplegar una primera dada del domini
- validar al servidor la informació rebuda i registrar-la o persistir-la de forma mínima
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
- evidència funcional d’una landing page o equivalent i del primer formulari executable
- registre o persistència mínima de la informació enviada en eixe primer flux
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
- prova en directe del primer flux funcional: accés a la landing page o equivalent, enviament de formulari, validació i registre de la dada
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
- existeix una primera peça funcional del producte, no només un esquelet tècnic
- hi ha una landing page o equivalent d’entrada, un formulari funcional i una validació mínima al servidor
- la informació del primer flux queda registrada o persistida de manera bàsica i verificable
- existeix ADR amb decisió arquitectònica clara i alternatives justificades
- el repositori mostra traçabilitat real (issues + commits coherents)
- s’ha registrat una validació tècnica mínima amb resultat verificable
- l’alumnat pot defensar oralment què ha fet, per què i com prepara el pas al Repte 2
- triar tecnologia o muntar un esquelet buit no es considera suficient per donar el repte per superat
