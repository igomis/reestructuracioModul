# Preparació docent directa per al curs que ve

## Finalitat del document

Baixar la `v1` prepilotatge ja congelada a un nivell de preparació docent directa perquè l'inici de curs no depenga d'improvisació. Este document no redefinix el model ni reobri l'arquitectura del paquet: concreta què ha d'estar realment preparat abans de setembre per poder activar el curs amb criteri estable.

Assumix el marc ja fixat al repositori: treball per reptes, projecte base compartit, seqüència en `2` avaluacions, evidències autèntiques, IA com a eina guiada i verificable, i acreditació individual encara que puguen existir contextos puntuals de producte compartit o moments de treball coordinat.

## Què ha d'arribar preparat a l'inici de curs

- criteri docent comú sobre el producte base, els reptes `R1-R5`, els checkpoints i la defensa individual
- itinerari principal de referència o criteri clar per gestionar `Laravel`, `Express/Nest` i `FastAPI` sense dispersió inicial
- paquet d'arrancada del curs llest per a `CP-P0`: enunciat base, projecte base, materials de sessió inicials, guies comunes de Git/`README`/IA i full de treball base
- lectura prèvia dels kits de pilotatge `1-20` i de la guia setmanal per saber què convé explicar, modelar i exigir en cada tram
- sistema d'evidències, rúbriques i instruments de seguiment accessibles des del primer dia
- criteri de reconducció per alumnat endarrerit ja decidit: reduir abast, reforçar traçabilitat i tancar mínims funcionals, no canviar de projecte ni reexplicar Git/GitHub des de zero

## Guions docents mínims per trams o reptes

### Arrancada i `R1` (`setmanes 1-4`)

- explicar amb claredat el model del curs, el projecte base, el criteri de no trivialitat i el paper de Git/GitHub com a repàs metodològic i traçabilitat
- modelar repositori usable, `README` mínim, primer flux funcional i primera validació o registre de dada
- tindre clar quin és el mínim funcional que permet entrar a `R2` sense arrossegar un esquelet buit

### `R2` (`setmanes 5-8`)

- explicar auth com a infraestructura per a un flux de negoci, no com a finalitat del repte
- modelar un recorregut autenticat curt amb una operació real del domini i un primer error controlat
- deixar preparat el criteri de tancament de `R2`: operació protegida usable, errors mínims i `README` actualitzat

### `R3` (`setmanes 9-12`)

- explicar el pas a arquitectura mantenible i persistència com a resposta a un producte que ja viu
- modelar una refactorització curta, una entitat persistent i una comprovació de regressió
- decidir abans d'entrar a aula quin mínim persistent és suficient per obrir `R4`

### `R4` (`setmanes 13-16`)

- explicar què fa publicable una part del producte i com convertir-la en contracte d'`API` amb sentit
- modelar un endpoint nuclear amb cas correcte, cas d'error, prova reproduïble i consum mínim
- tindre preparat el checkpoint fort de `R4`: contracte, proves, documentació, consum i autoria individual visibles

### `R5` i tancament (`setmanes 17-20`)

- explicar `R5` com a integració útil o flux híbrid al servei del producte, no com a exhibició d'eina
- modelar un workflow mínim amb entrada, consum d'`API`, eixida observable i una fallada rellevant
- preparar també la defensa final individual, el tancament del repositori i la recollida de feedback del curs

## Demos o modelatges que convé tindre llestos

- obertura de repositori, `README` inicial i rastre mínim d'ús verificable de la IA
- primera peça funcional de `R1` amb validació i registre de dada
- flux autenticat curt de `R2` amb una operació de negoci real
- refactorització o pas a capes d'`R3` amb una entitat persistent i comprovació de regressió
- contracte d'`API` i endpoint nuclear de `R4` amb prova curta i consum reproduïble
- workflow d'`R5` amb integració o automatització útil, més una incidència controlada
- defensa tècnica breu basada en autoria, decisions, proves, `README` i AI log

Criteri pràctic:

- les demos han de ser curtes, reproduïbles i reutilitzables; no convé preparar peces massa grans que després no es puguen modelar en directe amb claredat

## Materials d'entrega immediata a l'alumnat

- enunciat base del projecte i criteri general del curs
- fitxa del Repte `1` i materials de sessió de les primeres setmanes
- guies comunes de Git/GitHub, `README`, `ADR` o equivalent i ús verificable de la IA
- fulls de treball base, mini briefings i checkpoints curts d'aula
- sistema d'evidències, rúbrica base i criteri de defensa individual
- apunt real i materials contextualitzats del repte que s'obri en cada canvi de tram

## Decisions que no convé improvisar en setembre

- quin itinerari funcionarà com a referència principal i amb quin criteri s'obrirà la resta
- quins dominis o tipus de producte s'admetran i quins queden fora per evitar trivialitat o dispersió
- com es gestionarà la combinació entre context de producte compartit i acreditació individual
- quins checkpoints són de pas real i quines evidències mínimes els activen
- quina pauta mínima s'exigirà en `README`, traçabilitat, proves i AI log
- com es reconduirà alumnat endarrerit sense crear recorreguts paral·lels desconnectats

## Prioritats de preparació abans de l'inici de curs

1. Revisar la `v1` prepilotatge i el backlog per distingir amb nitidesa què és base estable i què continua sent millora pendent.
2. Tancar el paquet d'arrancada de `setmanes 1-4` i deixar preparada l'activació de `CP-P0`.
3. Seleccionar i assajar els modelatges mínims que s'usaran a `R1`, `R2`, `R3`, `R4` i `R5`.
4. Deixar accessibles els materials que s'entregaran immediatament a l'alumnat i els instruments de seguiment docent.
5. Fixar per escrit les decisions que no es volen improvisar en setembre.
6. Revisar els punts sensibles del backlog que sí convé ajustar abans de l'inici de curs, sense reobrir la `v1`.

## Definition of done de la preparació docent directa

La preparació docent directa es considera prou avançada quan:

- el professorat pot obrir el curs amb guió, materials i demos clars sense reconstruir el sistema ni improvisar arquitectura
- cada tram del curs té identificat què s'ha d'explicar, què s'ha de modelar i quin mínim funcional dóna pas al tram següent
- els materials d'entrega immediata estan seleccionats, accessibles i alineats amb el producte base
- queden fixades les decisions sobre itineraris, domini, checkpoints, defensa individual, Git/GitHub i ús verificable de la IA
- el backlog de millora continua separat de la base estable i només s'usa per a ajustos finals previs a l'inici de curs
