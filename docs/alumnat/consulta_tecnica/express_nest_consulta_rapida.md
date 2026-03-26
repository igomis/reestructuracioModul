# Express/Nest: consulta ràpida

## Què és

És una guia curta per situar les peces clau de la via `Node.js` del curs. Et servix tant si vas per `Express` com si vas per `Nest`, però sempre amb la mateixa idea: backend explicable, no estructura opaca.

## Quan la necessites en el curs

- en `R1`, per decidir i defensar si et convé més `Express` o `Nest`
- en `R2`, per separar auth, accés i operació protegida
- en `R3`, per no barrejar lògica, persistència i entrada HTTP
- en `R4`, per publicar `API` sobre una base mantenible

## Què has de saber sí o sí

- en `Express`, la llibertat estructural exigix disciplina teua
- en `Nest`, `module`, `controller`, `service`, `guard` i `dto` no poden ser màgia negra
- has de saber on entra la petició, on es valida, on es resol la lògica i on es persistix
- no és bona idea deixar tota la lògica en `app.ts`, en una ruta o en un sol controlador
- la configuració d'entorn i les proves mínimes formen part del projecte

## Errors habituals

- projectes `Express` sense arquitectura recognoscible
- projectes `Nest` generats amb `CLI` però no compresos
- barrejar rutes, lògica i dades al mateix lloc
- triar `Express` o `Nest` només per moda o per suggeriment d'IA
- no deixar clar quin flux es validarà, quin persistirà i quin es publicarà com a `API`

## On ampliar

- Material del curs: [Guia de bootstrap Express/Nest](../../04_materials/itineraris/express_nest/guia_bootstrap_express_nest.md)
- Material del curs: [Guia d'auth i persistència Express/Nest](../../04_materials/itineraris/express_nest/guia_auth_i_persistencia_express_nest.md)
- Express Docs: [Routing](https://expressjs.com/en/guide/routing.html)
- Express Docs: [Using middleware](https://expressjs.com/en/guide/using-middleware.html)
- NestJS Docs: [Controllers](https://docs.nestjs.com/controllers)
- NestJS Docs: [Authentication](https://docs.nestjs.com/security/authentication)
