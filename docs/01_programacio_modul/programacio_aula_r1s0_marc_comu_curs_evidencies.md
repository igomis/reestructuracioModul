# R1S0. Marc comú del curs i criteri d'evidències

## Finalitat de la sessió

Esta sessió obri el curs abans d'entrar en els microreptes de `R1`. La seua funció és fixar el model de treball, el projecte base, el sistema d'evidències, la traçabilitat i el paper verificable de la IA.

## Encaix dins del Repte 1

- **Repte**: `R1. Kickoff backend`
- **Microrepte**: `Sessió sense microrepte propi`
- **Sessió**: `R1S0`
- **Duració orientativa**: `3 hores`
- **Focus**: model de curs, repositori, evidències, ús d'IA, criteri de defensa i primer mapa del producte
- **No entra encara**: implementació tècnica del backend

## Seqüència d'aula de 3 hores

### 0:00-0:40. Presentació del curs per reptes

Usar la presentació general del curs per deixar explícit:

- el fil `R1 -> R5`: no són pràctiques soltes, sinó un producte backend que creix;
- el paper de cada repte: arrancada, processament, framework, `API`, integració i defensa;
- el repartiment en dues avaluacions lectives i el paper residual de la tercera avaluació;
- la diferència entre treball cooperatiu, contrast tècnic i evidència individual;
- què vol dir `repte`, `microrepte`, `microtaller`, `checkpoint` i defensa.

Resultat esperat: l'alumnat pot explicar en una frase quin producte construirà, com evolucionarà durant el curs i com es comprovarà que el treball és seu.

### 0:40-1:20. Sistema de treball i repositori

Revisar estructura mínima de repositori, `README`, commits, issues i criteri de traçabilitat.

### 1:20-2:00. Ús verificable de la IA

Modelar què és un `AI log` útil, què és delegació excessiva i com es contrasta autoria.

### 2:00-2:40. Primer mapa del producte

El primer mapa del producte no és un disseny final ni un document llarg d'anàlisi. És una fitxa inicial de decisions per evitar començar amb una idea massa genèrica.

Cada alumne o equip deixa escrit en el `README.md` inicial:

| Decisió | Pregunta guia | Exemple de resposta curta |
|---|---|---|
| Producte | Què vols construir? | Gestor d'incidències d'aula |
| Usuari principal | Qui l'usarà primer? | Professorat que registra incidències |
| Necessitat real | Quin problema resol? | Saber què està pendent i qui ho ha revisat |
| Primera acció útil | Quina acció ha de funcionar abans que cap altra? | Crear una incidència amb estat inicial |
| Dades principals | Quines dades mínimes apareixen? | títol, aula, prioritat, estat, data |
| Primera resposta backend | Què hauria de respondre el servidor en `R1/R2`? | confirmació o error validat |
| Dubte o risc | Què pot bloquejar el projecte? | rols massa amplis o flux poc concret |

L'objectiu és tindre una primera hipòtesi de producte, no tancar encara totes les pantalles, entitats o permisos.

### 2:40-3:00. Checkpoint inicial

Checkpoint breu, oral i verificable. No es revisa encara codi de backend: es comprova que l'alumnat està preparat per començar `R1S1` sense improvisar.

Preguntes de comprovació:

| Pregunta | Mínim acceptable |
|---|---|
| Quin producte vas a construir? | Una frase concreta, no "una web" o "un CRUD" |
| Qui l'usarà? | Un actor inicial recognoscible |
| Quina serà la primera acció real? | Una operació funcional que després es puga validar |
| On deixaràs les evidències? | Repositori i `README.md` identificats |
| Com registraràs l'ús d'IA si apareix? | Criteri o plantilla d'`AI log` entés |
| Què has de portar a `R1S1`? | Idea acotada, repositori preparat i primera decisió de stack pendent o iniciada |

## Evidències mínimes

| Evidència | Mínim acceptable |
|---|---|
| Repositori | creat o identificat i accessible per al professorat |
| README inicial | conté la fitxa inicial del producte i la ubicació de les evidències |
| AI log | plantilla preparada o criteri clar sobre quan registrar ajuda d'IA |
| Primer mapa del producte | producte, usuari, necessitat, primera acció, dades i risc inicial |
| Checkpoint inicial | alumne capaç d'explicar producte, primera acció i pròxim pas cap a `R1S1` |

## Checklist de tancament

- [ ] Repositori preparat.
- [ ] `README.md` inicial amb primer mapa del producte.
- [ ] Criteri d'evidències entés.
- [ ] Ús d'IA explicat.
- [ ] Domini inicial registrat amb primera acció real.
- [ ] Checkpoint inicial fet: l'alumnat sap què ha de portar a `R1S1`.

## Materials associats per a portar a l'aula

- **Presentació general del curs**: [Presentació 00. Visió del curs](../07_presentacions/presentacio_00_visio_curs.md). Font docent existent; pendent de publicar com a PDF en la documentació d'alumnat si es genera amb Gamma.
- **Briefing docent**: [Briefing inicial del curs](../08_materials_compartibles/briefing_inicial_curs.md)
- **Presentació de microtaller associada**: [MT19. IA responsable aplicada al repte](https://cipfpbatoi.github.io/dwes2627/recursos/Tallers/MT19-IA-responsable-aplicada-al-repte.pdf)
- **Material de consulta associat**: [Ús verificable de la IA](https://cipfpbatoi.github.io/dwes2627/04_materials/guia_us_verificable_ia.html)

## Microtaller associat

- **Microtaller**: `MT19. IA responsable aplicada al repte`
- **Moment recomanat**: en l'obertura del curs i de manera recurrent abans dels checkpoints quan aparega ús intensiu d'IA.
- **Evidència mínima**: primera pauta d'AI log i criteri clar sobre què ha de poder defensar l'alumnat.
