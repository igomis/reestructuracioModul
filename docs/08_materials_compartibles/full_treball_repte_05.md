# Full de treball del Repte 5

## Objectiu

Tancar el producte amb una integració o flux híbrid útil, provat i defensable.

## Tasca

- tria una necessitat real del producte que resolgues amb integració
- defineix entrada, procés i eixida del flux
- reutilitza l'`API` pròpia com a peça central
- implementa el recorregut principal en `n8n` o eina equivalent si té sentit
- prova un cas correcte i una fallada rellevant
- documenta el flux i prepara la defensa final

## Evidència mínima

- integració o workflow justificat
- recorregut complet de punta a punta
- eixida observable
- prova d'almenys un error o incidència
- documentació final i `README` actualitzat

## Targeta fixa de traçabilitat

- **Criteri/objectiu**: `RA9`, integració híbrida amb valor de producte.
- **Descriptor de rúbrica**: flux complet, prova de punta a punta, traçabilitat i defensa.
- **Moment d'avaluació**: validació de font i demo final.
- **Agent d'avaluació**: professorat amb mini defensa de l'alumne.
- **Tipus d'evidència**: workflow o connector, mapping, demo, error i documentació.

## Validació mínima

- mostra què inicia el flux
- executa el recorregut complet
- ensenya què passa quan falla una part rellevant
- localitza on està documentat i com es reproduïx

## Errors habituals

- usar `n8n` només perquè queda vistós
- no connectar de veritat amb l'`API` de `R4`
- duplicar lògica de negoci al workflow
- no deixar rastre de fallades o incidències
- no saber explicar quin valor real aporta el flux

## Ampliació si acabes prompte

- reforça control d'errors o reintents
- millora traçabilitat del procés
- afegeix un segon pas justificat dins del mateix flux, sense obrir un projecte paral·lel
