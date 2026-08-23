# Repte 1. Kickoff funcional

## Què és el repte

És l'arrancada real del producte. Has de deixar una base backend executable, una primera resposta funcional mínima i documentació suficient perquè una altra persona puga entendre què has muntat i com provar-ho.

No és un repte de framework complet. El focus és entendre el model client/servidor, arrancar una base en `PHP` amb `Docker` i servidor web, completar l'entorn mínim i deixar evidències reals.

## Com s'organitza

El repte té `4` microreptes com a passos lògics:

- `Microrepte 1`: entendre client/servidor, diferenciar execució en client i servidor, i prendre una primera decisió tècnica
- `Microrepte 2`: muntar l'entorn executable
- `Microrepte 3`: construir la landing inicial servida pel backend
- `Microrepte 4`: documentar, verificar i preparar el checkpoint

En classe es treballa en `2` sessions principals:

- Sessió `1`: microrepte `1` + inici del microrepte `2`
- Sessió `2`: tancament del microrepte `2` + microrepte `3` + microrepte `4`

Pot haver-hi una sessió `3` opcional si cal fer defensa, checkpoint formal o revisió més forta d'evidències.

## Què has de fer

- explicar què s'executa al client web i què s'executa al servidor en el teu producte
- omplir la fitxa d'exploració tècnica inicial
- justificar una primera decisió tècnica orientativa
- iniciar i completar un entorn executable amb `Docker`, `PHP` i servidor web
- incorporar BBDD i phpMyAdmin si cal per deixar l'entorn complet del repte
- crear una primera pàgina, ruta, `endpoint` o `healthcheck` funcional
- escriure un `README` que permeta arrancar i comprovar el projecte
- crear un directori de documentació dins del repositori
- penjar les fitxes o documents del repte al repositori
- crear un índex o pàgina visible que enllace eixa documentació
- deixar traçabilitat mínima amb commits i, si toca, `AI log`

## Evidència mínima

- fitxa tècnica inicial
- explicació breu del model d'execució client vs servidor aplicada al teu producte
- repositori usable
- `docker-compose.yml` o equivalent funcional
- entorn que arranca
- landing inicial servida pel backend
- `README` executable
- documentació del repte organitzada dins del repositori
- justificació tècnica curta
- registre d'una decisió, incidència o dubte real

## Checkpoint

Has de poder explicar:

- quina part del teu producte s'executa al client i quina al servidor
- quin paper tindrà el backend
- com s'arranca el projecte
- què fa cada peça important de l'entorn
- quina és la primera funcionalitat mínima real
- on està la documentació del repte dins del repositori
- què has decidit i què queda pendent

## Què no és suficient

- deixar només una comparativa de tecnologies
- copiar una configuració de Docker sense entendre-la
- tindre contenidors que no pots provar
- fer només un `hello world` sense relació amb el projecte
- entregar un `README` que no permet arrancar el projecte
- tindre fitxes o documents fora del repositori i sense enllaç visible
- usar IA per generar solucions que no pots explicar ni modificar

## Connexió amb el següent pas

El que crees ací ha de servir perquè en `R2` pugues construir el primer flux funcional amb dades, lògica, estat o autenticació sobre una base comuna en `PHP`.

## Si vols el detall complet

Consulta [Repte 1. Kickoff funcional d'un servei web backend](../../02_reptes/repte_01_kickoff_backend.md), el [full de treball del Repte 1](../../08_materials_compartibles/full_treball_repte_01.md) i la [fitxa d'exploració tècnica inicial](../../08_materials_compartibles/fitxa_exploracio_tecnica_inicial.md).
