# Guia de README i ADR

## Finalitat

Fer que cada projecte o repte deixe documentació tècnica útil per a onboarding, continuïtat d'equip i defensa de decisions, no només una descripció superficial.

En el mòdul, un `README` i un `ADR` no són complements decoratius. Formen part de les evidències autèntiques del treball: permeten entendre què s'ha construït, com s'executa, quines decisions s'han pres i com es podria continuar o mantindre el projecte.

## Contingut operatiu

El `README` ha de permetre que una altra persona entenga i pose en marxa el treball sense dependre d'explicacions informals.

Contingut mínim d'un `README` tècnic:

- què resol el projecte o el lliurable
- requisits previs i dependències
- passos de posada en marxa
- com executar proves o verificacions mínimes
- estructura bàsica o punts rellevants del repositori
- limitacions, decisions pendents o advertències d'ús
- on estan les evidències clau del repte o del producte

Quan usar-lo dins del mòdul:

- en tots els reptes com a document mínim de continuïtat
- en el projecte base com a peça central de posada en marxa i manteniment
- sempre que hi haja canvis que afecten execució, proves o ús del producte

Un `ADR` s'ha d'usar quan cal documentar una decisió tècnica rellevant, per exemple:

- elecció de framework o arquitectura
- criteri de persistència o modelat
- contracte d'API o patró d'autenticació
- estratègia de proves o integració
- adopció d'una eina externa o d'un flux híbrid amb impacte en el projecte

Contingut mínim d'un `ADR`:

- context del problema
- alternatives considerades
- decisió adoptada
- conseqüències o impacte esperat

Criteri d'ús:

- no fa falta un `ADR` per cada detall menor
- sí que fa falta quan una decisió canvia l'arquitectura, la manera de provar, la manera d'integrar o la manera de mantindre el producte
- si una decisió és prou important per afectar defensa tècnica o mantenibilitat, convé deixar-la fora del cap de l'equip i portar-la a document

## Errors habituals o riscos

- convertir el `README` en text promocional en lloc de guia operativa
- deixar instruccions incompletes o desactualitzades
- no documentar decisions tècniques que després afecten manteniment o avaluació
- crear `ADR` massa genèrics, massa tard o per decisions irrellevants
- omplir el `README` amb teoria general del tema en lloc d'informació útil del projecte concret
- descriure una arquitectura o unes proves que no corresponen amb l'estat real del repositori

## Checklist final

- el `README` permet arrancar el treball i comprovar-ne l'estat real
- la documentació descriu el comportament actual i no una versió idealitzada
- les decisions importants no queden només en commits o converses
- els `ADR` documenten decisions significatives, no detalls trivials
- la documentació ajuda a defensar el treball en un entorn professional realista
- qualsevol membre de l'equip podria reprendre el treball amb la informació escrita
- els canvis importants en execució o arquitectura queden actualitzats a la documentació
