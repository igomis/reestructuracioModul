# Orquestració de fluxos: consulta ràpida

## Què és

Guia curta per situar eines d'orquestració dins del curs. Aquestes eines no són un fi en si mateixes: són possibles implementacions de `R5` per orquestrar un flux híbrid útil sobre l'`API` del teu producte.

## Quan la necessites en el curs

- sobretot en `R5`
- només després de tindre una `API` clara i prou estable de `R4`
- quan el teu projecte realment necessita una notificació, automatització o recorregut extern

## Què has de saber sí o sí

- el flux ha d'eixir d'una necessitat real del producte
- has de poder dibuixar clarament `trigger`, entrada, consum d'`API`, transformació i eixida
- el backend continua sent la font de veritat de la lògica
- has de provar com a mínim un cas correcte i una fallada rellevant
- el `workflow` ha de quedar exportat o documentat de manera reproduïble

## Errors habituals

- usar una eina d'orquestració només perquè es veu bé
- construir un `workflow` decoratiu que no tanca cap problema del producte
- copiar nodes, credencials o `mappings` sense entendre'ls
- no controlar què passa quan falla l'`API` o el servei extern
- no deixar rastre clar del procés complet

## On ampliar

- Material del curs: [Repte 5. Integració híbrida i tancament](../../02_reptes/repte_05_integracio_hibrida.md)
- Material del curs: [Guia d'orquestració i automatització](../../04_materials/repte_05/guia_orquestracio_i_automatitzacio.md)
- Docs d'eines d'orquestració (ex.: n8n) i recursos externs
