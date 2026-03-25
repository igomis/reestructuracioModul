# APIs i contracte

## Què és
És la part del curs on una funcionalitat real del producte deixa de ser només interna i passa a tindre una interfície clara per a tercers. El contracte d'`API` és el pacte entre el teu backend i qui el consumix.

## Quan la necessites en el curs
- al final de `R3`, quan ja has de decidir quina part del producte publicaràs
- en `R4`, com a nucli del repte
- en `R5`, quan la integració reutilitza eixe contracte

## Què has de saber sí o sí
- una `API` útil naix d'un cas d'ús real, no d'un `CRUD` arbitari
- el contracte inclou entrada, eixida, errors, autenticació i condicions d'ús
- has de tindre com a mínim una prova correcta i una prova d'error
- la documentació ha de coincidir amb el comportament real del backend
- el consum ha de ser reproduïble: `curl`, col·lecció, script o client simple

## Errors habituals
- exposar massa endpoints sense prioritzar el flux principal
- documentar una cosa i retornar-ne una altra
- provar només el cas feliç
- oblidar permisos o autenticació en endpoints sensibles
- considerar consum una crida manual aïllada sense rastre reutilitzable

## On ampliar
- Material del curs: [Repte 4. Publicació i consum d'API](../../02_reptes/repte_04_api_i_consum.md)
- Material del curs: [Guia de contracte i disseny d'API](../../04_materials/repte_04/guia_contracte_i_disseny_api.md)
- MDN: [HTTP request methods](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods)
- MDN: [HTTP status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
- FastAPI Docs: [Handling Errors](https://fastapi.tiangolo.com/tutorial/handling-errors/)
- NestJS Docs: [Controllers](https://docs.nestjs.com/controllers)
