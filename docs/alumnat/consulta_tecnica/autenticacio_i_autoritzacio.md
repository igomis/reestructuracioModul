# Autenticació i autorització

## Què és

Autenticació és demostrar qui eres. Autorització és decidir què pots fer. En el curs les dos coses només tenen valor si protegixen una operació real del producte.

## Quan la necessites en el curs

- en `R2`, com a nucli del primer flux de negoci protegit
- en `R3`, quan rols, restriccions i persistència han de quedar coherents
- en `R4`, quan exposes endpoints que no pot usar qualsevol actor

## Què has de saber sí o sí

- no n'hi ha prou amb fer `login`; has de protegir una acció amb sentit de negoci
- necessites com a mínim un actor clar i una operació que puga ser denegada
- els permisos han d'estar lligats al domini, no a un rol inventat sense ús
- l'autorització s'ha de comprovar al servidor
- has de poder ensenyar un cas correcte i un cas denegat

## Errors habituals

- confondre autenticació amb autorització
- fer un rol `admin` sense cap justificació funcional
- protegir pantalles, però no la lògica real del backend
- no provar accessos denegats
- generar esquelets d'auth i no saber què comproven de veritat

## On ampliar

- Material del curs: [Repte 2. Sessions, autenticació i primera funcionalitat](../../02_reptes/repte_02_sessions_i_autenticacio.md)
- Material del curs: [Apunts reals del Repte 2](../../04_materials/apunts_reals/repte_02_sessions_i_autenticacio.md)
- Laravel Docs: [Authentication](https://laravel.com/docs/13.x/authentication)
- Laravel Docs: [Authorization](https://laravel.com/docs/13.x/authorization)
- FastAPI Docs: [Security](https://fastapi.tiangolo.com/tutorial/security/)
- NestJS Docs: [Authentication](https://docs.nestjs.com/security/authentication)
