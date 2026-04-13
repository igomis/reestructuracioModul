# FastAPI: consulta ràpida

## Què és

És una guia curta per situar les peces clau de `FastAPI` dins del curs. En este repositori, `FastAPI` no es presenta com a itinerari base general: queda com a via avançada o excepcional.

## Quan la necessites en el curs

- només si el professorat t'ha autoritzat una via avançada
- en `R3`, per no confondre `schemas`, `models` i serveis
- en `R4`, per publicar `API` sobre una base clara i verificable
- en `R5`, per mantindre el mateix projecte en integració

## Què has de saber sí o sí

- `main.py` és el punt d'entrada, no el lloc on ha de viure tota la lògica
- `routers` definixen exposició HTTP
- `schemas` definixen validació i contracte, però no són necessàriament el model persistent
- `models` i la capa `db` sostenen la persistència del domini
- `services` o casos d'ús equivalents t'ajuden a no dissoldre el negoci dins del `router`

## Errors habituals

- posar tota la lògica dins dels `routers`
- confondre `schema` de validació amb model persistent
- tindre connexió a base de dades només aparent
- muntar `FastAPI` com una col·lecció d'endpoints sense arquitectura
- acceptar patrons d'IA sense provar si encaixen amb el projecte real

## Línia metodològica

- no és la via base general del curs
- no s'usa per substituir la base comuna de `R2`
- només té sentit si pots sostindre igualment autoria, traçabilitat i defensa individual

## On ampliar

- Material del curs: [Guia de bootstrap FastAPI](../../04_materials/itineraris/fastapi/guia_bootstrap_fastapi.md)
- Material del curs: [Guia d'auth i persistència FastAPI](../../04_materials/itineraris/fastapi/guia_auth_i_persistencia_fastapi.md)
- FastAPI Docs: [Bigger Applications](https://fastapi.tiangolo.com/tutorial/bigger-applications/)
- FastAPI Docs: [Request Body](https://fastapi.tiangolo.com/tutorial/body/)
- FastAPI Docs: [Security](https://fastapi.tiangolo.com/tutorial/security/)
- FastAPI Docs: [SQL Databases](https://fastapi.tiangolo.com/tutorial/sql-databases/)
