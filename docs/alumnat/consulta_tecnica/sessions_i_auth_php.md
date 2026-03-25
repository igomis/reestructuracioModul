# Sessions i auth en PHP

## Què és
És la versió pràctica de `login`, `logout`, control d'estat i restricció d'accés quan treballes en `PHP` sense un framework gran o quan vols entendre què fa realment el framework per tu.

## Quan la necessites en el curs
- sobretot en `R2`
- en `R3`, si estàs refactoritzant auth i permisos a una estructura més neta
- en `R4`, si conviu una part web amb una part `API`

## Què has de saber sí o sí
- `session_start()` ha d'estar ben situat i no és decoratiu
- l'usuari autenticat s'ha de guardar i llegir amb criteri des de `$_SESSION`
- el `logout` ha d'invalidar l'estat, no només redirigir
- després del `login` convé regenerar l'identificador de sessió
- la contrasenya s'ha de verificar amb `password_verify`, no comparant text

## Errors habituals
- oblidar arrancar la sessió abans d'usar-la
- guardar massa informació sensible dins de la sessió
- no invalidar la sessió en `logout`
- no regenerar l'ID de sessió després d'autenticar
- confiar en un camp ocult o una cookie pròpia com si fora auth completa

## On ampliar
- Material del curs: [Guia de flux d'usuari i sessions](../../04_materials/repte_02/guia_flux_usuari_i_sessions.md)
- Material del curs: [Apunts reals del Repte 2](../../04_materials/apunts_reals/repte_02_sessions_i_autenticacio.md)
- PHP Manual: [Sessions](https://www.php.net/manual/en/book.session.php)
- PHP Manual: [`session_regenerate_id`](https://www.php.net/manual/en/function.session-regenerate-id.php)
- PHP Manual: [`password_verify`](https://www.php.net/manual/en/function.password-verify.php)
- MDN: [HTTP cookies](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies)
