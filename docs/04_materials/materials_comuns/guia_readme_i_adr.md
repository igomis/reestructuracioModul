# Guia de README i ADR

## Finalitat
Fer que cada projecte o repte deixe documentació tècnica útil per a onboarding, continuïtat d'equip i defensa de decisions, no només una descripció superficial.

## Contingut mínim operatiu
El `README` ha de permetre que una altra persona entenga i pose en marxa el treball sense dependre d'explicacions informals.

Contingut mínim d'un `README` tècnic:
- què resol el projecte o el lliurable
- requisits previs i dependències
- passos de posada en marxa
- com executar proves o verificacions mínimes
- estructura bàsica o punts rellevants del repositori
- limitacions, decisions pendents o advertències d'ús

Un `ADR` s'ha d'usar quan cal documentar una decisió tècnica rellevant, per exemple:
- elecció de framework o arquitectura
- criteri de persistència o modelat
- contracte d'API o patró d'autenticació
- estratègia de proves o integració

Contingut mínim d'un `ADR`:
- context del problema
- alternatives considerades
- decisió adoptada
- conseqüències o impacte esperat

## Checklist o punts clau
- el `README` permet arrancar el treball i comprovar-ne l'estat real
- la documentació descriu el comportament actual i no una versió idealitzada
- les decisions importants no queden només en commits o converses
- els `ADR` documenten decisions significatives, no detalls trivials
- la documentació ajuda a defensar el treball en un entorn professional realista

## Errors habituals o riscos
- convertir el `README` en text promocional en lloc de guia operativa
- deixar instruccions incompletes o desactualitzades
- no documentar decisions tècniques que després afecten manteniment o avaluació
- crear `ADR` massa genèrics, massa tard o per decisions irrellevants
