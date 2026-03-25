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
5. Definir projectes tècnics reals: backend, APIs, IA, n8n.

## Estructura
- `docs/00_visio_general/` visió global del mòdul
- `docs/alumnat/` accés web sintètic per a alumnat
- `docs/professorat/` accés web sintètic per a professorat
- `docs/01_programacio_modul/` nova programació
- `docs/02_reptes/` fitxes dels reptes
- `docs/03_avaluacio/` rúbriques, checklists i evidències
- `docs/04_materials/` mapa i adaptació d’apunts
- `docs/05_projectes_tecnics/` backend, IA, n8n, integracions
- `docs/06_plantilles/` plantilles reutilitzables
- `docs/07_presentacions/` micro-presentacions docents de curs, reptes i avaluació
- `docs/08_materials_compartibles/` peces breus i donables per a ús real en aula
- `docs/09_paquets_ús_directe/` agrupació dels materials més útils segons el moment del curs

## Navegació documental
- Índex central: [Index documental del projecte](docs/00_visio_general/index_documental.md)
- Recorreguts principals de consulta: alumnat per entendre i executar el curs; professorat per preparar-lo i conduir-lo; materials compartibles i paquets d'ús directe per a ús immediat en aula
- Accés d'alumnat: [portal d'apunts online](docs/alumnat/index.md)
- Consulta tècnica d'alumnat: [guia breu per dubtes reals del curs](docs/alumnat/consulta_tecnica/index.md), ara ampliada amb més fitxes i enllaços oficials o molt fiables
- Paquets d'ús directe: [agrupacions per moment del curs](docs/09_paquets_ús_directe/index.md) per saber què obrir, què donar i què usar en checkpoint o defensa
- Materials de classe compartibles: [peces curtes per a aula](docs/08_materials_compartibles/index.md), ara ja ampliades a `R1-R5`, checkpoints i tancament breu de defensa
- Accés de professorat: [portal docent de navegació ràpida](docs/professorat/index.md)
- Accés docent breu: [micro-presentacions del curs](docs/07_presentacions/presentacio_00_visio_curs.md)
- Índexs per blocs: [Programació del mòdul](docs/01_programacio_modul/index.md), [Avaluació](docs/03_avaluacio/index.md) i [Materials](docs/04_materials/index.md)
- Consulta web: la documentació queda preparada amb [mkdocs.yml](mkdocs.yml) i el workflow [docs.yml](.github/workflows/docs.yml) per publicar-se a GitHub Pages
- Primer desplegament: cal activar una vegada `Settings > Pages > Build and deployment > Source: GitHub Actions` al repositori `igomis/reestructuracioModul`
- Previsualització local: quan `mkdocs` estiga instal·lat, es pot llançar amb `mkdocs serve`

## Estat actual
La base curricular del projecte ja està definida i el repositori entra en fase de **implantació docent en 2 avaluacions lectives reals**.

Lectura ràpida de la fase actual:
- el projecte base del curs, l'enunciat base i la seua concretització en tres projectes base ja existixen i funcionen com a base pública usable del mòdul
- els materials nuclears dels Reptes `2`, `3`, `4` i `5` ja estan publicats, encara que `MG-05` i `MG-06` continuen oberts a una ronda final de consolidació
- els tres itineraris tecnològics (`Laravel`, `Express/Nest`, `FastAPI`) ja existixen com a paquet comparable dins d'un mateix marc docent
- la implantació docent ja està baixada a diversos nivells: pla general, calendarització orientativa, calendarització per avaluacions, programació d'aula operativa i seqüenciació fina de sessions
- el repositori entra ara en la capa de curs executable: una peça única perquè el professorat puga aplicar el model sense reconstruir la seqüència des de zero
- el model assumix que el desenvolupament principal del projecte es resol i es defensa dins de les dues primeres avaluacions; la tercera queda com a espai residual o de connexió amb empresa o `FCT`
- la implantació docent es calibra sobre un escenari orientatiu d'unes `20` setmanes i `6` hores setmanals, és a dir, unes `120` hores lectives dins de les dues primeres avaluacions
- Git/GitHub es tracta com a metodologia de treball, traçabilitat i repàs de criteris professionals, no com a iniciació des de zero
- el model admet moments de col·laboració limitada o de producte parcialment compartit, però el seguiment, la verificació, la defensa i l'acreditació es resolen individualment
- la seqüència docent completa del curs ja queda pilotable de punta a punta en un bloc coherent de `20` setmanes
- la `v1` prepilotatge queda preparada com a base estable i els projectes base concretats passen a producció com a encàrrec docent més tancat i més defensable
- la capa web per a alumnat i professorat, els materials compartibles i els paquets d'ús directe ja queden publicats com a accessos curts per a ús real
- la web ja queda usable com a entorn final de consulta per perfil i per moment d'ús, sense necessitat d'obrir noves capes de documentació

## Documents clau de la fase actual
- [Index documental del projecte](docs/00_visio_general/index_documental.md)
- [Index de programació del mòdul](docs/01_programacio_modul/index.md)
- [Index del bloc d’avaluació](docs/03_avaluacio/index.md)
- [Index del bloc de materials](docs/04_materials/index.md)
- [Curs executable DWES en 2 avaluacions](docs/01_programacio_modul/curs_executable_dwes_2_avaluacions.md)
- [Guia sessió a sessió del curs en 20 setmanes](docs/01_programacio_modul/guia_sessio_a_sessio_20_setmanes.md)
- [Guió docent complet de la setmana 1](docs/01_programacio_modul/setmana_01_guio_docent.md)
- [Revisió transversal del bloc pilotable de 20 setmanes](docs/01_programacio_modul/revisio_transversal_bloc_pilotable_20_setmanes.md)
- [Ajustos finals abans de l'inici de curs](docs/01_programacio_modul/ajustos_finals_abans_inici_curs.md)
- [Projectes base concretats del mòdul](docs/05_projectes_tecnics/projectes_base_concretats.md)
- [Estat de producció actual del projecte](docs/00_visio_general/issues_inicials.md)

## Focus actual
1. Mantindre la `v1` prepilotatge preparada com a base estable i reusable del paquet docent.
2. Tindre en producció els tres projectes base concretats del mòdul com a encàrrecs ja usables, comparables i defensables.
3. Mantindre visible i usable el doble accés web per a alumnat i professorat sense duplicar la documentació llarga.
4. Mantindre el paquet llest per a inici de curs amb ajustos només menors, sense reobrir l'arquitectura principal.
