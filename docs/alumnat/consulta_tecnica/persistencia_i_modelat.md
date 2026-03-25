# Persistència i modelat

## Què és
És el pas de dades provisionals o massa acoblades a un model de domini persistent i explicable. En el curs no compta només guardar a base de dades: compta que el model sostinga una funcionalitat real del producte.

## Quan la necessites en el curs
- ja en `R1`, per entendre què registres encara que siga de manera bàsica
- sobretot en `R3`, on passa a ser el nucli del repte
- en `R4`, perquè una `API` estable necessita model i persistència coherents

## Què has de saber sí o sí
- comença per una entitat principal i un cas d'ús clar
- modelar no és fer totes les taules possibles; és triar quines dades sostenen el flux principal
- persistència i validació han d'anar lligades al domini
- necessites identificadors clars, restriccions bàsiques i coherència en lectures i escriptures
- les migracions o mecanismes equivalents formen part de la traçabilitat tècnica

## Errors habituals
- crear base de dades abans de tindre clar el cas d'ús
- modelar moltes entitats però no poder demostrar una operació de punta a punta
- barrejar entrada, lògica i persistència al mateix controlador o `router`
- tindre persistència aparent però continuar depenent d'estat temporal
- fer canvis d'esquema sense cap rastre ni explicació

## On ampliar
- Material del curs: [Repte 3. Migració a MVC i persistència segura](../../02_reptes/repte_03_mvc_i_persistencia.md)
- Material del curs: [Guia de persistència i modelat de dades](../../04_materials/repte_03/guia_persistencia_i_modelat_dades.md)
- Laravel Docs: [Eloquent ORM](https://laravel.com/docs/13.x/eloquent)
- Laravel Docs: [Migrations](https://laravel.com/docs/13.x/migrations)
- FastAPI Docs: [SQL Databases](https://fastapi.tiangolo.com/tutorial/sql-databases/)
- NestJS Docs: [Database](https://docs.nestjs.com/techniques/database)
