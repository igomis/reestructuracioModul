# Formularis i validació

## Què és
És la capa que convertix una entrada del producte en una dada usable de veritat. Al curs no compta només tindre una pantalla o un camp: compta que el servidor reba la informació, la valide i la tracte amb criteri mínim.

## Quan la necessites en el curs
- en `R1`, per obrir la primera entrada funcional del producte
- en `R2`, per alta, login i primera operació de negoci protegida
- en `R3`, per lligar validació amb model i persistència
- en `R4`, quan una entrada passa a formar part del contracte d'`API`

## Què has de saber sí o sí
- la validació important és la del servidor, encara que també valides al client
- un formulari del curs ha d'estar lligat a un cas d'ús real del projecte, no a una pantalla ornamental
- no és el mateix validar camps obligatoris que validar una regla de negoci
- has de poder mostrar almenys un cas correcte i un cas incorrecte
- les respostes d'error han de ser comprensibles per provar i depurar

Exemples alineats amb els projectes base:
- inventari: no permetre una eixida si falta l'identificador del recurs o la quantitat és incoherent
- reserves: no acceptar una reserva si falta la franja o hi ha conflicte temporal bàsic
- incidències: no acceptar una alta si no hi ha descripció mínima o context suficient

## Errors habituals
- validar només al client i confiar que el backend “ja ho arreglarà”
- resoldre només el cas feliç
- crear diversos formularis buits en lloc d'un flux útil
- donar per bona una entrada perquè “guarda dades” però sense missatge clar en error
- copiar validacions suggerides per IA sense provar quins casos fallen de veritat

## On consultar-ho bé
- [Repte 1. Kickoff funcional](../../02_reptes/repte_01_kickoff_backend.md)
- [Repte 2. Sessions, autenticació i primera funcionalitat](../../02_reptes/repte_02_sessions_i_autenticacio.md)
- [Apunts reals del Repte 2](../../04_materials/apunts_reals/repte_02_sessions_i_autenticacio.md)
- [Guia de validació i errors de servidor](../../04_materials/repte_02/guia_validacio_i_errors_servidor.md)
