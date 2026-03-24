# Cookies, sessions i estat

## Què és
És la part que permet que el backend sàpia si una persona usuària ja està autenticada, quin context manté i quan eixe estat deixa de ser vàlid. En el curs això no és teoria de navegador: és infraestructura perquè el producte puga controlar accés real.

## Quan la necessites en el curs
- sobretot en `R2`, quan obris registre, login, logout i operació protegida
- en `R4`, si l'`API` manté autenticació o exigeix capçalera, sessió o mecanisme equivalent
- en `R5`, quan una integració necessita saber com s'autoritza el consum d'`API`

## Què has de saber sí o sí
- autenticació, sessió i autorització no són el mateix
- la sessió o l'estat s'ha de validar al servidor, no només a la interfície
- el `logout` o invalidació equivalent forma part del flux, no és un detall opcional
- si el teu backend és més `API` que web, el “manteniment d'estat” pot ser via token o capçalera, però igualment has d'explicar com es comprova
- el que importa és que una operació real del domini quede protegida i siga verificable

## Errors habituals
- tindre login aparent però cap operació realment protegida
- confiar en una variable del client com si fóra control d'accés
- no comprovar què passa després del `logout`
- barrejar lògica de permisos amb lògica de sessió sense distingir-les
- no documentar com es reproduïx el flux complet d'estat

## On consultar-ho bé
- [Repte 2. Sessions, autenticació i primera funcionalitat](../../02_reptes/repte_02_sessions_i_autenticacio.md)
- [Apunts reals del Repte 2](../../04_materials/apunts_reals/repte_02_sessions_i_autenticacio.md)
- [Guia de flux d'usuari i sessions](../../04_materials/repte_02/guia_flux_usuari_i_sessions.md)
- [Repte 2 per a alumnat](../reptes/repte_02.md)
