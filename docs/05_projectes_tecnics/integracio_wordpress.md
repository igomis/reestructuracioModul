# Integració WordPress

## Objectiu

Incorporar WordPress com a plataforma externa o complementària dins del projecte backend del curs, com a punt d'ampliació o integració dins del Repte 5. WordPress s'entén com a sistema extern integrat, no com a nucli del desenvolupament del producte.

## Ubicació recomanada

- Repte 5 (integració híbrida) com a ubicació principal
- connexió secundària amb Repte 4 si cal tractar API, autenticació o contracte de servei

## Casos d’ús suggerits

- consumir la REST API de WordPress des del backend propi
- publicar continguts des del backend cap a WordPress (sites, posts, tipus de contingut personalitzats)
- sincronitzar continguts, usuaris o metadades entre producte i WordPress
- usar WordPress com a backend de continguts complementari (headless CMS per determinats recursos)
- integrar WordPress dins d’un flux d’automatització o webhook
- ampliar un WordPress existent amb connectors o plugins que actuen com a sistema satèl·lit del producte principal

## Paper de la IA

La IA pot ajudar a:

- entendre l’estructura de la REST API i exemples de payload
- generar esquelets de connectors o scripts d’integració
- revisar payloads, mecanismes d’autenticació i gestió d’errors
- redactar documentació operativa i casos de prova

L’alumnat ha d’especificar, provar i defensar la integració implementada; l’ús d’IA ha d’estar registrat i justificat.

## Evidències (alineades amb el sistema del curs)

- repositori individual o traça equivalent amb branca o commits identificables
- commits o historial verificable del connector / adaptador
- prova reproduïble de la integració (scripts, Postman collection, demo enregistrada)
- documentació operativa (README tècnic, instruccions de desplegament, mapping de dades)
- AI log quan corresponga
- defensa tècnica individual sobre decisions, contracte i tractament d’errors

## Criteris de qualitat

- contracte clar entre sistemes (endpoints, models, SLA/expectatives)
- autenticació i autorització ben resoltes (tokens, claus, OAuth segons cas)
- tractament d’errors i estratègies de reintents o conciliació
- proves de la integració (unitàries/integradors o scripts de validació)
- documentació suficient per reproduir la integració
- justificació tècnica de per què WordPress és adequat o no per al cas

## Risc didàctic

El valor formatiu no està en “muntar una web amb WordPress”, sinó en integrar, automatitzar, comparar i justificar decisions tècniques sobre un sistema real. Evitar que la integració sigui només una demostració superficial.
