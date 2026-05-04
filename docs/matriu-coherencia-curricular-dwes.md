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
| **RA1. Arquitectura i tecnologies servidor** | `Repte 1` i [enunciat del projecte base](05_projectes_tecnics/enunciat_projecte_base.md) | comparativa tècnica inicial, ADR o justificació tècnica, repositori executable, Docker, README, primera peça funcional | rúbrica del repte, checklist de revisió de repositori, defensa tècnica breu | execució real de l'entorn, justificació del stack, preguntes de transferència i microcanvis sobre arrencada | suport acceptable per comparar opcions, resumir documentació i detectar errors inicials | cobertura principal en `R1`; `RA5` només queda com a preparació no principal |
| **RA2. Codi executable embegut en llenguatges de marques** | `Repte 2` sobre base comuna en `PHP` | codi embegut executable, variables, operadors, directives, formulari base, resposta generada en servidor | checklist de formulari i recuperació de dades, rúbrica breu de processament bàsic | revisió de codi en context, execució del flux complet, reconstrucció guiada d'una part del processament | suport condicionat quan la IA propose esquelets de formulari o processament | concentrat en `R2`; no convé dissoldre'l dins d'autenticació |
| **RA3. Estructures de programació, formularis i interacció** | `Repte 2` i reforç funcional del projecte base | formulari funcional, recuperació de dades, decisions, arrays, funcions, comparativa abans/després en `MP7`, evidència de lògica aplicada | rúbrica del repte, checklist de flux funcional, revisió de repositori | casos positius i negatius, explicació de la lògica, modificació de condicions o validacions en directe | suport condicionat per a lògica i estructures; alt risc si l'alumne no pot explicar decisions i funcions | `R2` és el nucli; el pas a `R3` no ha de reavaluar `RA3` com a focus principal |
| **RA4. Estat, autenticació, prova i depuració** | `Repte 2` i checkpoints de pas a `R3` | demo d'estat, sessió o cookies, autenticació, cas autoritzat i denegat, registre d'incidències, proves mínimes, documentació i checkpoint tècnic | rúbrica del repte, checklist de verificació, defensa tècnica breu, observació docent | reproducció del login o operació protegida, explicació de l'estat, revisió d'errors i correccions, contrast entre codi i comportament | suport condicionat; zona d'alt risc si la IA resol autenticació o debugging sense comprensió real | `RA4` tanca `R2` i prepara `R3`; la defensa ha de verificar autoria individual |
| **RA5. Separació lògica-presentació, patrons i documentació** | `Repte 3`, [projecte backend base](05_projectes_tecnics/projecte_base_backend.md) i fase final integradora | diagnosi del codi anterior, pla de migració, estructura en framework, abans/després d'un cas d'ús, README, decisions tècniques, backlog de migració | rúbrica del repte, checklist d'arquitectura, revisió de repositori, defensa tècnica | explicació de rutes, controladors, serveis, vistes o equivalents, justificació d'estructura i de migració, revisió del canvi real al repositori | suport condicionat per modelat i refactorització; no acceptable si genera arquitectura opaca no defensable | `RA5` és el nucli de `R3`; es reactiva després en fase final, però no s'ha de reobrir com a refactorització infinita |
| **RA6. Accés a dades, integritat i seguretat** | `Repte 3` com a cobertura principal, `Repte 4` com a suport del servei i `Repte 5` només quan hi ha transformació o persistència externa | migrations, seeders, model de dades, lectura i escriptura reals, validacions, tractament d'errors, proves de regressió, dades reals servides per l'API | rúbrica del repte, checklist de persistència i proves, revisió de repositori, prova guiada | reconstrucció de BBDD, execució de consultes o fluxos amb dades reals, verificació d'errors i integritat mínima | suport condicionat i d'alt risc en model de dades, migracions i consultes | cobertura principal en `R3`; en `R4-R5` només ha d'aparéixer com a suport i no menjar-se `RA7` o el tancament transversal de `R5` |
| **RA7. Serveis web** | `Repte 4` com a cobertura principal, reforç en fase final i cobertura principal compartida en `R5` quan la integració reutilitza o orquestra serveis | contracte d'API, mapa d'endpoints, primer endpoint funcional, autenticació d'API, consum real, proves del servei, documentació d'API, defensa | rúbrica específica de servei, checklist de consum, revisió de repositori, defensa tècnica breu | consum real del servei, casos autoritzats i denegats, contrast entre contracte, codi i resposta observada | suport condicionat; alt risc de delegació excessiva en contractes, endpoints i documentació ornamental | `RA7` ha de dominar `R4` i dona sentit nuclear a `R5` quan hi ha integració entre servei propi i servei extern |
| **RA8. Generació dinàmica amb tecnologies/frameworks del servidor** | `Repte 3` com a focus principal, reactivació parcial en el projecte base i eventual projecció en `R5` quan la integració impacta en fluxos renderitzats o respostes del backend | projecte en framework arrancable, almenys un flux **server-rendered**, vistes o plantilles, formulari o interacció processada pel framework, resposta HTML dinàmica, proves mínimes | rúbrica del repte, checklist de fluxos end-to-end, revisió de repositori, observació docent | demostració d'almenys un flux renderitzat en servidor, explicació del circuit petició -> controlador -> vista/resposta -> dades | suport condicionat; risc mitjà si la IA genera vistes o plantilles no compreses | `RA8` està fortament concentrat en `R3`; en `R5` només reapareix si la integració modifica de manera visible el comportament dinàmic del backend |

## Cobertura per repte i pel projecte base

| Peça | RA principals | Evidències principals | Instruments vinculats |
|---|---|---|---|
| [Projecte base](05_projectes_tecnics/enunciat_projecte_base.md) | transversal `RA1-RA8` segons fase | README, arquitectura, decisions, proves, traçabilitat, defensa tècnica | revisió de repositori, rúbriques, defensa tècnica |
| [Repte 1](02_reptes/repte_01_kickoff_backend.md) | `RA1` | comparativa, ADR, Docker, README, arrencada, primera peça funcional | rúbrica, checklist, defensa tècnica breu |
| [Repte 2](02_reptes/repte_02_sessions_i_autenticacio.md) | `RA2`, `RA3`, `RA4` | formularis, codi embegut, lògica, estat, autenticació, proves, `AI log`, checkpoint | checklist, rúbrica, defensa tècnica breu, revisió de repositori |
| [Repte 3](02_reptes/repte_03_mvc_i_persistencia.md) | `RA5`, `RA6`, `RA8` | migració d'un cas d'ús, framework, BBDD, migrations, seeders, flux server-rendered, proves, README | rúbrica, checklist, revisió de repositori, defensa tècnica |
| [Repte 4](02_reptes/repte_04_api_i_consum.md) | `RA7` amb suport de `RA6` | contracte de servei, endpoints, consum real, autenticació d'API, documentació, proves, `AI log` | rúbrica específica, checklist, revisió de repositori, defensa tècnica breu |
| [Repte 5](02_reptes/repte_05_integracio_hibrida_n8n.md) | tancament transversal amb focus principal en `RA7`, projecció aplicada de `RA8` i suport eventual de `RA6` | connector extern, mapping, transformació, integració híbrida, proves, documentació, defensa | rúbrica, checklist d'integració, revisió de repositori, defensa tècnica |

## Relació amb ús assistit per IA

La matriu no regula de nou l'ús assistit per IA. La lectura és:

- **suport acceptable**: comparatives inicials, resum de documentació, esquelets de treball, ajuda de debugging i revisió de documentació
- **suport condicionat**: arquitectura, model de dades, autenticació, contractes API, integracions externes i proves sobre comportaments crítics
- **zona d'alt risc de delegació excessiva**: quan l'alumne no pot explicar el codi, no sap fer microcanvis, no entén la font externa o no pot relacionar evidència, prova i resultat

El criteri complet depén de [Ús de la IA per a professorat i alumnat](us-ia-professorat-i-alumnat.md).

## Cobertura global del mòdul

- La seqüència `R1-R5` cobreix tots els `RA` del mòdul `0613`.
- `RA1` queda concentrat en `R1`; `RA2-RA4` en `R2`; `RA5-RA6-RA8` en `R3`; `RA7` en `R4`; `R5` funciona com a tancament transversal amb focus principal en `RA7` i suport eventual de `RA8` i `RA6`.
- El projecte base i la defensa tècnica actuen com a peces transversals de coherència i verificació real.

## Buits o punts febles detectats

- `RA8` depén fortament de `R3` i pot quedar tapat darrere de persistència i framework si no es manté visible el flux **server-rendered**.
- `RA6` té risc de desbordar-se i competir massa amb `RA7` en `R4` o amb el caràcter transversal de `R5`.
- La qualitat de la verificació de l'ús assistit per IA depén molt de la constància real en `AI log`, revisió de repositori i defensa tècnica.

## Decisions de millora proposades per a la Fase 4

- Fer més explícita la comprovació de `RA8` en instruments de `R3` si es detecta que el flux renderitzat en servidor queda massa implícit.
- Revisar si els checklists de `R4` i `R5` diferencien prou bé suport de `RA6` i focus principal de `RA7` en integració.
- Estudiar si convé derivar una plantilla curta de verificació d'ús assistit per IA lligada als checkpoints principals del curs.

## Correcció curricular aplicada

- S'elimina el resultat d'aprenentatge inexistent que s'havia atribuït erròniament a `Repte 5`.
- `Repte 5` deixa d'aparéixer com a resultat d'aprenentatge autònom i passa a llegir-se com a tancament transversal de la seqüència.
- La seua justificació curricular queda recolzada sobretot en `RA7`, amb projecció aplicada de `RA8` quan la integració afecta respostes o fluxos del backend, i suport puntual de `RA6` quan hi ha persistència o transformació de dades externes.

## Impacte sobre el paper de Repte 5 dins del mòdul

`Repte 5` no fixa un `RA` nou ni obri una capa curricular separada. El seu valor està en comprovar que el backend construït fins a `R4` pot interoperar amb fonts externes, transformar dades i generar una funcionalitat híbrida defensable sense perdre traçabilitat, verificació ni control sobre l'ús assistit per IA.
