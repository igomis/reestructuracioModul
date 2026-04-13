# NestJS: consulta ràpida

## Què és

És una guia curta per situar les peces clau de `NestJS` dins del curs. No substituïx la documentació oficial: t'ajuda a llegir el framework com a eina de treball del teu projecte i no com a generador opac d'estructura.

## Quan la necessites en el curs

- a partir de `R3`, quan entra el contrast de frameworks
- en `R3`, per no barrejar lògica, persistència i entrada HTTP
- en `R4`, per publicar `API` sobre una base mantenible
- en `R5`, per integrar i mantindre el mateix producte

## Què has de saber sí o sí

- `module`, `controller`, `service`, `guard` i `dto` no poden ser màgia negra
- has de saber on entra la petició, on es valida, on es resol la lògica i on es persistix
- no és bona idea deixar tota la lògica en `main.ts` o en un sol controlador
- la configuració d'entorn i les proves mínimes formen part del projecte

## Errors habituals

- projectes `Nest` generats amb `CLI` però no compresos
- barrejar rutes, lògica i dades al mateix lloc
- triar `NestJS` només per moda o per suggeriment d'IA
- no deixar clar quin flux es validarà, quin persistirà i quin es publicarà com a `API`

## On ampliar

- Material del curs: [Guia de bootstrap NestJS](../../04_materials/itineraris/express_nest/guia_bootstrap_express_nest.md)
- Material del curs: [Guia d'auth i persistència NestJS](../../04_materials/itineraris/express_nest/guia_auth_i_persistencia_express_nest.md)
- NestJS Docs: [Controllers](https://docs.nestjs.com/controllers)
- NestJS Docs: [Authentication](https://docs.nestjs.com/security/authentication)
