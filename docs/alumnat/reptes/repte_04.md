# Repte 4. API i consum

## Què és el repte
És el pas de backend usable per a l'equip a backend publicable i consumible per tercers. Has de convertir casos d'ús reals del producte en una API clara, provada i documentada.

## Què no és suficient
- obrir rutes soltes
- generar `Swagger` o JSON sense contracte real
- documentació que no coincideix amb el codi
- consum fictici o només descrit

## Mínim funcional no trivial
- endpoints prioritaris lligats a casos d'ús reals
- validació d'entrada i codis d'estat coherents
- errors d'API comprensibles
- documentació operativa d'API
- una prova real de consum amb client, script o eina equivalent

## Evidència mínima
- documentació d'API usable
- col·lecció de proves o script de consum
- casos correctes i casos d'error verificats
- commits i documentació del procés
- prova que productor i consumidor parlen el mateix contracte

## Errors habituals
- exposar una API ornamental
- oblidar autenticació o permisos en endpoints sensibles
- no provar errors ni dades invàlides
- documentar una cosa i retornar-ne una altra
- donar per bo un consum que només funciona de manera manual o parcial

## Connexió amb el següent pas
En `R5`, esta API passa a formar part d'un flux híbrid o automatitzat. Si el contracte no està clar, la integració final es trenca.

## Si vols el detall complet
Consulta [Repte 4. Publicació i consum d'API](../../02_reptes/repte_04_api_i_consum.md).
