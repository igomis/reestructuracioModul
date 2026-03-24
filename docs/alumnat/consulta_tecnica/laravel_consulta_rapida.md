# Laravel: consulta ràpida

## Què és
És una guia curta per localitzar les peces de `Laravel` que més et fan falta en este curs. No vol substituir la documentació del framework: vol ajudar-te a entendre com encaixa `Laravel` amb els reptes i amb el teu projecte base.

## Quan la necessites en el curs
- en `R1`, per arrencar projecte i entendre el recorregut mínim
- en `R2`, per auth, validació i protecció de rutes o operacions
- en `R3`, per models, migracions i persistència
- en `R4`, per separar bé `web.php` i `api.php`

## Què has de saber sí o sí
- `routes/web.php` i `routes/api.php` no juguen el mateix paper
- un `Controller` coordina la petició; no hauria de contindre tota la lògica del negoci
- `Model` i `Eloquent` et servixen per persistir domini i relacions, no només per “fer CRUD”
- `Form Request` o validació equivalent et permeten separar millor comprovacions d'entrada
- `middleware` és útil per autenticació i control d'accés
- `migrations` formen part del model i de la traçabilitat del projecte

## Errors habituals
- barrejar rutes web i `API` sense criteri
- deixar controladors massa grans
- confiar-ho tot a scaffolding o paquets generats automàticament
- no entendre què fa el `middleware` o què està validant el `Form Request`
- tindre `.env` o base de dades “aparentment” configurats però no verificats

## On consultar-ho bé
- [Guia de bootstrap Laravel](../../04_materials/itineraris/laravel/guia_bootstrap_laravel.md)
- [Guia d'auth i persistència Laravel](../../04_materials/itineraris/laravel/guia_auth_i_persistencia_laravel.md)
- [Checklist de l'itinerari Laravel](../../04_materials/itineraris/laravel/checklist_itinerari_laravel.md)
- [Repte 3 per a alumnat](../reptes/repte_03.md)
