# Errors HTTP i codis de resposta

## Què és

És la lectura mínima dels codis que el backend torna quan una petició va bé, falla o queda denegada. En el curs no importa memoritzar-los tots: importa usar els que expliquen de veritat què ha passat.

## Quan la necessites en el curs

- en `R2`, per distingir validació, accés denegat i error intern
- en `R4`, quan l'`API` ja és una interfície pública del teu producte
- en `R5`, quan una integració o un `workflow` ha de reaccionar davant errors

## Què has de saber sí o sí

- `2xx` indica èxit; `4xx`, problema de petició o permisos; `5xx`, error del servidor
- `400`, `401`, `403`, `404`, `409`, `422` i `500` solen cobrir gran part dels casos del curs
- el codi i el cos de resposta han de contar la mateixa història
- si el backend valida dades, l'error ha de dir què falta o què és invàlid
- si denies un accés, has de distingir entre no autenticat i no autoritzat

## Errors habituals

- respondre `200` a tot, inclosos errors
- usar `500` per a problemes de validació o permisos
- tornar missatges massa vagues com "ha fallat"
- no documentar quins errors pot rebre el consumidor
- provar només el cas correcte i no els codis d'error

## On ampliar

- Material del curs: [Guia de validació i errors de servidor](../../04_materials/repte_02/guia_validacio_i_errors_servidor.md)
- Material del curs: [Guia de proves i documentació d'API](../../04_materials/repte_04/guia_proves_i_documentacio_api.md)
- MDN: [HTTP response status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
- MDN: [HTTP request methods](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods)
- FastAPI Docs: [Handling Errors](https://fastapi.tiangolo.com/tutorial/handling-errors/)
- NestJS Docs: [Exception filters](https://docs.nestjs.com/exception-filters)
