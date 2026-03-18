# Curs executable DWES en 2 avaluacions

## Finalitat del document
Convertir el model docent del repositori en una peça única, reutilitzable i executable perquè el professorat puga posar en marxa el curs sense haver de reconstruir la seqüència a partir de documents dispersos.

Este document no substituïx [pla_implantacio_docent.md](pla_implantacio_docent.md), [calendaritzacio_orientativa_aula.md](calendaritzacio_orientativa_aula.md), [calendaritzacio_per_avaluacions.md](calendaritzacio_per_avaluacions.md), [programacio_aula_operativa_2_avaluacions.md](programacio_aula_operativa_2_avaluacions.md), [seqüenciacio_sessions_2_avaluacions.md](seqüenciacio_sessions_2_avaluacions.md) ni [matriu_evidencies_i_instruments_per_fase.md](../03_avaluacio/matriu_evidencies_i_instruments_per_fase.md). La seua funció és condensar-los en una guia de desplegament docent real.

## Condicions de partida del curs
- el curs es calibra sobre un escenari orientatiu de `20` setmanes, `6` hores setmanals i unes `120` hores lectives aproximades
- el desenvolupament principal del projecte s'ha de completar dins de les dues primeres avaluacions
- la tercera avaluació no és període central de desenvolupament, sinó espai residual o de connexió amb empresa o `FCT`
- el model de treball és per reptes i amb projecte base compartit
- l'alumnat ja té base prèvia de treball amb GitHub; per tant, Git i GitHub es tracten com a repàs metodològic, traçabilitat i criteri professional, no com a iniciació des de zero
- els dominis admesos continuen sent gestor d'incidències o tickets, sistema de reserves o cites i gestor intern de recursos o inventari
- els itineraris `Laravel`, `Express/Nest` i `FastAPI` són variacions tecnològiques del mateix producte docent, no cursos paral·lels
- la IA es tracta com a eina guiada i verificable; si s'usa en parts nuclears, cal deixar evidència i validació humana explícites

## Estructura global en 2 avaluacions
| Tram | Setmanes orientatives | Hores orientatives | Fases i reptes | Resultat exigible |
|---|---|---|---|---|
| **Avaluació 1** | `1-10` | `~60h` | `Fase 0`, `Fase 1`, `Fase 2` i inici de `Fase 3` | producte funcional amb auth o estat equivalent i entrada real a arquitectura i persistència |
| **Avaluació 2** | `11-20` | `~60h` | tancament de `Fase 3`, `Fase 4`, `Fase 5` i defensa final | producte persistent, publicat com a `API`, integrat i defensable |
| **Avaluació 3** | fora del nucli lectiu del projecte | residual | sense desenvolupament central del projecte | seguiment puntual, connexió amb empresa o `FCT`, tancaments menors si el centre els necessita |

Lectura operativa:
- si al final de l'Avaluació 1 no hi ha una base funcional real i una entrada clara a `R3`, el ritme del curs queda en risc
- si al mig de l'Avaluació 2 no hi ha persistència consolidada, no s'hauria d'obrir `R4`
- `R4`, `R5` i la defensa final no es poden ajornar a la tercera avaluació

## Què ha de tindre preparat el professorat abans de començar
- repositori del curs visible i amb les rutes clau identificades
- [enunciat_projecte_base.md](../05_projectes_tecnics/enunciat_projecte_base.md) compartit com a encàrrec base del producte
- selecció clara dels dominis admesos i del criteri amb què l'alumnat en triarà un
- materials comuns accessibles des del primer dia
- materials dels Reptes `2`, `3`, `4` i `5` preparats per a activació progressiva
- itineraris `Laravel`, `Express/Nest` i `FastAPI` disponibles com a suport de stack
- instruments mínims localitzats abans de començar: control inicial de repositori, rúbrica base de reptes, checklist de repte i defensa tècnica
- criteri compartit sobre ús verificable de la IA, `AI log`, `README`, `ADR`, proves i evidències de procés
- decisió docent sobre com es faran equips, seguiment i checkpoints dins de les dues primeres avaluacions

## Seqüència mínima obligatòria
### Tram 1. Arrancada i marc comú
Objectiu:
- activar el projecte amb criteris comuns de treball, evidència i traçabilitat

Accions mínimes:
- presentar el projecte base, els dominis i la seqüència per reptes
- posar en marxa el repositori i revisar criteris de `README`, commits, `ADR`, proves i ús de la IA
- comprovar que Git i GitHub es reorienten a metodologia de treball professional

Resultat mínim exigible:
- repositori usable
- primer `README`
- criteri d'evidències compartit

### Tram 2. Kickoff tècnic del producte
Objectiu:
- passar del marc comú a un producte amb domini, stack i esquelet tècnic defensable

Accions mínimes:
- seleccionar domini i focus funcional inicial
- triar itinerari tecnològic i justificar-lo
- deixar documentada una primera decisió tècnica

Resultat mínim exigible:
- entorn funcional
- domini i stack definits
- primera decisió tècnica registrada

### Tram 3. Base funcional del producte
Objectiu:
- resoldre `R2` com a nucli funcional real

Accions mínimes:
- implementar registre, login, logout o estat equivalent
- aplicar accés protegit, validacions i errors mínims
- recollir primeres proves i actualitzar documentació

Resultat mínim exigible:
- flux funcional real i reproduïble
- proves bàsiques
- `README` actualitzat

### Tram 4. Arquitectura i persistència
Objectiu:
- obrir i tancar `R3` com a base de mantenibilitat i persistència del producte

Accions mínimes:
- separar responsabilitats per capes o equivalent
- modelar dades i persistència
- revisar regressió mínima i coherència entre codi, proves i documentació

Resultat mínim exigible:
- model de dades explicable
- persistència coherent
- arquitectura mantenible

### Tram 5. Publicació i consum d'API
Objectiu:
- resoldre `R4` amb una `API` usable, documentada i provada

Accions mínimes:
- definir contracte mínim d'`API`
- publicar endpoints principals
- documentar i provar el consum

Resultat mínim exigible:
- `API` coherent amb el producte real
- proves verificables
- documentació d'`API` usable

### Tram 6. Integració híbrida, tancament i defensa
Objectiu:
- resoldre `R5`, tancar el producte i preparar defensa final abans de `FCT`

Accions mínimes:
- integrar servei extern, `n8n` o flux híbrid equivalent
- provar el recorregut complet
- revisar documentació final, autoria i discurs tècnic

Resultat mínim exigible:
- integració funcional
- prova de punta a punta
- defensa tècnica preparada

## Materials que s'activen en cada moment
| Moment | Materials prioritaris |
|---|---|
| **Inici de curs** | materials comuns, enunciat base del projecte, projecte base, sistema d'evidències |
| **Kickoff tècnic** | criteris metodològics, model d'itineraris, suport inicial de `Laravel`, `Express/Nest` o `FastAPI` |
| **Repte 2** | [materials del Repte 2](../04_materials/repte_02/), materials comuns, guia inicial de l'itinerari triat |
| **Repte 3** | [materials del Repte 3](../04_materials/repte_03/), materials comuns, suport directe d'itinerari per auth, capes i persistència |
| **Repte 4** | [materials del Repte 4](../04_materials/repte_04/), materials comuns, reutilització de l'itinerari en context d'`API` |
| **Repte 5** | [materials del Repte 5](../04_materials/repte_05/), materials comuns, suport final d'itinerari per integració i tancament |

## Evidències mínimes que s'han de recollir
- repositori actiu i traçable des del començament
- `README` inicial, `README` tècnic i `README` final actualitzats segons el tram
- decisions tècniques registrades amb `ADR` o equivalent quan hi haja impacte real
- proves mínimes de flux funcional, persistència, `API` i integració
- checklists de repte o comprovacions equivalents en punts de pas
- evidències de procés sobre validació, debugging i correcció d'errors
- `AI log` o registre equivalent quan la IA haja participat en parts rellevants
- documentació final i defensa tècnica coherent amb el repositori real

## Instruments mínims de seguiment
| Moment | Instrument principal | Instrument de suport | Ús mínim |
|---|---|---|---|
| **Arrancada** | `checklist_revisio_repo.md` | revisió de `README` i traçabilitat | comprovar que el curs comença amb metodologia i no amb improvisació |
| **R2** | `rubrica_base_reptes.md` | checklist del Repte 2 | validar que la base funcional és real i reproduïble |
| **R3** | `rubrica_base_reptes.md` | checklist del Repte 3 | comprovar arquitectura, persistència i mantenibilitat mínimes |
| **R4** | `rubrica_base_reptes.md` | checklist del Repte 4 | controlar coherència entre contracte, implementació, proves i documentació |
| **R5 i defensa** | `rubrica_defensa_tecnica.md` | checklist del Repte 5 | verificar producte final, integració, autoria i justificació tècnica |

## Punts de decisió docent
- si el repositori no mostra traçabilitat mínima en el tram inicial, no s'hauria de donar per estabilitzat el marc comú
- si el kickoff tècnic no deixa domini, stack i entorn funcional, convé retallar superfície del projecte abans d'obrir `R2`
- si `R2` no és reproduïble, no s'hauria d'obrir `R3`
- si `R3` no deixa persistència coherent i capes o equivalent explicables, no s'hauria d'obrir `R4`
- si `R4` no està provat ni documentat, no s'hauria d'avançar cap a `R5`
- si la integració final no té valor real o no és verificable, convé simplificar-la abans d'arribar a la defensa

## Adaptacions si baixa la càrrega real
- si la càrrega baixa per davall de les `120` hores orientatives, s'han de compactar activitats dins del mateix tram, no traslladar el nucli del projecte a la tercera avaluació
- la primera simplificació ha de recaure en ornamentació, refinament visual o ampliacions opcionals, no en auth, persistència, `API` o integració mínima
- si cal retallar abast, convé reduir nombre de casos d'ús del domini abans que relaxar traçabilitat, proves o documentació essencial
- els itineraris continuen sent útils en context reduït, però només com a suport per mantindre la viabilitat tècnica del producte
- si un grup queda bloquejat, és preferible absorbir temps dins de la mateixa avaluació i tancar una versió més curta però real

## Tancament del projecte abans de FCT/empresa
El criteri del model és que el projecte base del mòdul quede completat, documentat i defensat abans de l'entrada en `FCT` o empresa. Això implica:
- el producte ha d'estar tancat al final de la segona avaluació lectiva
- la tercera avaluació no pot quedar carregada amb `R4`, `R5` ni defensa final
- si el centre necessita connexions posteriors amb empresa, estes s'han de plantejar com a transferència, seguiment residual o contextualització professional, no com a resolució del nucli del curs

## Checklist final de curs
- el domini triat ha produït un producte recognoscible i usable
- el repositori mostra procés real, traçabilitat i documentació suficient
- `R2` ha deixat auth o estat equivalent funcional
- `R3` ha deixat persistència i arquitectura explicables
- `R4` ha deixat una `API` documentada i provada
- `R5` ha deixat una integració híbrida o automatització amb valor real
- `README`, decisions tècniques, proves i evidències finals estan actualitzades
- l'ús de la IA, si existix, és verificable i defensable
- el producte queda preparat per a defensa final abans de `FCT` o empresa

## Definition of done del document
Este document es considera completat quan:
- oferix una versió única i executable del curs per a professorat
- connecta explícitament amb la resta de documents d'implantació, calendarització, seqüenciació i avaluació
- deixa clar que el projecte s'ha de completar dins de les dues primeres avaluacions
- concreta què preparar, què activar, què recollir i amb què seguir cada tram
- manté Git/GitHub com a repàs metodològic i traçabilitat, no com a iniciació bàsica
- és reutilitzable en context real amb marge d'adaptació sense perdre el nucli del model
