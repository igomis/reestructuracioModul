# Revisió transversal dels apunts reals R2-R5

## Finalitat del document

Deixar constància de la revisió transversal aplicada a la sèrie d'apunts reals dels Reptes `2-5` perquè funcionen com un paquet docent coherent, progressiu i usable en aula, sense lectures trivials ni salts de criteri entre un repte i el següent.

## Apunts revisats

- `repte_02_sessions_i_autenticacio.md`
- `repte_03_mvc_i_persistencia.md`
- `repte_04_api_i_consum.md`
- `repte_05_integracio_hibrida_n8n.md`

## Estructura comuna exigida

Tots els apunts reals de la sèrie han de compartir, com a mínim, esta estructura pública:

- `Finalitat del document`
- `Què sap ja l'alumnat`
- `Què s'ha de recordar breument`
- `Què ha d'explicar el professorat`
- `Què s'ha de modelar en directe`
- `Què treballa l'alumnat amb autonomia`
- `Exemple mínim orientatiu`
- `Errors habituals`
- `Com es verifica que funciona`
- `Evidències que s'han d'entregar`
- `Checklist final del repte`
- `Connexió amb el repte següent o amb la defensa final`

## Incoherències detectades

- `R2` podia continuar llegint-se massa prop d'un apunt de login o de control de sessió si no s'explicitava millor la funcionalitat de negoci autenticada.
- `R4` estava ben orientat a contracte i consum, però convenia reforçar la dimensió de defensa del cas d'ús publicat i no només la part tècnica d'endpoint.
- `R5` ja tenia bon nivell de tancament, però calia mantindre la mateixa lectura operativa que en `R3-R4`: flux real del producte, no eina o demo.
- la sèrie necessitava una terminologia més estable per repetir sempre el mateix patró docent: cas d'ús real, verificació, evidències, `README`, `AI log`, defensa.

## Ajustos aplicats

- s'ha reforçat a `R2` que el repte no és "fer login", sinó resoldre una funcionalitat de negoci autenticada amb restricció o regla recognoscible.
- s'ha deixat més explícit a `R3` que el repte no és "fer MVC" ni "guardar dades", sinó professionalitzar una funcionalitat real del producte.
- s'ha mantingut a `R4` que el repte no és "fer endpoints" ni un `CRUD` ornamental, sinó exposar una part usable del producte com a `API`.
- s'ha mantingut a `R5` que el repte no és "usar n8n", sinó resoldre una necessitat real del producte amb integració i automatització defensables.
- s'ha revisat la progressió de transició perquè cada apunt deixe preparada la lectura del següent.

## Terminologia unificada

Terminologia que convé mantindre estable en tota la sèrie:

- `funcionalitat real del producte`
- `cas d'ús real del domini`
- `mínim funcional no trivial`
- `evidències autèntiques`
- `verificació reproduïble`
- `README` actualitzat
- `AI log`
- `defensa tècnica`

## Progressió didàctica R2 → R5

- `R2`: obrir el primer flux funcional del producte amb autenticació, control d'accés i primera regla recognoscible de negoci.
- `R3`: professionalitzar eixe flux amb arquitectura mantenible, persistència real i proves mínimes de regressió.
- `R4`: exposar com a `API` una part rellevant i usable d'eixa funcionalitat, amb contracte, proves i consum reproduïble.
- `R5`: integrar eixa `API` en un flux híbrid o automatització amb valor real i tancar el producte amb criteri de manteniment i defensa.

Lectura global:

- la sèrie no està organitzada per tècniques
- està organitzada per fases de professionalització del mateix producte backend

## Punts pendents o opcionals

- afegir, més avant, variants d'exemple específiques per domini (`incidències`, `reserves`, `inventari`) si es detecta necessitat docent real.
- afegir, si convé, una capa final de materials comparatius per itinerari sobre com canvia la implementació sense canviar el llindar docent.
- revisar més avant si cal una versió reduïda o compartible dels apunts reals per a ús extern al repositori.

## Definition of done de la revisió

Esta revisió transversal es considera completada quan:

- els quatre apunts comparteixen la mateixa estructura pública bàsica
- queda bloquejada la lectura trivial de `R2`, `R3`, `R4` i `R5`
- la progressió didàctica `R2 -> R5` és clara i usable
- la terminologia crítica queda prou unificada
- la sèrie es pot llegir com un conjunt coherent dins del paquet docent del mòdul

## Nota final

La revisió transversal recollida ací deixa consolidada la lectura comuna de `R2-R5`, però el tancament definitiu de la sèrie queda pendent fins incorporar i rellegir també l'apunt real del Repte 1 com a obertura completa del bloc `R1-R5`.
