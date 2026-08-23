# Matriu de coherència curricular del mòdul DWES

## Classificació documental

Este és un **document canònic**. La seua funció és relacionar resultats d'aprenentatge, reptes, projecte base, evidències, instruments d'avaluació, verificació d'aprenentatge real i paper de l'ús assistit per IA.

No substituïx els documents canònics de [visió del model](visio-model-dwes.md), [curs executable](curs-executable.md), [avaluació i evidències](03_avaluacio/index.md) o [ús de la IA per a professorat i alumnat](us-ia-professorat-i-alumnat.md). Els articula curricularment.

## Finalitat

Permetre al professorat comprovar, d'un colp d'ull, que:

- el curs cobreix els resultats d'aprenentatge del mòdul `0613`
- cada repte té una funció curricular recognoscible
- el projecte base dona coherència transversal
- les evidències exigides són reals i revisables
- els instruments d'avaluació verifiquen aprenentatge i no només producte aparent
- l'ús assistit per IA queda regulat i no genera un buit metodològic

## Criteri de lectura

- un mateix resultat d'aprenentatge pot aparéixer en diversos reptes
- un repte pot contribuir a diversos resultats d'aprenentatge
- el projecte base actua com a peça transversal de coherència
- la defensa tècnica i la revisió de repositori no són complements decoratius: són mecanismes centrals de verificació
- el criteri complet sobre ús assistit per IA i delegació excessiva depén de [us-ia-professorat-i-alumnat.md](us-ia-professorat-i-alumnat.md)

## Matriu principal

| RA del mòdul `0613` | On es treballa principalment | Evidències exigides | Instrument d'avaluació | Verificació d'aprenentatge real | Paper de la IA | Observacions o límits |
|---|---|---|---|---|---|---|
| **RA1. Arquitectura i tecnologies servidor** | `Repte 1` i [enunciat del projecte base](05_projectes_tecnics/enunciat_projecte_base.md) | comparativa tècnica inicial, explicació del model d'execució client vs servidor en `MP1`, nota tècnica de decisió o justificació tècnica, repositori executable, Docker, README, primera peça funcional | rúbrica del repte, checklist de revisió de repositori, defensa tècnica breu | execució real de l'entorn, justificació del stack, preguntes de transferència sobre què s'executa al client i què al servidor, i microcanvis sobre arrencada | suport acceptable per comparar opcions, resumir documentació i detectar errors inicials | cobertura principal en `R1`; `RA1a` queda explicitat en `MP1` i la sessió 1; `RA5` només queda com a preparació no principal |
| **RA2. Codi executable embegut en llenguatges de marques** | `Repte 2` sobre base comuna en `PHP` | codi embegut executable, variables, operadors, directives, formulari base, resposta generada en servidor | checklist de formulari i recuperació de dades, rúbrica breu de processament bàsic | revisió de codi en context, execució del flux complet, reconstrucció guiada d'una part del processament | suport condicionat quan la IA propose esquelets de formulari o processament | concentrat en `R2`; no convé dissoldre'l dins d'autenticació |
| **RA3. Estructures de programació, formularis i interacció** | `Repte 2` i reforç funcional del projecte base | formulari funcional, recuperació de dades, decisions, arrays, funcions, comparativa abans/després en `MP7`, evidència de lògica aplicada | rúbrica del repte, checklist de flux funcional, revisió de repositori | casos positius i negatius, explicació de la lògica, modificació de condicions o validacions en directe | suport condicionat per a lògica i estructures; alt risc si l'alumne no pot explicar decisions i funcions | `R2` és el nucli; el pas a `R3` no ha de reavaluar `RA3` com a focus principal |
| **RA4. Estat, autenticació, prova i depuració** | `Repte 2` i checkpoints de pas a `R3` | demo d'estat, sessió o cookies, autenticació, cas autoritzat i denegat, registre d'incidències, proves mínimes, documentació i checkpoint tècnic | rúbrica del repte, checklist de verificació, defensa tècnica breu, observació docent | reproducció del login o operació protegida, explicació de l'estat, revisió d'errors i correccions, contrast entre codi i comportament | suport condicionat; zona d'alt risc si la IA resol autenticació o debugging sense comprensió real | `RA4` tanca `R2` i prepara `R3`; la defensa ha de verificar autoria individual |
| **RA5. Separació lògica-presentació, patrons i documentació** | `Repte 3`, [projecte backend base](05_projectes_tecnics/projecte_base_backend.md) i fase final integradora | diagnosi del codi anterior, pla de migració, estructura en framework, abans/després d'un cas d'ús, README, decisions tècniques, backlog de migració | rúbrica del repte, checklist d'arquitectura, revisió de repositori, defensa tècnica | explicació de rutes, controladors, serveis, vistes o equivalents, justificació d'estructura i de migració, revisió del canvi real al repositori | suport condicionat per modelat i refactorització; no acceptable si genera arquitectura opaca no defensable | `RA5` és el nucli de `R3`; es reactiva després en fase final, però no s'ha de reobrir com a refactorització infinita |
| **RA6. Accés a dades, integritat i seguretat** | `Repte 3` com a cobertura principal, `Repte 4` com a suport del servei i `Repte 5` només quan hi ha transformació o persistència externa | migrations, seeders, model de dades, lectura i escriptura reals, validacions, tractament d'errors, proves de regressió, dades reals servides per l'API | rúbrica del repte, checklist de persistència i proves, revisió de repositori, prova guiada | reconstrucció de BBDD, execució de consultes o fluxos amb dades reals, verificació d'errors i integritat mínima | suport condicionat i d'alt risc en model de dades, migracions i consultes | cobertura principal en `R3`; en `R4-R5` només ha d'aparéixer com a suport i no menjar-se `RA7` o el tancament transversal de `R5` |
| **RA7. Serveis web** | `Repte 4` com a cobertura principal, reforç en fase final i suport clar en `R5` quan la integració reutilitza o orquestra serveis | contracte d'API, mapa d'endpoints, primer endpoint funcional, autenticació d'API, consum real, proves del servei, documentació d'API, defensa | rúbrica específica de servei, checklist de consum, revisió de repositori, defensa tècnica breu | consum real del servei, casos autoritzats i denegats, contrast entre contracte, codi i resposta observada | suport condicionat; alt risc de delegació excessiva en contractes, endpoints i documentació ornamental | `RA7` ha de dominar `R4`; en `R5` reforça la integració híbrida, però no substituïx el centre de `RA9` |
| **RA8. Generació dinàmica amb tecnologies/frameworks del servidor** | `Repte 3` com a focus principal, reactivació parcial en el projecte base i eventual projecció en `R5` quan la integració impacta en fluxos renderitzats o respostes del backend | projecte en framework arrancable, almenys un flux **server-rendered**, vistes o plantilles, formulari o interacció processada pel framework, resposta HTML dinàmica, proves mínimes | rúbrica del repte, checklist de fluxos end-to-end, revisió de repositori, observació docent | demostració d'almenys un flux renderitzat en servidor, explicació del circuit petició -> controlador -> vista/resposta -> dades | suport condicionat; risc mitjà si la IA genera vistes o plantilles no compreses | `RA8` està fortament concentrat en `R3`; en `R5` només reapareix si la integració modifica de manera visible el comportament dinàmic del backend |
| **RA9. Aplicacions web híbrides i repositoris heterogenis d'informació** | `Repte 5` com a cobertura principal, amb suport de `R4` quan reutilitza serveis propis i de la fase final quan es verifica estabilitat global | comparativa de fonts externes, connector funcional, mapping, flux híbrid integrat, comparativa font-transformació-resultat, proves del cas positiu i d'error, documentació i defensa | checklist d'integració híbrida, rúbrica del repte, revisió de repositori, prova guiada i mini defensa tècnica | demostració del mapa d'integració, explicació del contracte extern, justificació del valor afegit, microcanvi sobre connector o mapping i contrast entre documentació, `AI log` i comportament observat | suport condicionat; zona d'alt risc de delegació excessiva si l'alumne integra sense entendre ni la font externa ni la transformació | `RA9` ha d'estar al centre de `R5`; `RA7` i `RA8` poden reforçar-lo, però no substituir-lo |

## Cobertura per repte i pel projecte base

| Peça | Funció didàctica | RA principals | Evidències principals | Instruments vinculats |
|---|---|---|---|---|
| [Projecte base](05_projectes_tecnics/enunciat_projecte_base.md) | peça transversal | transversal `RA1-RA9` segons fase | README, arquitectura, decisions, proves, traçabilitat, defensa tècnica | revisió de repositori, rúbriques, defensa tècnica |
| [Repte 1](02_reptes/repte_01_kickoff_backend.md) | iniciació / arranque | `RA1` | model d'execució client vs servidor, comparativa, nota tècnica de decisió, Docker, README, arrencada, primera peça funcional, commit comentat i mini defensa | checklist d'arrencada, revisió de repositori, defensa tècnica breu |
| [Repte 2](02_reptes/repte_02_sessions_i_autenticacio.md) | construcció nuclear | `RA2`, `RA3`, `RA4` | formularis, codi embegut, lògica, estat, autenticació, proves, registre d'errors, checkpoint i comparativa d'ús d'IA quan corresponga | rúbrica del repte, checklist de flux funcional, defensa tècnica breu, revisió de repositori |
| [Repte 3](02_reptes/repte_03_mvc_i_persistencia.md) | consolidació | `RA5`, `RA6`, `RA8` | migració d'un cas d'ús, framework, BBDD, migrations, seeders, flux server-rendered, nota tècnica de decisió breu, README i doble checkpoint | rúbrica de reconstrucció, checklist per checkpoint, revisió de repositori, defensa tècnica |
| [Repte 4](02_reptes/repte_04_api_i_consum.md) | integració | `RA7` amb suport de `RA6` | contracte de servei, endpoints, consum real, autenticació d'API, comparativa contracte-resposta, documentació, proves i mini defensa | rúbrica específica, checklist de consum, revisió de repositori, defensa tècnica breu |
| [Repte 5](02_reptes/repte_05_integracio_hibrida.md) | síntesi amb nucli mínim obligatori de `RA9` i ampliació avançada opcional | `RA9` amb reforç de `RA7`, `RA8` i suport eventual de `RA6` | connector extern, mapping, transformació, integració híbrida, mapa d'integració, comparativa font-transformació-resultat, proves, documentació i defensa | checklist d'integració, rúbrica del repte, revisió de repositori, defensa tècnica, prova guiada |

## Relació amb ús assistit per IA

La matriu no regula de nou l'ús assistit per IA. La lectura és:

- **suport acceptable**: comparatives inicials, resum de documentació, esquelets de treball, ajuda de debugging i revisió de documentació
- **suport condicionat**: arquitectura, model de dades, autenticació, contractes API, integracions externes i proves sobre comportaments crítics
- **zona d'alt risc de delegació excessiva**: quan l'alumne no pot explicar el codi, no sap fer microcanvis, no entén la font externa o no pot relacionar evidència, prova i resultat

El criteri complet depén de [Ús de la IA per a professorat i alumnat](us-ia-professorat-i-alumnat.md).

## Cobertura global del mòdul

- La seqüència `R1-R5` cobreix tots els `RA` del mòdul `0613`.
- `RA1` queda concentrat en `R1`; `RA2-RA4` en `R2`; `RA5-RA6-RA8` en `R3`; `RA7` en `R4`; `RA9` en `R5`, amb reforç puntual de `RA7` i `RA8`.
- El projecte base i la defensa tècnica actuen com a peces transversals de coherència i verificació real.

## Buits o punts febles detectats

- `RA8` depén fortament de `R3` i pot quedar tapat darrere de persistència i framework si no es manté visible el flux **server-rendered**.
- `RA6` té risc de desbordar-se i competir massa amb `RA7` en `R4` o amb el nucli de `RA9` en `R5`.
- La qualitat de la verificació de l'ús assistit per IA depén molt de la constància real en `AI log`, revisió de repositori i defensa tècnica.

## Línies activades en Fase 4

- S'ha fet més explícita la comprovació de `RA8` en instruments i checkpoints de `R3`.
- S'ha reforçat la diferenciació entre suport de `RA6` i focus principal de `RA7` en `R4`, i entre suport de `RA7/RA8` i nucli de `RA9` en `R5`.
- Queda oberta per a una futura fase la possible derivació d'una plantilla encara més curta de verificació d'ús assistit per IA lligada als checkpoints principals del curs.

## Ajust fi aplicat en Fase 4

- `R1` queda fixat com a iniciació / arranque i no carrega exigències de persistència o arquitectura avançada.
- `R2` queda com a construcció nuclear del mòdul sobre base comuna.
- `R3` es desdobla en `CP-R3A` i `CP-R3B` per controlar millor la càrrega i evitar que `RA5`, `RA6` i `RA8` es confonguen.
- `R4` reforça el contracte i el consum real com a nucli de `RA7`.
- `R5` queda situat com a síntesi amb nucli mínim obligatori de `RA9` i ampliació avançada opcional.

## Impacte sobre el paper de Repte 5 dins del mòdul

`Repte 5` actua com a lloc natural de desplegament de `RA9`. El seu valor està en comprovar que el backend construït fins a `R4` pot interoperar amb fonts externes, transformar dades i generar una funcionalitat híbrida defensable. El mínim obligatori és nuclear per al mòdul; les integracions múltiples, automatitzacions més riques o orquestracions avançades queden com a ampliació.
