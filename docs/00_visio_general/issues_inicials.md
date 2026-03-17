# Estat de producció actual

El repositori ja no està en fase de bootstrap. La base curricular, el projecte base, els materials comuns, els materials per repte i els tres itineraris tecnològics ja existixen. La necessitat actual és consolidar el conjunt perquè siga llegible, comparable i usable en implantació docent real.

## Paquets consolidats
- `MG-01` queda consolidat com a marc de priorització i seqüència de producció a `docs/04_materials/pla_materials_prioritaris.md`.
- `MG-02` queda consolidat com a base comuna del mòdul amb guies de Git, README/ADR, testing/debugging i ús verificable de la IA.
- `MG-03` queda consolidat com a paquet nuclear del Repte 2 amb materials sobre flux d'usuari, sessions, validació i errors de servidor.
- `MG-04` queda consolidat com a paquet nuclear del Repte 3 amb materials sobre arquitectura per capes o equivalent, persistència i qualitat tècnica.
- `PB-01` queda consolidat amb l'enunciat base del projecte del curs ja usable i visible.

## Paquets en producció
- `MG-05` continua com a paquet en producció perquè els materials del Repte 4 encara han de passar una ronda equivalent de consolidació pública i revisió de coherència.
- `MG-06` continua com a paquet en producció perquè els materials del Repte 5 encara s'han d'acabar d'alinear amb la seqüència `R3 -> R4 -> R5` i amb el tancament del producte del curs.

## Itineraris consolidats / en revisió
- `MI-01` `Laravel` queda consolidat com a primer patró reusable de stack.
- `MI-02` `Express/Nest` queda consolidat com a segon patró reusable de stack.
- `MI-03` `FastAPI` queda en revisió transversal junt amb `MI-01` i `MI-02` per assegurar comparabilitat pública.

Criteri comú dels itineraris:
- han de compartir estructura pública, profunditat mínima, tipus de checklist i nivell d'exigència
- han de connectar de manera equivalent amb els Reptes 2, 3, 4 i 5
- han de mantindre el mateix nivell de control sobre auth, persistència, proves, `README` i `AI log`

## Següent focus recomanat
- tancar la ronda de consolidació de `MG-05` i `MG-06`
- homogeneïtzar definitivament els tres itineraris perquè funcionen com a patró docent comparable
- preparar la fase següent de materials avançats i d'implantació docent sense obrir encara nous paquets
