# Programació d'aula del Repte 2

## Finalitat del document

Este document baixa `R2` a una seqüència operativa d'aula perquè el professorat puga conduir el repte com una progressió completa de dades, lògica, estat i autenticació, sense reduir-lo a “formulari + login”.

## Finalitat del repte

- consolidar una base comuna en `PHP` per a tot l'alumnat
- construir una primera funcionalitat real del producte a partir d'un flux complet de servidor
- fer visible la relació entre formulari, processament, lògica, estat, autenticació i funcionalitat protegida
- mantindre la persistència com a suport funcional del flux, no encara com a centre metodològic del repte
- preparar un pas net cap a `R3`, que serà el punt d'entrada dels itineraris diferenciats

## Duració base

- `18 hores`
- `6` sessions de `3` hores
- cada sessió es correspon amb un microprojecte docent concret

## Coordinació explícita entre sessions i microprojectes

| Sessió | Duració | Microprojecte | Focus principal | Evidència clau |
|---|---:|---|---|---|
| `1` | `3h` | `MP1` | formulari i validació visible | dades recuperades, errors clars i reintent |
| `2` | `3h` | `MP2` | processament i guardat funcional | dada correcta tractada, guardada i reutilitzada |
| `3` | `3h` | `MP3` | lògica del flux i regles del projecte | decisió, estructura o funció amb efecte visible |
| `4` | `3h` | `MP4` | estat, sessió i/o cookies | recuperació del flux i invalidació controlada |
| `5` | `3h` | `MP5` | autenticació i funcionalitat protegida | cas autoritzat i cas denegat d'una operació real |
| `6` | `3h` | `MP6` | prova, depuració, documentació mínima i checkpoint | checklist, README i demo reproduïble |

## Seqüència recomanada de sessions

### Sessió 1. Microprojecte 1

**Formulari i validació visible**

- Objectiu: obrir el punt d'entrada de dades del projecte i deixar clar què es rep, què es valida i què no pot continuar mentre hi haja errors.
- Què explica el professorat: quina acció real del domini es treballarà durant `R2`, què diferencia una validació visible d'un missatge genèric i per què encara no toca començar per auth.
- Què modela el professorat: un exemple curt de recuperació de dades, validació de servidor i feedback útil a l'usuari.
- Què fa l'alumnat: concreta l'acció del domini, implementa formulari o entrada equivalent, recupera dades, mostra errors i prova un reintent corregit.
- Materials necessaris: fitxa del Repte 2, base comuna en `PHP`, guia de validació i errors del Repte 2, materials comuns.
- Evidència esperada: formulari funcional, error visible, reenviament corregit i explicació de com arriba la dada al servidor.
- Checkpoint: el flux es talla quan hi ha error i l'alumnat pot explicar per què.

### Sessió 2. Microprojecte 2

**Processament i guardat funcional**

- Objectiu: fer visible el processament bàsic en servidor i deixar una primera conservació funcional de la informació correcta.
- Què explica el professorat: com la base comuna en `PHP` genera resposta, quin paper tenen variables, operadors i àmbits, i per què guardar funcionalment no significa encara obrir un bloc fort de persistència.
- Què modela el professorat: un tram curt de processament amb resposta generada a partir de la dada rebuda i reutilització posterior de la informació correcta.
- Què fa l'alumnat: processa una entrada ja validada, guarda de manera simple la informació útil i la torna a mostrar o reutilitzar dins del projecte.
- Materials necessaris: fitxa del Repte 2, materials comuns, suport de guardat triat pel grup, exemples de fitxer o imatge si apliquen.
- Evidència esperada: tractament executable, dada correcta guardada, primera reutilització visible i justificació del mecanisme triat.
- Checkpoint: si apareix base de dades, l'alumnat pot explicar per què ací continua sent suport funcional i no el centre del repte.

### Sessió 3. Microprojecte 3

**Lògica del flux i regles del projecte**

- Objectiu: fer que el backend prenga decisions amb sentit i aplique almenys una regla recognoscible del projecte.
- Què explica el professorat: quan convé usar decisions, recorreguts, arrays o funcions i com evitar una lògica ornamental.
- Què modela el professorat: una regla simple del domini amb una decisió i una funció curta que canvia el comportament del flux.
- Què fa l'alumnat: incorpora una regla significativa, usa una estructura o funció amb sentit i prova almenys dos casos amb resultat diferent.
- Materials necessaris: fitxa del Repte 2, materials comuns, esquema del domini i casos de prova breus.
- Evidència esperada: lògica observable, funció o estructura útil, comportament diferenciat i checkpoint curt del recorregut fins ací.
- Checkpoint: el professorat pot veure que el sistema ja “pensa” i no només rep i guarda dades.

### Sessió 4. Microprojecte 4

**Estat, sessió i/o cookies**

- Objectiu: mantindre informació provisional entre peticions i distingir-la de la conservació funcional del domini.
- Què explica el professorat: diferència entre estat, sessió, cookies i altres mecanismes equivalents; què convé guardar en client, què en servidor i quan toca invalidar-ho.
- Què modela el professorat: una recuperació breu d'estat després d'un error o d'un pas intermedi i una invalidació controlada.
- Què fa l'alumnat: implementa estat temporal coherent amb el seu flux, recupera el punt del procés i neteja la informació quan deixa de tindre sentit.
- Materials necessaris: fitxa del Repte 2, guia de flux d'usuari i sessions, navegador amb eines de desenvolupament, materials comuns.
- Evidència esperada: recuperació funcional del flux, explicació clara del que queda en client o en servidor i prova d'invalidació.
- Checkpoint: l'alumnat sap distingir estat temporal, conservació funcional i autenticació.

### Sessió 5. Microprojecte 5

**Autenticació i funcionalitat protegida**

- Objectiu: connectar tot el flux anterior amb una operació real del domini protegida per autenticació o per una restricció funcional observable.
- Què explica el professorat: diferència entre autenticació i autorització, quin és el mínim funcional no trivial del repte i per què una ruta decorativa no és una funcionalitat protegida.
- Què modela el professorat: un accés permés, un accés denegat i el punt exacte on es comprova la restricció.
- Què fa l'alumnat: implementa autenticació funcional mínima, protegix una acció del projecte i demostra el cas autoritzat i el denegat.
- Materials necessaris: fitxa del Repte 2, guia de flux d'usuari i sessions, materials comuns, usuaris de prova.
- Evidència esperada: autenticació funcional, operació protegida lligada al domini, cas positiu i negatiu reproduïbles.
- Checkpoint: no es tanca `R2` si hi ha auth aparent però no una operació real protegida.

### Sessió 6. Microprojecte 6

**Prova, depuració, documentació mínima i checkpoint**

- Objectiu: revisar el flux complet, deixar proves mínimes registrades i preparar la transició cap a `R3`.
- Què explica el professorat: com usar la checklist de proves, quins casos s'han de poder mostrar i quina documentació mínima ha d'estar viva al `README`.
- Què modela el professorat: una prova curta del flux complet i una lectura ràpida de com la documentació ajuda a reproduir-lo.
- Què fa l'alumnat: executa casos correctes i incorrectes, registra incidències, actualitza `README` i deixa clar què caldrà reorganitzar després.
- Materials necessaris: checklist del Repte 2, guia de testing i debugging, fitxa del Repte 2, materials comuns.
- Evidència esperada: proves mínimes, errors controlats, rastre de depuració, documentació actualitzada i demo breu reproduïble.
- Checkpoint: el professorat valida que el pas a `R3` es fa sobre un flux real i no sobre una demo puntual.

## Evidències esperades per sessió

- Sessió `1`: formulari o entrada equivalent, recuperació real de dades i errors visibles.
- Sessió `2`: tractament executable, guardat funcional i primera reutilització de la informació correcta.
- Sessió `3`: decisió, regla o funció amb efecte real sobre el flux.
- Sessió `4`: estat recuperable, demostració d'invalidació i frontera clara entre estat i conservació funcional.
- Sessió `5`: operació del domini protegida amb cas autoritzat i cas denegat.
- Sessió `6`: checklist de prova, documentació mínima i checkpoint final.

## Moments de checkpoint

- Checkpoint curt `1`: al final de la sessió `2`, per comprovar que el flux ja rep, valida, processa i reutilitza dades.
- Checkpoint curt `2`: al final de la sessió `4`, per validar que estat, sessió o cookies no s'estan confonent amb persistència del domini.
- Checkpoint curt `3`: al final de la sessió `5`, per confirmar que hi ha una operació real protegida.
- Checkpoint de pas `R2 -> R3`: al final de la sessió `6`, per decidir si el grup entra al contrast de frameworks amb una base funcional defensable.

## Preparació del tancament del repte

- demanar una demo curta del flux complet, no només del login
- revisar que la informació correcta es recupera o es reutilitza dins del projecte
- exigir un cas de validació visible, un cas autoritzat i un cas denegat
- comprovar que la documentació mínima permet repetir la prova
- demanar què haurà de reorganitzar-se en `R3` i què encara continua sent suport funcional de `R2`

## Criteri pràctic de tancament

`R2` queda preparat quan el professorat pot veure un flux complet de dades, lògica, estat i autenticació sobre la base comuna en `PHP`, amb una operació real protegida, proves mínimes reproduïbles i un pas justificat cap a `R3`.
