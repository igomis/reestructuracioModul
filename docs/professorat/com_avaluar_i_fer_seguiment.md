# Com avaluar i fer seguiment

## Classificació documental

Este és un **document derivat**. Depén d'[Avaluació i evidències](../03_avaluacio/index.md) per al règim d'avaluació i d'[Ús de la IA per a professorat i alumnat](../us-ia-professorat-i-alumnat.md) per al criteri sobre ús assistit per IA i delegació excessiva.

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
- decisions tècniques registrades amb nota tècnica de decisió o equivalent
- `AI log` o rastre equivalent quan la IA haja tingut pes real

## Defensa tècnica

La defensa final no és una presentació ornamental. S'ha de poder revisar:

- explicació del codi
- justificació de decisions
- capacitat de detectar errors
- capacitat de fer canvis o localitzar punts crítics
- comprensió del paper real de la IA en el resultat

## Ús assistit per IA

Quan la IA haja intervingut de manera rellevant, el professorat no ha de reobrir criteri propi ací. Ha d'aplicar el document canònic [Ús de la IA per a professorat i alumnat](../us-ia-professorat-i-alumnat.md) i verificar rastre, comprensió, proves i defensa tècnica.

## Checkpoints mínims

- `CP0`: primer mapa provisional del producte, criteri de traçabilitat i preparació per acceptar GitHub Classroom
- `CP1`: repositori Classroom usable, `README` inicial, domini, base comuna en `PHP`, entorn funcional i primera decisió tècnica
- `CP2`: operació protegida o equivalent, validacions i errors mínims sobre la base comuna en `PHP`
- `CP3`: persistència coherent i arquitectura explicable
- `CP4`: `API` publicada, documentada i provada
- `CP5`: integració final, `AI log` tancat i defensa preparada

## Instruments que convé obrir

- [Guia d'avaluació automàtica dels microreptes](../03_avaluacio/guia_avaluacio_automatica_microreptes.md)
- [Rúbrica base dels reptes](../03_avaluacio/rubrica_base_reptes.md)
- [Rúbrica de defensa tècnica](../03_avaluacio/rubrica_defensa_tecnica.md)
- [Sistema d'evidències](../03_avaluacio/sistema_evidencies.md)
- [Instruments de seguiment docent](../03_avaluacio/instruments_seguiment_docent.md)

## Ús de l'autocorrecció dels microreptes

L'autocorrecció és un instrument de triatge i feedback, no una substitució de la decisió docent. Abans d'acceptar una nota provisional cal revisar si el microrepte corregit és el correcte, si les evidències són localitzables i si hi ha flags de baixa confiança, autoria dubtosa o absència de proves.

Per al flux complet de preparació, llançament, lectura de resultats i revisió manual, aplica la [Guia d'avaluació automàtica dels microreptes](../03_avaluacio/guia_avaluacio_automatica_microreptes.md).

## Criteri de seguiment

- revisar producte real abans que discurs
- registrar decisions docents breus en checkpoints o seguiment periòdic
- bloquejar el pas al repte següent si no hi ha evidència mínima individual
- mantindre la mateixa exigència en `Laravel`, `Symfony` i `NestJS`
- tractar `FastAPI` només com a via avançada o excepcional quan realment s'haja autoritzat
