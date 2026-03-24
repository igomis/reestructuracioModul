# FastAPI: consulta ràpida

## Què és
És una guia curta per situar les peces clau de `FastAPI` dins del curs. La idea no és “fer endpoints ràpids”, sinó mantindre clara la separació entre contracte HTTP, validació, negoci i persistència.

## Quan la necessites en el curs
- en `R1`, per arrancar projecte i entendre l'estructura base
- en `R2`, per auth, dependències i protecció d'operacions
- en `R3`, per no confondre `schemas`, `models` i serveis
- en `R4`, per publicar `API` sobre una base clara i verificable

## Què has de saber sí o sí
- `main.py` és el punt d'entrada, no el lloc on ha de viure tota la lògica
- `routers` definixen exposició HTTP
- `schemas` definixen validació i contracte, però no són necessàriament el model persistent
- `models` i la capa `db` sostenen la persistència del domini
- `services` o casos d'ús equivalents t'ajuden a no dissoldre el negoci dins del `router`
- si uses dependències o ORM, has de poder explicar què resol cada peça

## Errors habituals
- posar tota la lògica dins dels `routers`
- confondre `schema` de validació amb model persistent
- tindre connexió a base de dades només aparent
- muntar `FastAPI` com una col·lecció d'endpoints sense arquitectura
- acceptar snippets o patrons d'IA sense provar si encaixen amb el projecte real

## On consultar-ho bé
- [Guia de bootstrap FastAPI](../../04_materials/itineraris/fastapi/guia_bootstrap_fastapi.md)
- [Guia d'auth i persistència FastAPI](../../04_materials/itineraris/fastapi/guia_auth_i_persistencia_fastapi.md)
- [Checklist de l'itinerari FastAPI](../../04_materials/itineraris/fastapi/checklist_itinerari_fastapi.md)
- [Repte 3 per a alumnat](../reptes/repte_03.md)
