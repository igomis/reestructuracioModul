# Tokens útils en backend

## Què és

En este curs, un token és un mecanisme funcional del backend per confirmar, cancel·lar, convidar, traçar o donar accés limitat a una operació concreta. No és un tema obligatori de `JWT` ni de `web3`.

## Quan la necessites en el curs

- quan el teu projecte base ja demana un flux tokenitzat útil
- sobretot en `R4`, quan publiques una operació com a `API`
- sobretot en `R5`, quan reutilitzes eixe flux en integració o notificació externa

## Què has de saber sí o sí

- un token útil ha d'estar lligat a una operació, reserva, incidència o recurs concret
- el seu abast ha de ser limitat: què permet fer, durant quant de temps i quantes vegades
- la caducitat, el consum únic i la traçabilitat no són extres
- un token funcional del domini no és el mateix que un mecanisme general d'autenticació
- has de poder explicar qui crea el token, qui el valida i què passa quan caduca

## Errors habituals

- afegir tokens perquè sona pro però sense cap necessitat funcional
- crear tokens sense caducitat ni restricció d'ús
- donar massa permisos a un canal extern tokenitzat
- confondre tokenització funcional amb autenticació completa
- no registrar qui crea, valida o consumix el token

## On ampliar

- Material del curs: [Integració API](../../05_projectes_tecnics/integracio_api.md)
- Material del curs: [Repte 5. Integració híbrida i tancament](../../02_reptes/repte_05_integracio_hibrida_n8n.md)
- MDN: [Authorization header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Authorization)
- RFC Editor: [RFC 7519 JSON Web Token](https://www.rfc-editor.org/rfc/rfc7519)
- Laravel Docs: [Sanctum](https://laravel.com/docs/13.x/sanctum)
- FastAPI Docs: [OAuth2 with Password and Bearer](https://fastapi.tiangolo.com/tutorial/security/oauth2-jwt/)
