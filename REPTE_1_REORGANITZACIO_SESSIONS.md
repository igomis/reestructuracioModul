# Reorganització de sessions del Repte 1

## Què es manté dels 4 microreptes

El Repte 1 continua tenint `4` microreptes:

- `Microrepte 1`: entendre client/servidor, diferenciar execució en client i servidor, i decisió tècnica inicial
- `Microrepte 2`: muntar l’entorn executable
- `Microrepte 3`: construir el primer punt d’entrada funcional
- `Microrepte 4`: documentar, verificar i preparar el checkpoint

La decisió no elimina cap microrepte ni canvia la funció bàsica de cada un. Els microreptes queden com a unitats de progrés del repte.

## Com s’ha reorganitzat la temporalització

La temporalització passa de llegir-se com `4` sessions separades a una execució compactada:

- Sessió `1`: `Microrepte 1` + inici del `Microrepte 2`
- Sessió `2`: tancament del `Microrepte 2` + `Microrepte 3` + `Microrepte 4`
- Sessió `3` opcional: defensa, checkpoint formal, revisió de traçabilitat o microcanvis en viu

La idea clau incorporada és que els microreptes són unitats de progrés i les sessions són unitats de temps docent. En `R1`, diversos microreptes poden agrupar-se dins d’una mateixa sessió.

## Com s’ha actualitzat la programació d’aula

`docs/01_programacio_modul/programacio_aula_repte_01.md` queda reescrit amb:

- relació explícita entre microreptes i sessions
- `2` sessions principals de `3` hores
- una tercera sessió opcional
- sessió `1` dedicada a model client/servidor, decisió inicial i arrencada de l’entorn
- sessió `2` dedicada a tancar l’entorn, crear la primera funcionalitat mínima i documentar el repte
- evidències i checkpoints ajustats a esta compactació

## Com s’ha incorporat la documentació en repositori

El Repte 1 incorpora com a evidència real que l’alumnat:

- cree un directori de documentació dins del repositori
- penge les fitxes o documents del repte al repositori
- cree un índex o pàgina visible que enllace eixa documentació

No queda plantejat com a burocràcia. La documentació en repositori servix per donar traçabilitat al treball, facilitar la revisió docent i preparar el checkpoint.

## Comprovació de coherència amb criteris i evidències

- Es manté el treball per reptes.
- Es manté la base comuna en `PHP`, `Docker` i servidor web.
- El Repte 1 continua sense ser un repte de framework complet.
- El `Microrepte 3` continua sent el primer punt d’entrada funcional.
- El `Microrepte 4` continua sent documentació, verificació i checkpoint.
- Les evidències continuen incloent repositori usable, commits significatius, README executable, primera funcionalitat mínima, justificació tècnica breu, AI log quan pertoque i defensa o checkpoint.

## Nota d'ajust curricular: RA1a

S'ha incorporat explícitament el `RA1a` al Repte 1: “S'han caracteritzat i diferenciat els models d'execució de codi en el servidor i en el client web.”

L'ajust queda visible en:

- `docs/02_reptes/repte_01_kickoff_backend.md`: el `Microrepte 1` incorpora `RA1a`, demana diferenciar què s'executa al client i què al servidor, i afegeix evidència i pregunta oral de verificació.
- `docs/01_programacio_modul/programacio_aula_repte_01.md`: la sessió 1 incorpora el model d'execució client vs servidor en objectiu, evidència esperada i checkpoint.
- `docs/matriu-coherencia-curricular-dwes.md`: la fila de `RA1` explicita que `RA1a` es cobreix en `MP1` i sessió 1.
- `docs/alumnat/reptes/repte_01.md`: la guia curta de l'alumnat queda alineada amb la temporalització compactada, el `RA1a` i les evidències reals del repte.

Evidència associada: explicació breu del model d'execució client vs servidor aplicada al producte propi.

Checkpoint associat: cada alumne ha de poder explicar quina part del seu producte s'executa al client i quina al servidor.
