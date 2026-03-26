# Pla d'execució del pilotatge real

## Finalitat del document

Baixar el pilotatge real del mòdul a una peça operativa perquè el professorat sàpia com iniciar-lo, amb quin abast mínim, què ha de registrar en cada punt i com convertir el feedback en decisions útils sobre el paquet docent.

Este document complementa [pla_pilotatge_real.md](pla_pilotatge_real.md). El pla de pilotatge definix el marc, la hipòtesi i els objectius; esta peça definix com executar el pilotatge en context real.

## Context del pilotatge

El paquet docent ja està en una versió `1` funcional i ha passat per una fase llarga de definició de reptes, materials, itineraris, implantació, avaluació i apunts reals. El pas següent ja no és afegir arquitectura documental, sinó validar el sistema en ús real amb alumnat.

El pilotatge s'ha d'entendre com una prova docent controlada d'un model ja usable, no com una primera exploració improvisada.

## Grup o escenari de pilotatge

Escenari recomanat de pilotatge:

- un grup real del mòdul `DWES`
- una aplicació completa del recorregut en dues primeres avaluacions
- un itinerari tecnològic principal triat per coherència docent i disponibilitat real del professorat
- ús dels altres itineraris com a suport o referència, però sense forçar comparativa completa si no hi ha condicions per sostenir-la

Si hi ha més d'un grup disponible:

- convé començar amb un sol grup pilot
- només té sentit obrir un segon grup si el professorat pot mantindre el mateix nivell de seguiment i registre

## Condicions de partida

Hipòtesi de treball assumida per a l'execució:

- `20` setmanes aproximades
- `6` hores setmanals
- `120` hores lectives aproximades
- desenvolupament principal del projecte dins de les dues primeres avaluacions
- tercera avaluació fora del desenvolupament nuclear del projecte, com a espai residual o de connexió amb empresa o `FCT`

Condicions docents mínimes:

- materials comuns, materials per repte i apunts reals disponibles abans de començar
- itinerari principal decidit abans de l'arrancada del curs
- instruments de seguiment accessibles i assumits pel professorat
- criteri compartit sobre evidències, `README`, `AI log`, proves i defensa tècnica
- alumnat amb base prèvia de treball amb GitHub; per tant, `Git/GitHub` es tracta com a repàs metodològic i criteri de traçabilitat, no com a iniciació des de zero

## Abast mínim del pilotatge

Per considerar que el pilotatge és real i útil, com a mínim s'ha d'aplicar:

- la seqüència `R1-R5`
- la lògica d'implantació en dues avaluacions lectives
- els checkpoints mínims del curs
- els materials comuns i els apunts reals dels reptes
- els instruments de seguiment, feedback i incidències
- la revisió del producte final amb defensa tècnica i ús verificable de la IA

No es recomana reduir el pilotatge a:

- només una part del curs
- només una prova de materials sense producte real
- només observació informal sense registre d'incidències i feedback

## Decisió recomanada de pilotatge

La decisió recomanada és fer un pilotatge complet però controlat:

- un únic grup
- un únic itinerari principal
- seguiment setmanal o quinzenal amb registre breu
- checkpoints formals en els punts de pas crítics
- recollida de feedback concentrada al tancament de `R1`, final d'avaluació `1`, tancament de `R4` i tancament de `R5`

La prioritat no és comparar totes les variants possibles, sinó validar si el model central aguanta bé una implantació real sense improvisació excessiva.

## Preparació prèvia del professorat

Abans d'iniciar el pilotatge, el professorat hauria de deixar tancat:

- itinerari principal de pilotatge
- seqüència real del curs segons les dues avaluacions disponibles
- materials clau que s'activaran en cada repte
- criteri de què compta com a evidència suficient en cada checkpoint
- sistema de registre: seguiment per equip, acta de checkpoint, feedback i incidents
- criteri de canvi immediat vs canvi reservat per a una `v2`

També convé preparar:

- un repositori de referència o exemple mínim intern, si ajuda a desbloquejar arrencada
- una carpeta o espai únic on es guarden registres del pilotatge
- una pauta breu de comunicació perquè l'alumnat entenga com es revisarà el curs

## Preparació prèvia de l'alumnat

Abans d'entrar en `R1`, l'alumnat ha de tindre clar:

- que el curs es treballa per reptes sobre un mateix producte backend
- que el projecte s'ha de completar dins de les dues primeres avaluacions
- que `Git/GitHub` es revisa com a metodologia i traçabilitat, no com a bloc d'iniciació
- que cada repte exigix evidències reproduïbles, no només una demo
- que la IA es pot usar, però amb registre mínim, verificació i capacitat de defensa

## Checkpoints reals del pilotatge

| Checkpoint | Moment | Objectiu real |
|---|---|---|
| `CP-P0` | abans de començar amb alumnat | verificar que el professorat té preparats materials, instruments i itinerari |
| `CP-P1` | tancament de `R1` | confirmar que l'arrancada funcional real del producte és viable en el temps previst |
| `CP-P2` | final de `R2` / tancament d'avaluació `1` | veure si el primer bloc funcional del producte i l'inici de `R3` són assumibles dins de la primera avaluació |
| `CP-P3` | tancament de `R3` | validar si arquitectura i persistència sostenen bé l'obertura de `API` |
| `CP-P4` | tancament de `R4` | comprovar si contracte, consum i documentació d'`API` aguanten una revisió real sense forçar el calendari |
| `CP-P5` | tancament de `R5` i defensa final | decidir si el paquet permet tancar el projecte dins de les dues primeres avaluacions amb criteri professional |
| `CP-P6` | tancament del pilotatge | resumir ajustos aplicats, ajustos pendents i viabilitat de la iteració següent |

## Què s'ha de registrar en cada checkpoint

En cada checkpoint convé deixar, com a mínim:

- estat real del producte
- evidències revisades
- problemes detectats
- desviació temporal respecte a la previsió
- decisió docent adoptada
- canvi immediat aplicat, si n'hi ha
- ajust pendent per a revisió posterior, si cal

Regla pràctica:

- si el checkpoint afecta un equip concret, convé combinar registre per equip i acta breu
- si el checkpoint afecta el model docent en conjunt, convé afegir també una entrada al registre d'incidents i ajustos

## Com s'usarà la plantilla de feedback

La [plantilla_recollida_feedback_pilotatge.md](../03_avaluacio/plantilla_recollida_feedback_pilotatge.md) s'ha d'usar:

- al final de `R1`
- al tancament de la primera avaluació
- després del pas per `R4`
- al tancament de `R5` o defensa final

Ús recomanat:

- una versió breu per a alumnat
- una versió paral·lela o complementària per a observació docent
- síntesi dels patrons repetits, no només llistat de comentaris aïllats

No convé usar-la:

- només al final del curs
- com a qüestionari genèric sense connexió amb reptes, càrrega o instruments

## Com s'usarà el registre d'incidents i ajustos

El [registre_incidents_i_ajustos_pilotatge.md](../03_avaluacio/registre_incidents_i_ajustos_pilotatge.md) s'ha d'activar des del primer incident rellevant i no esperar al tancament del pilotatge.

Convé registrar-hi:

- bloquejos recurrents d'un mateix repte
- sobrecàrrega temporal clara
- materials que obliguen a massa explicació addicional
- problemes d'ús dels instruments d'avaluació o seguiment
- dificultats repetides sobre evidències, `README`, proves o `AI log`

## Criteris per decidir canvis immediats

Convé aplicar un canvi immediat quan:

- el problema bloqueja el progrés del grup dins del calendari real
- la incidència afecta una peça instrumental bàsica del curs
- l'ajust no altera el model central, però sí en millora la viabilitat immediata
- hi ha risc de generar una lectura incorrecta d'un repte si no s'actua

Exemples de canvi immediat:

- aclarir una instrucció d'un material
- simplificar una evidència massa ambigua
- reordenar un checkpoint o una pauta de seguiment

## Criteris per reservar canvis per a una v2

Convé reservar un canvi per a una `v2` quan:

- implica reescriure diversos documents del paquet
- afecta el model global del curs i no només una peça concreta
- encara no hi ha prou evidència perquè el problema siga estructural
- el canvi podria introduir una desviació major enmig del pilotatge

Exemples de canvi per a `v2`:

- redisseny complet d'un repte
- canvi de la seqüència temporal global
- comparativa formal i simultània entre itineraris
- revisió profunda del sistema de ponderació sense prou dades del pilotatge

## Resultat esperat del pilotatge

S'espera arribar al final del pilotatge amb:

- una validació real del paquet docent en context d'aula
- un registre usable de feedback, incidents i decisions
- una llista curta i prioritzada d'ajustos immediats ja aplicats
- una llista separada de canvis reservats per a una `v2`
- criteri suficient per decidir si el paquet passa a ús estable, a segona iteració o a revisió parcial

## Definition of done del pla d'execució

Este pla d'execució es considera completat quan:

- el professorat pot iniciar el pilotatge sense reconstruir el procediment des de zero
- queden definits escenari, abast mínim, checkpoints i ús dels instruments
- la hipòtesi temporal de `20` setmanes, `6` hores setmanals i `120` hores queda integrada de manera explícita
- queda clar què es registra, quan i amb quina finalitat
- es diferencien amb criteri els canvis immediats dels canvis reservats per a una `v2`
