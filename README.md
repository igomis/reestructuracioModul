# Reestructuració del mòdul DWES

Repositori de treball per al redisseny del mòdul **Desenvolupament d’Aplicacions Web en Entorn Servidor** en clau de:

- aprenentatge per reptes
- integració guiada de IA
- entorn professional realista
- activitats formativo-productives
- avaluació basada en evidències autèntiques

## Objectius del repositori

1. Reestructurar la programació del mòdul.
2. Dissenyar els reptes del curs.
3. Adaptar els materials actuals.
4. Crear rúbriques i instruments d’avaluació.
5. Definir projectes tècnics reals: backend, APIs, IA i integracions.

## Seqüència metodològica actual

El model del repositori queda fixat així:

- `R1` obri el projecte i deixa una primera peça funcional real.
- `R2` es resol sobre una **base comuna en PHP** per a tot l’alumnat.
- `R2` es desplega en `7` sessions de `3` hores i incorpora una sessió final específica de refactorització i millora de mantenibilitat, amb organització simple en fitxers i un objecte mínim de domini.
- el contrast fort de frameworks **no entra com a norma general en `R2`**
- a partir de `R3` el mateix projecte pot continuar-se amb itineraris diferents
- els frameworks base del tram de contrast són `Laravel`, `Symfony` i `NestJS`
- `FastAPI` deixa de ser itinerari base general i queda com a opció avançada o excepcional quan hi haja criteri docent

La modalitat preferent és:

- mateix projecte
- mateix encàrrec funcional
- repositoris individuals
- evidències individuals
- defensa individual
- contrast tècnic compartit

El model base de cooperació és el de **parelles de contrast tècnic**. Els **trios avançats** només s’obrin com a possibilitat puntual en equips amb prou autonomia. En tots els casos, la cooperació no substituïx l’autoria, la traçabilitat ni la defensa individual.

## Estructura

- `docs/00_visio_general/` visió global del mòdul
- `docs/alumnat/` accés web sintètic per a alumnat
- `docs/professorat/` accés web sintètic per a professorat
- `docs/01_programacio_modul/` nova programació
- `docs/02_reptes/` fitxes dels reptes
- `docs/03_avaluacio/` rúbriques, checklists i evidències
- `docs/04_materials/` mapa i adaptació d’apunts
- `docs/05_projectes_tecnics/` backend, IA, n8n i integracions
- `docs/06_plantilles/` plantilles reutilitzables
- `docs/07_presentacions/` micro-presentacions docents de curs, reptes i avaluació
- `docs/08_materials_compartibles/` peces breus i donables per a ús real en aula
- `docs/09_paquets_ús_directe/` agrupació dels materials més útils segons el moment del curs

## Navegació documental

- Índex central: [Index documental del projecte](docs/00_visio_general/index_documental.md)
- Accés d'alumnat: [portal d'apunts online](docs/alumnat/index.md)
- Accés de professorat: [portal docent de navegació ràpida](docs/professorat/index.md)
- Paquets d'ús directe: [agrupacions per moment del curs](docs/09_paquets_ús_directe/index.md)
- Materials de classe compartibles: [peces curtes per a aula](docs/08_materials_compartibles/index.md)
- Índexs per blocs: [Programació del mòdul](docs/01_programacio_modul/index.md), [Avaluació](docs/03_avaluacio/index.md) i [Materials](docs/04_materials/index.md)
- Consulta web: la documentació queda preparada amb [mkdocs.yml](mkdocs.yml) i el workflow [docs.yml](.github/workflows/docs.yml) per publicar-se a GitHub Pages
- Primer desplegament: cal activar una vegada `Settings > Pages > Build and deployment > Source: GitHub Actions` al repositori `igomis/reestructuracioModul`
- Previsualització local: quan `mkdocs` estiga instal·lat, es pot llançar amb `mkdocs serve`

## Estat actual

La base curricular del projecte ja està definida i el repositori entra en fase de **implantació docent en 2 avaluacions lectives reals**.

Lectura ràpida de la fase actual:

- el projecte base del curs, l'enunciat base i la seua concretització en tres projectes base ja existixen com a base pública usable del mòdul
- `R2` queda definit com a base comuna controlada en PHP per consolidar tractament de dades, lògica bàsica, estat o sessió, autenticació i funcionalitat protegida
- la sessió `7` de `R2` queda lligada a refactorització i millora de mantenibilitat, amb `include` / `require` i un objecte mínim de domini, no a una entrada obligatòria a POO completa o BBDD com a focus central
- el contrast de frameworks s’obri a partir de `R3` sobre el mateix projecte i el mateix encàrrec funcional
- `Laravel`, `Symfony` i `NestJS` passen a ser els frameworks base del tram de contrast
- `FastAPI` es manté documentat només com a via avançada o excepcional
- la implantació docent ja està baixada a diversos nivells: pla general, calendarització orientativa, calendarització per avaluacions, programació d'aula operativa i seqüenciació fina de sessions
- el model assumix repositoris, evidències, verificació i defensa **individuals**
- la cooperació es planteja com a revisió creuada, checkpoints comuns i contrast tècnic compartit, no com a autoria col·lectiva
- la seqüència docent completa del curs ja queda pilotable de punta a punta en un bloc coherent de `20` setmanes

## Documents clau de la fase actual

- [Index documental del projecte](docs/00_visio_general/index_documental.md)
- [Index de programació del mòdul](docs/01_programacio_modul/index.md)
- [Programació d'aula del Repte 2](docs/01_programacio_modul/programacio_aula_repte_02.md)
- [Index del bloc d’avaluació](docs/03_avaluacio/index.md)
- [Index del bloc de materials](docs/04_materials/index.md)
- [Curs executable DWES en 2 avaluacions](docs/01_programacio_modul/curs_executable_dwes_2_avaluacions.md)
- [Model d’itineraris tecnològics guiats](docs/01_programacio_modul/model_itineraris_tecnologics.md)
- [Projectes base concretats del mòdul](docs/05_projectes_tecnics/projectes_base_concretats.md)
- [Estat de producció actual del projecte](docs/00_visio_general/issues_inicials.md)

## Focus actual

1. Mantindre la `v1` prepilotatge preparada com a base estable i reusable del paquet docent.
2. Deixar explícita i coherent la seqüència `R2` comú en PHP en `7` sessions, amb sessió final de mantenibilitat, `include` / `require` i un objecte mínim de domini, -> contrast de frameworks des de `R3`.
3. Fixar el model preferent de cooperació com a implementació individual amb contrast tècnic compartit.
4. Mantindre visible i usable el doble accés web per a alumnat i professorat sense duplicar la documentació llarga.
