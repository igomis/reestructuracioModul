# Proves i debugging

## Què és
És la capa de verificació mínima del curs. No es tracta de fer un sistema enorme de tests des del primer dia, sinó de deixar evidència reproduïble que allò que dius que funciona realment funciona, i de saber localitzar on falla quan no funciona.

## Quan la necessites en el curs
- en `R1`, per provar arrencada, formulari i primer registre
- en `R2`, per casos correctes, errors i accés denegat
- en `R3`, per regressió i persistència
- en `R4`, per contracte, errors i consum d'`API`
- en `R5`, per flux complet, incidències i integració externa

## Què has de saber sí o sí
- cada repte ha de deixar almenys una prova o verificació clara i reproduïble
- cal provar tant el camí correcte com una fallada rellevant
- el `README` ha d'explicar com reproduir el que afirmes
- depurar no és tocar coses a cegues; és reproduir, observar, aïllar i corregir
- si uses IA per trobar solucions o errors, has de contrastar el resultat abans d'acceptar-lo

Formats vàlids segons el moment:
- prova automatitzada bàsica
- col·lecció de peticions o `curl`
- registre manual curt però reproduïble
- workflow exportat i revisió guiada en `R5`

## Errors habituals
- considerar suficient una captura o un vídeo
- no provar casos d'error
- deixar el debugging només en memòria i no actualitzar el `README`
- arreglar símptomes sense entendre la causa
- acceptar correccions suggerides per IA sense verificar el comportament real del repositori

## On consultar-ho bé
- [Guia de testing i debugging](../../04_materials/materials_comuns/guia_testing_i_debugging.md)
- [Guia de proves i documentació d'API](../../04_materials/repte_04/guia_proves_i_documentacio_api.md)
- [Apunts reals del Repte 3](../../04_materials/apunts_reals/repte_03_mvc_i_persistencia.md)
- [Apunts reals del Repte 4](../../04_materials/apunts_reals/repte_04_api_i_consum.md)
