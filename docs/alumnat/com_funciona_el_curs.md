# Com funciona el curs

## El model del curs

Este mòdul es treballa per reptes. Això vol dir que no faràs peces inconnexes, sinó un mateix producte backend que va creixent al llarg del curs.

La seqüència és:

- `R1`: arrancada real del producte
- `R2`: base comuna en `PHP` amb dades, lògica, estat i autenticació
- `R3`: entrada de framework, arquitectura mantenible i persistència
- `R4`: publicació i consum d'API
- `R5`: integració híbrida, tancament i defensa

La idea clau és esta:

- en `R2` tot el grup treballa sobre una base comuna més controlada
- el contrast de frameworks comença després
- el mateix projecte continua amb itineraris diferents a partir de `R3`

## El producte base

Des del principi has de treballar sobre un projecte base recognoscible. No és una pràctica solta ni una demo per a cada tema.

El producte base:

- ha de tindre un cas d'ús real
- ha de poder créixer sense reiniciar-lo a cada repte
- en `R2` es treballa sobre una base comuna en `PHP`
- des de `R3` pot continuar-se amb `Laravel`, `Symfony` o `NestJS`
- s'ha de poder defensar individualment encara que hi haja anàlisi compartida, revisió creuada o checkpoints comuns

Pots consultar els tres projectes admesos en [Projectes base](projectes_base.md).

## Com es combina cooperació i autoria

La modalitat preferent és:

- mateix projecte
- mateix encàrrec funcional
- repositoris individuals
- evidències individuals
- defensa individual
- contrast tècnic compartit

El model base és el de parelles de contrast tècnic. En alguns casos es poden obrir trios avançats amb tres stacks diferents, però no és la modalitat general.

## Dues avaluacions lectives

El desenvolupament principal del projecte es resol dins de les dues primeres avaluacions.

Lectura pràctica:

- **Avaluació 1:** arrancada, `R1`, `R2` i entrada a `R3`
- **Avaluació 2:** tancament de `R3`, `R4`, `R5` i defensa final
- **Avaluació 3:** no és el tram central del projecte; si existix, queda com a espai residual, de connexió amb empresa o de tancaments menors

Si acabes la primera avaluació sense una base funcional real, després vas tard.

## Què s'espera del teu treball

- treball regular sobre el mateix repositori
- un producte funcional i no trivial en cada repte
- `README`, proves, decisions i evidències actualitzades
- traçabilitat real amb commits i procés recognoscible
- capacitat d'explicar què has fet, per què i com ho has verificat

No és suficient:

- muntar esquelets buits
- fer només la tècnica aïllada del tema
- deixar funcionalitat sense proves ni comprovació real
- entregar codi que no pots defensar

## Què vol dir mínim funcional no trivial

Vol dir que cada repte ha de deixar una part del producte que tinga valor real i es puga provar.

No vol dir:

- una tècnica solta sense cas d'ús
- una pantalla o ruta ornamental
- un esquelet que “ja completarem després”

Sí vol dir:

- una acció recognoscible del producte
- una validació o regla mínima de negoci
- una comprovació real que funciona
- una base que permeta obrir el repte següent sense reconstruir-ho tot

## Què has d'anar deixant durant el curs

- repositori usable des del principi
- evidències mínimes de cada repte
- proves o verificacions del flux principal
- documentació tècnica operativa
- `AI log` o registre equivalent si uses IA en parts rellevants

## Si vols el document llarg

La versió docent completa està en [Curs executable DWES en 2 avaluacions](../01_programacio_modul/curs_executable_dwes_2_avaluacions.md).
