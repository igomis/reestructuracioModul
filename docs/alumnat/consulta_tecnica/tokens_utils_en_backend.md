# Tokens útils en backend

## Què és
En este curs, un token és un mecanisme funcional del backend per confirmar, cancel·lar, convidar, traçar o donar accés limitat a una operació concreta. No és una línia `web3` obligatòria ni un tema de criptomonedes.

## Quan la necessites en el curs
- quan el teu projecte base ja demana un flux tokenitzat útil
- sobretot en `R4`, quan publiques una operació com a `API`
- sobretot en `R5`, quan reutilitzes eixe flux en integració o notificació externa

## Què has de saber sí o sí
- un token útil ha d'estar lligat a una operació, reserva, incidència o recurs concret
- el seu abast ha de ser limitat: què permet fer, durant quant de temps i quantes vegades
- la caducitat, el consum únic i la traçabilitat no són extres; formen part del disseny mínim
- el token ha d'aportar valor al flux de negoci, no només “fer-lo més avançat”
- un token d'operació, confirmació o invitació no és el mateix que un mecanisme general d'autenticació

Exemples del curs:
- inventari: token d'operació per tancar una entrega o transferència
- reserves: token de confirmació o cancel·lació d'una reserva concreta
- incidències: token d'invitació o seguiment extern limitat

## Errors habituals
- afegir tokens perquè “sona pro” però sense cap necessitat funcional
- crear tokens sense caducitat ni restricció d'ús
- donar massa permisos a un canal extern tokenitzat
- confondre tokenització funcional de backend amb una exigència `web3`
- no registrar qui crea, valida o consumix el token

## On consultar-ho bé
- [Projectes base concretats](../../05_projectes_tecnics/projectes_base_concretats.md)
- [Integració API](../../05_projectes_tecnics/integracio_api.md)
- [Repte 4. API i consum](../../02_reptes/repte_04_api_i_consum.md)
- [Repte 5. Integració híbrida i tancament](../../02_reptes/repte_05_integracio_hibrida_n8n.md)
