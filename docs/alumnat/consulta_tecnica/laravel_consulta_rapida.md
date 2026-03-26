# Laravel: consulta ràpida

## Què és

És una guia curta per localitzar les peces de `Laravel` que més et fan falta en este curs. No substituïx la documentació del framework: t'ajuda a entendre com encaixa `Laravel` amb els reptes i amb el teu projecte base.

## Quan la necessites en el curs

- en `R1`, per arrencar projecte i entendre el recorregut mínim
- en `R2`, per auth, validació i protecció de rutes o operacions
- en `R3`, per models, migracions i persistència
- en `R4`, per separar bé `web.php` i `api.php`

## Què has de saber sí o sí

- `routes/web.php` i `routes/api.php` no juguen el mateix paper
- un `Controller` coordina la petició; no hauria de contindre tota la lògica del negoci
- `Eloquent` et servix per persistir domini i relacions, no només per fer `CRUD`
- `middleware` i `Form Request` t'ajuden a separar auth, permisos i validació
- les `migrations` formen part del model i de la traçabilitat del projecte

## Errors habituals

- barrejar rutes web i `API` sense criteri
- deixar controladors massa grans
- confiar-ho tot a `scaffolding` o paquets generats automàticament
- no entendre què fa el `middleware` o què està validant el `Form Request`
- tindre `.env` o base de dades aparentment configurats però no verificats

## On ampliar

- Material del curs: [Guia de bootstrap Laravel](../../04_materials/itineraris/laravel/guia_bootstrap_laravel.md)
- Material del curs: [Guia d'auth i persistència Laravel](../../04_materials/itineraris/laravel/guia_auth_i_persistencia_laravel.md)
- Laravel Docs: [HTTP Requests](https://laravel.com/docs/13.x/requests)
- Laravel Docs: [Validation](https://laravel.com/docs/13.x/validation)
- Laravel Docs: [Authentication](https://laravel.com/docs/13.x/authentication)
- Laravel Docs: [Eloquent ORM](https://laravel.com/docs/13.x/eloquent)
