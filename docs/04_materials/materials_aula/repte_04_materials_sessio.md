# Materials de sessió del Repte 4

## Finalitat del document

Contextualitzar les plantilles d'aula del curs per al `R4`, de manera que el professorat puga convertir una part rellevant del producte en `API` usable i consumible, sense reduir el repte a “fer endpoints” o “retornar JSON”.

## Mini-briefings de les sessions clau

### Sessió clau 1. Contracte d'`API`

- Objectiu de la sessió: decidir què es publicarà i amb quin contracte mínim
- Què s'espera al final: recursos, endpoints i respostes nuclears definits
- Error habitual a evitar: obrir rutes sense pensar quin cas d'ús real exposen
- Evidència mínima del dia: contracte bàsic d'`API`
- Pregunta de tancament: quina part del producte queda realment publicada i per a qui?

### Sessió clau 2. Implementació dels endpoints principals

- Objectiu de la sessió: portar a codi els endpoints nuclears del flux principal
- Què s'espera al final: operació principal disponible com a `API`
- Error habitual a evitar: tindre endpoint però no coherència d'errors o codis d'estat
- Evidència mínima del dia: endpoint funcional i resposta reproduïble
- Pregunta de tancament: què pot consumir ara un tercer que abans només vivia dins del backend?

### Sessió clau 3. Prova i consum

- Objectiu de la sessió: tancar `R4` amb consum i documentació real
- Què s'espera al final: `API` provada i documentada
- Error habitual a evitar: documentar un comportament que no coincidix amb el real
- Evidència mínima del dia: prova o col·lecció de peticions + documentació breu
- Pregunta de tancament: si una altra persona usara hui la vostra `API`, amb què podria començar?

## Checkpoints curts específics

- `CP-R4.1`
  - Què hauria d'estar fet: contracte mínim d'`API` clar
  - Com es verifica en `2-3` minuts: mostrar recursos, operacions i codis d'estat
  - Senyal d'alerta: hi ha llista d'endpoints, però no cas d'ús publicat
  - Acció correctiva ràpida: reduir a menys endpoints i reconnectar-los amb el flux principal
- `CP-R4.2`
  - Què hauria d'estar fet: endpoint nuclear funcional
  - Com es verifica en `2-3` minuts: llançar una petició i revisar resposta correcta i incorrecta
  - Senyal d'alerta: l'endpoint respon, però no es pot justificar la seua coherència
  - Acció correctiva ràpida: tancar només un endpoint central amb errors i validacions mínimes
- `CP-R4.3`
  - Què hauria d'estar fet: prova de consum i documentació alineades
  - Com es verifica en `2-3` minuts: repetir una petició des de col·lecció o client i contrastar amb la documentació
  - Senyal d'alerta: hi ha captures o text, però no consum reproduïble
  - Acció correctiva ràpida: simplificar documentació i deixar una sola prova clarament executable

## Exemples de feedback ràpid

- Vas bé: `L'API ja publica una part real del producte i es pot consumir. Ara reforça documentació i errors.`
- Cal corregir abans de seguir: `No pots obrir R5 si la teua API encara no és usable ni reproduïble per tercers.`
- Tens funcionalitat però falta verificació: `L'endpoint està, però encara falta provar-lo en un consumidor o en una col·lecció reproduïble.`
- Tens solució massa superficial: `Has obert rutes, però no hi ha contracte d'ús clar ni evidència de consum real.`
- Tens marge per ampliar: `Si el nucli de l'API ja està tancat, pots millorar documentació, errors o seguretat del mateix flux.`

## Fulls de treball base contextualitzats

### Full 1. Contracte d'`API`

- Objectiu: decidir què es publicarà i com
- Tasca: triar recurs, operació, entrada, eixida i error mínim
- Evidència a generar: contracte curt d'`API`
- Validació mínima: una tercera persona pot entendre què fa l'endpoint
- Ajuda si et bloqueges: torna al cas d'ús principal i elimina endpoints laterals
- Ampliació si acabes prompte: millora codis d'estat o documentació del mateix flux

### Full 2. Consum i documentació

- Objectiu: tancar la `API` com a peça usable
- Tasca: provar endpoint, documentar-lo i mostrar consum
- Evidència a generar: petició reproduïble + documentació breu + resultat coherent
- Validació mínima: el consum es pot repetir sense explicació improvisada
- Ajuda si et bloqueges: deixa una sola prova manual o col·lecció mínima
- Ampliació si acabes prompte: reforça resposta d'error o qualitat de documentació

## Suport per alumnat endarrerit

- limitar la `API` a un conjunt molt curt d'endpoints nuclears
- no obrir consumidor complex si encara no hi ha una prova simple reproduïble
- revisar primer contracte, prova i `README` abans d'afegir més operacions
- bloquejar el pas a `R5` si l'`API` no és consumible de forma clara

## Ampliacions per alumnat avançat

- millor tractament d'errors sobre el mateix endpoint
- millor documentació o col·lecció de proves
- segona operació coherent sobre el mateix recurs si el nucli ja està tancat

## Evidència mínima per tram

- Tram inicial: contracte mínim d'`API`
- Tram funcional: endpoint nuclear funcional i coherent
- Tram de tancament: consum reproduïble, documentació breu i proves mínimes

## Connexió amb el repte següent

El `R4` ha de deixar una `API` prou usable per integrar-la en `R5`. Si encara no hi ha contracte, consum o prova real, la integració final es convertirà en una capa ornamental sense base sòlida.
