# AGENTS.md

## Criteri transversal d'alineació

Els continguts de `dwes-restructuracio-modul`, `dwes-documentacio-alumnat` i `dwes-microreptes-autocorreccio` han d'estar alineats. Quan es cree, canvie o elimine un repte, sessió o microrepte en un d'estos repositoris, cal revisar si també cal actualitzar els altres dos.

La coherència mínima ha d'incloure:

- mateix codi de repte, sessió i microrepte, per exemple `R2`, `R2S2`, `R2M2`;
- mateix nom funcional del microrepte;
- mateix abast pedagògic;
- mateixos criteris d'avaluació treballats;
- evidències compatibles entre programació d'aula, documentació d'alumnat i autocorrecció;
- mateixa decisió sobre què entra com a mínim i què queda com a ampliació.

## Paper de cada projecte

- `dwes-restructuracio-modul`: font docent de planificació, programació d'aula, seqüenciació, criteris curriculars i decisions metodològiques.
- `dwes-documentacio-alumnat`: materials que veu l'alumnat: reptes, microreptes, instruccions de treball, rúbriques/checklists i materials de suport.
- `dwes-microreptes-autocorreccio`: definició executable de les autocorreccions: `challenge.json`, `rubric.json`, prompts, evidències esperades i proves de revisió.
- `dwes-microreptes-alumnes`: base o plantilla de treball de l'alumnat; ha de reflectir el que es demana en la documentació i el que després es podrà autocorregir.

## Estructura esperada de `dwes-documentacio-alumnat`

La documentació d'alumnat ha de diferenciar clarament tres blocs:

- Reptes i microreptes: què ha de construir l'alumnat, què ha d'entregar, requisits mínims i què queda per a més avant.
- Rúbriques, checklists o criteris de sessió/microrepte: com es valorarà cada sessió o microrepte, amb evidències observables.
- Materials de suport per als reptes: guies, consulta tècnica, exemples, plantilles i recursos que ajuden a resoldre el repte sense substituir l'enunciat.

No s'han de mesclar en una mateixa pàgina instruccions de lliurament, rúbrica i material teòric extens si això dificulta que l'alumnat entenga què ha de fer.

## Estructura obligatòria de les programacions d'aula

Les programacions d'aula de sessions o microreptes han de tractar sempre els mateixos punts i mantindre un ordre coherent entre pàgines. Quan es cree o es refactoritze una programació d'aula, ha de cobrir estos apartats:

- Finalitat de la sessió.
- Encaix dins del repte.
- Relació amb RA, CA i criteris de treball.
- Producte esperat.
- Preparació prèvia del professorat.
- Continguts a explicar.
- Seqüenciació de la sessió.
- Tasques concretes de l'alumnat.
- Evidències mínimes.
- Criteris d'èxit.
- Què no és suficient.
- Ús de la IA.
- Suport per a l'alumnat amb dificultats.
- Ampliació per a l'alumnat més avançat.
- Checklist de tancament.
- Connexió amb el microrepte posterior.

Si un apartat no aplica de manera directa, s'ha de mantindre igualment amb una indicació breu del motiu o amb una concreció mínima. No s'han de crear programacions d'aula amb estructures parcialment diferents si corresponen al mateix tipus de sessió.

## Relació entre sessions i microreptes

Cada sessió ordinària ha de tindre associat un microrepte. La nomenclatura ha de permetre veure la relació entre repte, sessió i microrepte, per exemple `R2S2` i `R2M2`.

Les úniques excepcions són les sessions de presentació o tancament dels reptes `2`, `3`, `4` i `5`. Estes sessions poden no tindre microrepte associat si la seua funció és introduir el repte, organitzar el treball, fer síntesi, revisar evidències o tancar el procés.

Quan una sessió no tinga microrepte per este motiu, s'ha d'indicar explícitament en la programació d'aula que és una sessió de presentació o tancament i que no genera microrepte propi.

## Forma de treball

Abans d'editar:

- revisar com està definit el mateix repte o microrepte en els altres repositoris;
- comprovar la nomenclatura existent;
- evitar avançar continguts que encara no pertoquen segons la seqüència acordada.

Després d'editar:

- executar `mkdocs build` si s'ha modificat documentació MkDocs;
- executar `npm run validate` si s'ha modificat `dwes-microreptes-autocorreccio`;
- revisar que els enllaços, títols i codis continuen sent coherents.
- al final de cada iteració, fer commit i push dels repositoris afectats;
- fer staging selectiu dels fitxers de la iteració i no incloure fitxers aliens o temporals, com `.DS_Store`.
