# Presentació breu del model DWES per reptes amb IA

## Finalitat del document
Presentar de manera breu i compartible el model docent del mòdul DWES reestructurat, pensat per explicar-lo a professorat o equips que no han seguit tot el procés de disseny del repositori.

## Punt de partida: quin problema docent resol
El model naix per resoldre un problema freqüent: tindre programació, materials, activitats i avaluació poc connectats entre si. La proposta reorganitza el mòdul com un recorregut coherent cap a un producte backend real, amb reptes progressius, materials activables, seguiment docent i evidències autèntiques.

## Principis del redisseny del mòdul
- aprenentatge per reptes
- entorn professional realista
- producte base evolutiu durant tot el curs
- evidències autèntiques de procés i de resultat
- IA com a suport habitual però verificable
- desplegament docent executable en `2` avaluacions lectives

## Estructura per reptes i producte backend evolutiu
El curs s'organitza com una seqüència de reptes que fan créixer un mateix producte:
- `Repte 1`: arranque tècnic i decisió de domini
- `Repte 2`: base funcional amb auth o estat equivalent
- `Repte 3`: arquitectura i persistència
- `Repte 4`: `API`, documentació i proves
- `Repte 5`: integració híbrida, automatització i defensa final

Això evita activitats desconnectades i converteix el curs en una construcció incremental d'un backend usable.

## Paper de la IA: ús normal però verificable
La IA no es tracta com a excepció ni com a prohibició. S'assumix com una eina de suport normal per generar idees, contrastar codi, redactar, revisar o documentar. El criteri és que qualsevol ús rellevant ha de ser verificable, explicable i defensable per l'alumnat.

## Materials, itineraris i avaluació
El sistema combina tres capes:
- materials comuns del mòdul
- materials específics per repte
- itineraris tecnològics homologables: `Laravel`, `Express/Nest` i `FastAPI`

L'avaluació es basa en rúbriques, checklists, checkpoints i revisió de repositori. El nivell d'exigència és comú encara que canvie el stack.

## Implantació en 2 avaluacions
La proposta està pensada per a contextos on la 3a avaluació no és període central de desenvolupament perquè l'alumnat està en empresa o `FCT`.
- `Avaluació 1`: marc comú, kickoff tècnic, base funcional i entrada a persistència
- `Avaluació 2`: tancament de persistència, `API`, integració i defensa final
- `Avaluació 3`: espai residual, de connexió amb empresa o de tancament puntual

La referència temporal és d'unes `20` setmanes i `120` hores lectives aproximades.

## Què aporta al professorat
El model aporta:
- un curs ja seqüenciat i no només descrit
- materials activables quan toquen
- un producte base que dona coherència al mòdul
- criteris clars de seguiment i de pas entre fases
- una capa de paquet docent exportable i reutilitzable

## Què és transferible a altres mòduls
El més transferible no és el contingut tècnic concret de DWES, sinó el patró:
- organització per reptes
- producte base evolutiu
- materials comuns + materials específics + variants tecnològiques
- evidències autèntiques
- seguiment per checkpoints
- IA guiada i verificable

## Properes línies o tancament de fase
En esta fase, el model ja no necessita més arquitectura interna per ser comprensible. El pas següent és tancar una versió compartible o lliurable del paquet docent perquè puga circular com a proposta docent ja presentable.
