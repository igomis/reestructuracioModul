# Realineació del backlog d'issues

## Situació actual
El repositori ha avançat més en documents i definició operativa que en la gestió pública d'issues. La fase de bootstrap ja està resolta, però el backlog visible encara arrossega una lògica inicial que no reflectix bé el moment actual del projecte.

Estat real de la fase actual:
- el README continua marcant com a focus tancar reptes, concretar evidències i connectar materials
- el projecte base ja té document backend i enunciat base redactat
- el pla de materials prioritaris ja està definit i permet passar de mapa general a planificació executiva
- les issues de reptes `R3-01`, `R4-01` i `R5-01` continuen sent útils com a fils de consolidació docent
- el backlog actiu ha de desplaçar-se ara cap a una fase de producció de materials, no cap a tasques de bootstrap

Nota de fase:
- amb `MG-02`, el projecte entra en producció efectiva dels materials comuns mínims que han de servir de base reutilitzable abans d'obrir materials específics per repte o per itinerari
- en la fase actual, `MG-02` passa de producció inicial a consolidació perquè estes guies ja han de poder funcionar com a materials reals i no com a esquelets mínims
- amb `MG-03`, el projecte obri el primer paquet específic de repte i trasllada la producció de materials al flux funcional de sessions, autenticació i validació del Repte 2
- amb `MG-04`, el projecte entra en el paquet de materials d'arquitectura, persistència i qualitat tècnica del Repte 3, que ha de preparar directament la transició cap a API

## Issues inicials que convé tancar
Les issues inicials de bootstrap han de quedar fora del backlog actiu perquè ja responen a treball resolt o superat:

- `#1 A1-01 · Completar la rúbrica base de reptes`
- `#2 R1-01 · Completar la fitxa docent del Repte 1`
- `#3 M1-01 · Completar el mapa de materials actuals`
- `#4 P1-01 · Consolidar el document de projecte backend base`
- `#5 G1-01 · Crear issues reals a GitHub a partir del backlog`

Criteri de tancament:
- són tasques ja executades o absorbides per documents consolidats del repositori
- mantenir-les com a referència oberta distorsiona la lectura del backlog real
- el focus ja no és arrancar el projecte, sinó produir materials útils per als reptes i per al projecte base

## Issues noves recomanades
El backlog recomanat per a la fase actual ha d'incorporar les issues següents:

| Codi | Prioritat | Objectiu principal | Referència de treball |
|---|---|---|---|
| **PB-01 · Verificar i consolidar l’enunciat base del projecte del curs** | alta | revisar que l'enunciat base queda complet, visible i alineat amb el producte del curs | `docs/05_projectes_tecnics/enunciat_projecte_base.md` |
| **MG-01 · Planificar materials nous prioritaris per repte** | alta | mantindre una planificació executable dels materials nous prioritaris | `docs/04_materials/pla_materials_prioritaris.md` |
| **MG-02 · Crear materials comuns mínims del mòdul** | alta | produir materials comuns sobre Git, README/ADR, testing/debugging i IA verificable | `docs/04_materials/` |
| **MG-03 · Crear materials nuclears del Repte 2** | alta | produir materials de sessions, autenticació, validació i proves bàsiques | `docs/04_materials/repte_02/` |
| **MG-04 · Crear materials nuclears del Repte 3** | alta | produir materials de MVC o equivalent, persistència segura i qualitat mínima | `docs/04_materials/repte_03/` |
| **MG-05 · Crear materials d’API i proves** | mitjana-alta | produir materials de contracte API, documentació, consum i col·leccions de prova | `docs/04_materials/materials_repte_04/` |
| **MG-06 · Crear materials d’integració híbrida i n8n** | mitjana | produir materials per al tancament del producte amb integració externa, automatització i manteniment | `docs/04_materials/materials_repte_05/` |
| **MG-07 · Planificar materials específics per Laravel / Express-Nest / FastAPI** | mitjana | ordenar l'adaptació dels materials de R3-R5 per itineraris tecnològics guiats | `docs/01_programacio_modul/model_itineraris_tecnologics.md` |

Lectura recomanada del nou backlog:
- `PB-01` i `MG-01` actuen com a peces de consolidació i control de coherència
- `MG-02` és la base comuna que ha de precedir la producció específica
- `MG-03` i `MG-04` obrin la producció tècnica principal perquè connecten directament amb el producte del curs
- `MG-05` i `MG-06` despleguen la capa d'API, proves i integració híbrida
- `MG-07` ordena l'entrada dels itineraris específics quan la base comuna ja és prou estable

## Ordre recomanat de treball
1. Consolidar `PB-01` perquè l'enunciat base del projecte ha de quedar plenament verificat i sense dubtes de sincronització.
2. Revalidar `MG-01` com a document de planificació i usar-lo com a marc de producció real.
3. Executar `MG-02` per disposar dels materials comuns mínims del mòdul.
4. Executar `MG-03` i `MG-04` com a nucli inicial de producció de materials per reptes.
5. Obrir `MG-07` després de `MG-04` per planificar amb criteri els materials per itinerari.
6. Executar `MG-05` quan la base de R3 ja estiga estabilitzada.
7. Executar `MG-06` com a tancament de la primera onada de producció de materials.

## Definition of done
Esta realineació es considera completada quan:
- el document deixa constància que el backlog inicial de bootstrap ja no és el focus actiu
- les issues `#1` a `#5` queden clarament identificades com a tasques que s'han de mantindre tancades
- el backlog recomanat queda orientat a `PB-01`, `MG-01` i a la nova sèrie `MG-02` a `MG-07`
- l'ordre de treball reflectix la fase actual del projecte: consolidació mínima i producció real de materials
- el document pot usar-se com a guia directa per revisar i crear issues a GitHub sense haver de reinterpretar el context
