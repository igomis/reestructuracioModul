# ORM i consulta de dades

## Què és
És la capa que et permet llegir i escriure dades amb objectes, models o repositoris en lloc d'omplir el projecte de SQL dispers. En el curs t'ajuda si manté el domini clar; no si amaga què està passant.

## Quan la necessites en el curs
- sobretot en `R3`, quan el model persistent passa a ser central
- en `R4`, quan l'`API` ha de consultar i retornar dades amb criteri
- en `R5`, quan una integració externa depén de lectures estables del domini

## Què has de saber sí o sí
- un ORM no et lleva l'obligació d'entendre taules, claus i relacions
- has de saber quina consulta fa cada operació important del producte
- model i consulta han d'anar lligats a un cas d'ús real
- les relacions i filtres han d'evitar lectures absurdes o massa pesades
- si una consulta és crítica, has de poder explicar-la encara que la genere el framework

## Errors habituals
- usar l'ORM com si fora màgia i no saber d'on ixen les dades
- fer `findAll` o equivalent i filtrar després en memòria
- omplir el controlador de consultes repetides
- no revisar relacions, càrrega de dades o selecció de camps
- confondre model de validació amb model persistent

## On ampliar
- Material del curs: [Guia de persistència i modelat de dades](../../04_materials/repte_03/guia_persistencia_i_modelat_dades.md)
- Material del curs: [Guia de refactorització MVC o equivalent](../../04_materials/repte_03/guia_refactoritzacio_mvc_o_equivalent.md)
- Laravel Docs: [Eloquent ORM](https://laravel.com/docs/13.x/eloquent)
- Laravel Docs: [Eloquent Relationships](https://laravel.com/docs/13.x/eloquent-relationships)
- SQLAlchemy Docs: [ORM Quick Start](https://docs.sqlalchemy.org/en/20/orm/quickstart.html)
- Prisma Docs: [CRUD queries](https://www.prisma.io/docs/orm/prisma-client/queries/crud)
