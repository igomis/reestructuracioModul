# Migracions i canvis de dades

## Què és

És la manera controlada de fer evolucionar l'esquema o les dades del projecte sense tocar la base de dades a mà cada vegada. En el curs és la traça que demostra que saps com ha canviat el model.

## Quan la necessites en el curs

- sobretot en `R3`, quan el model persistent deixa de ser provisional
- en `R4`, quan l'`API` depén d'un esquema estable
- en `R5`, quan una integració externa ja espera certes taules, camps o estats

## Què has de saber sí o sí

- una migració ha de correspondre a un canvi real del model, no a canvis aleatoris
- abans de migrar has de saber què passa amb les dades que ja existixen
- canviar noms, restriccions o relacions pot trencar fluxos ja fets
- si el teu stack usa ferramenta de migracions, has de saber crear-la, aplicar-la i explicar-la
- el `README` ha d'indicar com alçar la base de dades del projecte

## Errors habituals

- editar la base de dades a mà i no deixar rastre
- acumular canvis sense saber quin estat és el bo
- afegir camps nous sense pensar valors per a dades antigues
- canviar relacions i no provar els fluxos ja persistits
- fer una migració generada i no llegir què farà realment

## On ampliar

- Material del curs: [Repte 3. Reconstrucció en framework i persistència real](../../02_reptes/repte_03_mvc_i_persistencia.md)
- Material del curs: [Guia de persistència i modelat de dades](../../04_materials/repte_03/guia_persistencia_i_modelat_dades.md)
- Laravel Docs: [Migrations](https://laravel.com/docs/13.x/migrations)
- Alembic Docs: [Tutorial](https://alembic.sqlalchemy.org/en/latest/tutorial.html)
- Prisma Docs: [Prisma Migrate](https://www.prisma.io/docs/orm/prisma-migrate)
- NestJS Docs: [Database](https://docs.nestjs.com/techniques/database)
