# Com avaluar i fer seguiment

## Principi general

L'avaluació continua sent individual, encara que hi puga haver contextos de projecte compartit o contrast tècnic coordinat. El criteri és si cada alumne pot traçar, reproduir, explicar i defensar la seua part.

## Què es valora realment

- progrés del producte al llarg dels reptes
- coherència entre repte, evidència i documentació
- qualitat mínima de validació, proves, errors i traçabilitat
- capacitat d'explicar decisions i modificar el codi
- ús verificable de la IA quan haja intervingut

## Evidències que han d'aparéixer

- repositori actiu i usable
- `README` actualitzat segons el moment del curs
- funcionalitat executable del repte actual
- proves mínimes o passos reproduïbles
- decisions tècniques registrades amb `ADR` o equivalent
- `AI log` o rastre equivalent quan la IA haja tingut pes real

## Defensa tècnica

La defensa final no és una presentació ornamental. S'ha de poder revisar:

- explicació del codi
- justificació de decisions
- capacitat de detectar errors
- capacitat de fer canvis o localitzar punts crítics
- comprensió del paper real de la IA en el resultat

## IA verificable

Es pot usar IA per contrastar, desbloquejar, accelerar o explorar opcions. No és acceptable:

- lliurar codi que no es pot explicar
- presentar com a pròpia una decisió no compresa
- usar IA per substituir proves, verificació o criteri tècnic

El professorat ha de demanar rastre mínim i preguntes de contrast quan detecte ús rellevant de la IA.

## Checkpoints mínims

- `CP0`: repositori usable, `README` inicial i criteri de traçabilitat
- `CP1`: domini, base comuna en `PHP`, entorn funcional i primera decisió tècnica
- `CP2`: operació protegida o equivalent, validacions i errors mínims sobre la base comuna en `PHP`
- `CP3`: persistència coherent i arquitectura explicable
- `CP4`: `API` publicada, documentada i provada
- `CP5`: integració final, `AI log` tancat i defensa preparada

## Instruments que convé obrir

- [Rúbrica base dels reptes](../03_avaluacio/rubrica_base_reptes.md)
- [Rúbrica de defensa tècnica](../03_avaluacio/rubrica_defensa_tecnica.md)
- [Sistema d'evidències](../03_avaluacio/sistema_evidencies.md)
- [Instruments de seguiment docent](../03_avaluacio/instruments_seguiment_docent.md)

## Criteri de seguiment

- revisar producte real abans que discurs
- registrar decisions docents breus en checkpoints o seguiment periòdic
- bloquejar el pas al repte següent si no hi ha evidència mínima individual
- mantindre la mateixa exigència en `Laravel`, `Symfony` i `NestJS`
- tractar `FastAPI` només com a via avançada o excepcional quan realment s'haja autoritzat
