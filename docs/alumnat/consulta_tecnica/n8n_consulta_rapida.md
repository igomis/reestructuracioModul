# n8n: consulta ràpida

## Què és
És una guia curta per situar `n8n` dins del curs. `n8n` ací no és un fi en si mateix: és una possible eina de `R5` per orquestrar un flux híbrid útil sobre l'`API` del teu producte.

## Quan la necessites en el curs
- sobretot en `R5`
- només després de tindre una `API` clara i prou estable de `R4`
- quan el teu projecte realment necessita una notificació, automatització o recorregut extern

## Què has de saber sí o sí
- el flux ha d'eixir d'una necessitat real del producte
- has de poder dibuixar clarament trigger, entrada, consum d'`API`, transformació i eixida
- el backend continua sent la font de veritat de la lògica; `n8n` no ha de duplicar-la sense criteri
- has de provar com a mínim un cas correcte i una fallada rellevant
- el workflow ha de quedar exportat o documentat de manera reproduïble

## Errors habituals
- usar `n8n` només perquè “es veu bé”
- construir un workflow decoratiu que no tanca cap problema del producte
- copiar nodes, credencials o mappings sense entendre'ls
- no controlar què passa quan falla l'`API` o el servei extern
- no deixar rastre clar del procés complet

## On consultar-ho bé
- [Repte 5. Integració híbrida i tancament](../../02_reptes/repte_05_integracio_hibrida_n8n.md)
- [Apunts reals del Repte 5](../../04_materials/apunts_reals/repte_05_integracio_hibrida_n8n.md)
- [Integració de n8n](../../05_projectes_tecnics/integracio_n8n.md)
- [Guia `n8n` i automatització](../../04_materials/repte_05/guia_n8n_i_automatitzacio.md)
- [Guia d'integració externa i flux híbrid](../../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md)
