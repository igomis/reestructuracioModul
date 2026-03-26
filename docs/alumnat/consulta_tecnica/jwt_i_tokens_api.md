# JWT i tokens d'API

## Què és

És la part de l'autenticació d'`API` on una petició porta una credencial en capçalera en lloc de dependre d'una sessió clàssica. `JWT` és un format possible, però no sempre és la millor opció per al teu cas del curs.

## Quan la necessites en el curs

- en `R4`, si publiques una `API` que no depén d'una sessió web
- en `R5`, si una integració externa necessita autenticar-se contra la teua `API`
- quan has de distingir clarament entre token d'auth i token funcional del domini

## Què has de saber sí o sí

- un `Bearer token` viatja normalment en la capçalera `Authorization`
- `JWT` no és màgia: has d'entendre emissió, expiració, validació i revocació o equivalent
- si no tens un motiu clar per a `JWT`, potser et convé més un token opac o una solució del framework
- el backend ha de comprovar signatura o validesa abans d'executar l'operació
- has de saber quins endpoints exigixen token i quins no

## Errors habituals

- usar `JWT` perquè sembla més avançat encara que una sessió o un token simple era suficient
- guardar massa informació sensible dins del token
- no controlar expiració, rotació o invalidació
- acceptar qualsevol token ben format sense validar-lo
- confondre token d'autenticació amb token de confirmació d'una operació

## On ampliar

- Material del curs: [Repte 4. Publicació i consum d'API](../../02_reptes/repte_04_api_i_consum.md)
- Material del curs: [Integració API](../../05_projectes_tecnics/integracio_api.md)
- RFC Editor: [RFC 7519 JSON Web Token](https://www.rfc-editor.org/rfc/rfc7519)
- MDN: [Authorization header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Authorization)
- FastAPI Docs: [OAuth2 with Password and Bearer](https://fastapi.tiangolo.com/tutorial/security/oauth2-jwt/)
- Laravel Docs: [Sanctum](https://laravel.com/docs/13.x/sanctum)
