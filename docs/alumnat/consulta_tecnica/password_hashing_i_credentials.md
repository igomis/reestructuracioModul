# Password hashing i credencials

## Què és

És la part que convertix una contrasenya en una prova verificable sense guardar-la en text pla. També inclou com tractes usuaris, contrasenyes temporals i canvis de credencials sense fer atajos insegurs.

## Quan la necessites en el curs

- en `R2`, quan hi ha registre, `login` o canvi de contrasenya
- en `R3`, quan la persistència d'usuaris ja és estable
- en `R4`, si una `API` reutilitza credencials o identitats internes

## Què has de saber sí o sí

- una contrasenya no es guarda mai en text pla
- has d'usar funcions o llibreries de `hashing` pensades per a contrasenyes, no `sha256` manual
- el backend compara amb verificació de `hash`, no comparant text original
- si canvies l'algorisme o la configuració, has de saber quan rehashejar
- les credencials del projecte no s'han de barrejar amb credencials de proves o serveis externs

## Errors habituals

- guardar contrasenyes en text pla o amb `hash` inadequat
- reutilitzar la mateixa contrasenya per a usuaris de prova i serveis externs
- comparar contrasenyes abans de passar per la funció de verificació
- exposar contrasenyes de demo al repositori
- oblidar la caducitat o la invalidació quan resetejes credencials

## On ampliar

- Material del curs: [Apunts reals del Repte 2](../../04_materials/apunts_reals/repte_02_sessions_i_autenticacio.md)
- PHP Manual: [Password Hashing](https://www.php.net/manual/en/book.password.php)
- PHP Manual: [`password_hash`](https://www.php.net/manual/en/function.password-hash.php)
- PHP Manual: [`password_verify`](https://www.php.net/manual/en/function.password-verify.php)
- OWASP Cheat Sheet: [Password Storage](https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html)
- NestJS Docs: [Encryption and hashing](https://docs.nestjs.com/security/encryption-and-hashing)
