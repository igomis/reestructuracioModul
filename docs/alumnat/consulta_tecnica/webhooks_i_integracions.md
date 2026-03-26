# Webhooks i integracions

## Què és

És la part del curs on el teu backend deixa de ser un sistema tancat i comença a reaccionar a events o a enviar informació a un altre servei. En `R5` això només té sentit si resol un flux útil del producte.

## Quan la necessites en el curs

- sobretot en `R5`
- després d'haver tancat una `API` clara en `R4`
- quan el producte necessita notificació, sincronització o automatització externa

## Què has de saber sí o sí

- un `webhook` és una entrada HTTP que rep events d'un sistema extern
- una integració ha de tindre clar origen, payload, autenticació, resposta i traçabilitat
- si el servei extern falla, has de saber què passa i com ho detectes
- no convé duplicar lògica de negoci en `n8n` o en el consumidor extern
- necessites una prova mínima del flux correcte i una d'error

## Errors habituals

- muntar una integració sense cas d'ús real
- no validar la firma, el token o la capçalera del `webhook`
- assumir que el payload extern sempre vindrà complet i ben format
- no controlar reintents, duplicats o errors temporals
- no deixar export o rastre reproduïble del flux

## On ampliar

- Material del curs: [Repte 5. Integració híbrida i tancament](../../02_reptes/repte_05_integracio_hibrida_n8n.md)
- Material del curs: [Guia d'integració externa i flux híbrid](../../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md)
- n8n Docs: [Webhook node](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.webhook/)
- n8n Docs: [Error handling](https://docs.n8n.io/flow-logic/error-handling/)
- GitHub Docs: [Webhooks](https://docs.github.com/en/webhooks)
- MDN: [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CORS)
