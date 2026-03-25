# Formularis i validació

## Què és
És la capa que convertix una entrada del producte en una dada usable de veritat. En el curs no compta només tindre una pantalla o un `JSON`: compta que el servidor reba la informació, la valide i la tracte amb criteri mínim.

## Quan la necessites en el curs
- en `R1`, per obrir la primera entrada funcional del producte
- en `R2`, per alta, `login` i primera operació protegida
- en `R3`, per lligar validació amb model i persistència
- en `R4`, quan una entrada passa a formar part del contracte d'`API`

## Què has de saber sí o sí
- la validació important és la del servidor, encara que també valides al client
- no és el mateix validar camps obligatoris que validar una regla de negoci
- has de poder mostrar almenys un cas correcte i un cas incorrecte
- l'error ha de tornar de manera clara perquè el pugues provar i depurar
- la validació ha d'estar connectada amb un cas d'ús real del projecte

## Errors habituals
- validar només al client i confiar que el backend ja ho arreglarà
- resoldre només el cas feliç
- fer diversos formularis buits en lloc d'un flux útil
- acceptar dades incoherents perquè la base de dades les guarda igual
- copiar validacions suggerides per IA sense provar casos límit

## On ampliar
- Material del curs: [Repte 1. Kickoff funcional](../../02_reptes/repte_01_kickoff_backend.md)
- Material del curs: [Guia de validació i errors de servidor](../../04_materials/repte_02/guia_validacio_i_errors_servidor.md)
- MDN: [Client-side form validation](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms/Form_validation)
- Laravel Docs: [Validation](https://laravel.com/docs/13.x/validation)
- FastAPI Docs: [Request Body](https://fastapi.tiangolo.com/tutorial/body/)
- NestJS Docs: [Validation](https://docs.nestjs.com/techniques/validation)
