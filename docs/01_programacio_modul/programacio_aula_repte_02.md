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

- `21 hores`
- `7` sessions de `3` hores
- cada sessió es correspon amb un microprojecte docent concret

`R2` queda fixat amb estes `7` sessions com a base. La sessió `7` està dedicada específicament a refactorització i millora de mantenibilitat sobre un flux ja verificat.

## Coordinació explícita entre sessions i microprojectes

| Sessió | Duració | Microprojecte | Focus principal | Evidència clau |
|---|---:|---|---|---|
| `1` | `3h` | `MP1` | formulari i validació visible | dades recuperades, errors clars i reintent |
| `2` | `3h` | `MP2` | processament i guardat funcional | dada correcta tractada, guardada i reutilitzada |
| `3` | `3h` | `MP3` | lògica del flux i regles del projecte | decisió, estructura o funció amb efecte visible |
| `4` | `3h` | `MP4` | estat, sessió i/o cookies | recuperació del flux i invalidació controlada |
| `5` | `3h` | `MP5` | autenticació i funcionalitat protegida | cas autoritzat i cas denegat d'una operació real |
| `6` | `3h` | `MP6` | prova, depuració, documentació mínima i checkpoint tècnic | checklist, README i demo reproduïble |
| `7` | `3h` | `MP7` | refactorització final, organització en fitxers i primer objecte de domini | comparativa abans/després, reutilització en fitxers i justificació de la millora |

## Correspondència curta sessió -> RA -> evidència -> verificació

Esta taula és el mapa mínim de traçabilitat docent del repte. No substituïx la rúbrica ni les checklists, però ajuda a comprovar ràpidament que cada sessió deixa una evidència observable i una forma concreta de verificar aprenentatge real.

| Sessió | RA principal | Què s'aprén | Evidència mínima | Verificació docent |
|---|---|---|---|---|
| `1` | `RA2` + `RA3` | entrada de dades, recuperació en servidor i validació visible | formulari o entrada equivalent amb error i reintent corregit | execució en directe i pregunta sobre d'on ix cada dada i com arriba al servidor |
| `2` | `RA2` | generació de resposta, variables, operadors, àmbits i conservació funcional simple | dada correcta processada, guardada de manera simple i reutilitzada | canvi menut en viu sobre una variable, operador o directiva i justificació del mecanisme de conservació |
| `3` | `RA3` | decisions, arrays, funcions i regles de domini aplicades | regla amb dos resultats observables i funció o estructura útil | microcanvi en una condició o funció i explicació de per què no és ornamental |
| `4` | `RA4` | estat temporal, sessió, cookies i invalidació | recuperació d'estat i neteja o caducitat demostrada | execució de recuperació i invalidació, més pregunta sobre què queda en client, servidor o flux funcional |
| `5` | `RA4` | identificació, autenticació, autorització i protecció d'una operació real | cas autenticat permés i cas no permés sobre una acció del domini | demo dels dos casos i pregunta sobre el punt exacte on es comprova la restricció |
| `6` | `RA4` | prova, depuració, documentació i reproduïbilitat | taula mínima de proves, incidències i README actualitzat | execució d'un cas triat pel professorat i contrast amb documentació, codi i AI log |
| `7` | `RA3` + `RA4` | refactorització funcional, mantenibilitat i preparació cap a `RA5` | comparativa abans/després, fitxer comú, objecte simple i prova de no regressió | revisió del diff, execució del flux i defensa de què millora ara i què queda per a `R3` |

## Conceptes que han de quedar diferenciats

Durant el repte convé usar estos termes amb precisió, especialment en les sessions `4`, `5` i `6`:

- **Identificació**: l'usuari declara qui diu que és, per exemple amb un correu, nom d'usuari o identificador.
- **Autenticació**: el sistema comprova que eixa identitat és vàlida, per exemple amb credencials, i crea o reconeix una sessió autenticada.
- **Autorització**: el sistema decideix si un usuari ja autenticat pot executar una operació concreta segons rol, permís, propietat del recurs o regla de negoci.
- **Estat**: informació temporal o contextual que permet continuar un flux entre peticions.
- **Sessió**: mecanisme habitual per mantindre estat associat a un client des del servidor.

No es considera suficient dir que una operació està “protegida” si només hi ha login. Cal veure quina identitat s'ha declarat, com s'ha autenticat, quin estat o sessió queda activa i quina comprovació d'autorització o restricció funcional bloqueja o permet l'operació.

## Paper operatiu de la IA per fases

La IA pot aparéixer en totes les sessions, però el seu ús només compta com a suport vàlid si queda contrastat amb execució, proves i defensa posterior:

| Sessió | Ús raonable de la IA | Evidència de control |
|---|---|---|
| `1` | esborrany de formulari, missatges de validació o estructura inicial | l'alumnat explica el recorregut de cada camp i ajusta almenys una validació pròpia |
| `2` | exemples de processament, guardat simple o tractament de fitxer | prova real de reutilització de la dada i justificació del mecanisme triat |
| `3` | suggeriments de funcions, arrays o casos de decisió | defensa de la regla de domini i microcanvi en viu |
| `4` | interpretació d'errors de sessió, cookies o estat | demostració de què es guarda, on es guarda i quan s'invalida |
| `5` | esquelet de login, comprovació d'accés o missatges d'error | demo de cas permés i cas bloquejat, amb explicació del punt de control |
| `6` | generació o ampliació de casos de prova i ajuda en debugging | execució dels casos i registre de què s'ha acceptat, descartat o corregit |
| `7` | proposta de refactorització, detecció de duplicació o documentació | comparativa abans/després i justificació pròpia de la decisió final |

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

**Prova, depuració, documentació mínima i checkpoint tècnic**

- Objectiu: revisar el flux complet, deixar proves mínimes registrades i tancar un checkpoint tècnic abans de la sessió final de refactorització.
- Què explica el professorat: com usar la checklist de proves, quins casos s'han de poder mostrar i quina documentació mínima ha d'estar viva al `README`.
- Què modela el professorat: una prova curta del flux complet i una lectura ràpida de com la documentació ajuda a reproduir-lo.
- Què fa l'alumnat: executa casos correctes i incorrectes, registra incidències, actualitza `README` i deixa clar quines parts del codi es revisaran a la sessió `7`.
- Materials necessaris: checklist del Repte 2, guia de testing i debugging, fitxa del Repte 2 i materials comuns.
- Evidència esperada: proves mínimes, errors controlats, rastre de depuració, documentació actualitzada i demo breu reproduïble.
- Checkpoint: el professorat valida que la sessió `7` partirà d’un flux real i no d’una demo puntual.

**Bateria mínima obligatòria de prova**

La sessió `6` ha de deixar registrada una taula breu amb estos casos, encara que la forma siga manual, amb peticions guardades o amb proves automatitzades simples:

| Cas | Què comprova | Resultat esperat |
|---|---|---|
| cas vàlid | el flux complet accepta dades correctes i executa l'operació prevista | resposta correcta i dada reutilitzable dins del projecte |
| cas invàlid per validació | el servidor rebutja dades absents, mal formades o incoherents | error interpretable i possibilitat de correcció |
| cas no autenticat | una persona sense sessió vàlida intenta accedir a una part protegida | bloqueig, redirecció o resposta coherent |
| cas amb sessió caducada o estat invàlid | el sistema rep un estat que ja no hauria de permetre continuar | invalidació controlada i missatge o resposta coherent |
| cas d'accés a operació protegida | un usuari autenticat intenta una operació sotmesa a restricció de domini | permís o denegació segons la regla definida, no segons una ruta decorativa |

Cada cas ha d'incloure entrada, resultat esperat, resultat obtingut i incidència si n'hi ha. Si la IA ajuda a proposar proves, l'equip ha d'indicar quines accepta, quines descarta i què ha verificat manualment.

### Sessió 7. Microprojecte 7

**Refactorització, organització en fitxers i primer objecte del domini**

- Objectiu: revisar el codi que ja funciona, netejar-lo i justificar una millora de mantenibilitat que incorpore reutilització real, organització simple en fitxers i un primer objecte de domini, sense convertir esta fase en una reescriptura de `R3`.
- Què explica el professorat: com detectar duplicació, mescla excessiva de `HTML + PHP`, responsabilitats poc clares o noms millorables; per què no convé tindre-ho tot en un únic fitxer; per a què servixen `include` i `require`; diferència bàsica entre `include`, `require`, `include_once` i `require_once`; i per què una entitat mínima del domini dona més valor a la refactorització final.
- Què modela el professorat: una refactorització curta sobre una part del flux ja validat, extraient funcions comunes a un fitxer, important-les amb `require_once` o equivalent, introduint un objecte simple del domini i comprovant després que no hi ha regressió.
- Què fa l'alumnat: neteja una part rellevant del codi, extraïx funcions comunes a un fitxer separat, usa `include` / `require` amb sentit, ordena millor dades i renderitzat, representa almenys una entitat del projecte amb un objecte simple i justifica per què la versió revisada és millor.
- Materials necessaris: fitxa del Repte 2, full de treball del Repte 2, checklist del Repte 2, apunts reals del Repte 2, materials comuns i comparativa breu abans/després.
- Evidència esperada: reducció visible de duplicació o mescla innecessària, almenys un fitxer comú importat amb criteri, una entitat simple del domini recognoscible com a objecte, comparativa abans/després, justificació de la millora i comprovació final del flux.
- Checkpoint: el professorat valida que la refactorització aporta claredat, reutilització i millor organització sense desplaçar el nucli de `R3`.

La refactorització no s'ha de valorar només per “tindre més fitxers”. Ha de millorar almenys una responsabilitat concreta: validació, tractament de dades, comprovació d'accés, renderitzat, reutilització de missatges o representació d'una entitat del domini. La defensa breu ha d'explicar quin problema del codi inicial s'ha reduït, quin risc de regressió s'ha comprovat i quina part continua pendent per al treball arquitectònic de `R3`.

## Criteri metodològic de la sessió 7

Què sí pot incloure:

- netejar barreja excessiva de `HTML + PHP`
- extraure funcions útils a un fitxer separat
- usar `include` / `require` o, millor encara quan toque, `include_once` / `require_once`
- ordenar millor el codi
- millorar noms
- reduir duplicació
- separar millor preparació de dades i renderitzat
- incorporar una entitat mínima del domini com a objecte simple
- justificar per què la nova versió és més clara i mantenible

Què no ha de convertir-se en:

- entrada obligatòria a POO completa
- entrada obligatòria a BBDD com a focus central
- reescriptura arquitectònica total del repte
- arquitectura completa tipus `MVC`

Si apareixen més classes, més objectes o una persistència més formal, s'han de plantejar com a tast introductori, ampliació opcional o pont cap a `R3`.

## Evidències esperades per sessió

- Sessió `1`: formulari o entrada equivalent, recuperació real de dades i errors visibles.
- Sessió `2`: tractament executable, guardat funcional i primera reutilització de la informació correcta.
- Sessió `3`: decisió, regla o funció amb efecte real sobre el flux.
- Sessió `4`: estat recuperable, demostració d'invalidació i frontera clara entre estat i conservació funcional.
- Sessió `5`: operació del domini protegida amb cas autoritzat i cas denegat.
- Sessió `6`: checklist de prova, documentació mínima i checkpoint tècnic.
- Sessió `7`: comparativa breu abans/després, fitxer comú importat amb criteri, objecte simple del domini i comprovació final del flux.

## Moments de checkpoint

- Checkpoint curt `1`: al final de la sessió `2`, per comprovar que el flux ja rep, valida, processa i reutilitza dades.
- Checkpoint curt `2`: al final de la sessió `4`, per validar que estat, sessió o cookies no s'estan confonent amb persistència del domini.
- Checkpoint curt `3`: al final de la sessió `5`, per confirmar que hi ha una operació real protegida.
- Checkpoint tècnic `4`: al final de la sessió `6`, per confirmar que el flux és reproduïble, provat i documentat.
- Checkpoint de pas `R2 -> R3`: al final de la sessió `7`, per decidir si el grup entra al contrast de frameworks amb una base funcional i una primera millora de mantenibilitat defensable.

## Preparació del tancament del repte

- demanar una demo curta del flux complet, no només del login
- revisar que la informació correcta es recupera o es reutilitza dins del projecte
- exigir la bateria mínima de proves de la sessió `6`: cas vàlid, cas invàlid per validació, cas no autenticat, cas amb sessió caducada o estat invàlid i cas d'accés a operació protegida
- comprovar que la documentació mínima permet repetir la prova
- demanar una refactorització lleu sobre codi que ja funciona i una justificació breu del canvi
- demanar què haurà de reorganitzar-se en `R3` i què encara continua sent suport funcional de `R2`

## Criteri pràctic de tancament

`R2` queda preparat quan el professorat pot veure un flux complet de dades, lògica, estat i autenticació sobre la base comuna en `PHP`, amb una operació real protegida, proves mínimes reproduïbles, una sessió final de refactorització amb millora de mantenibilitat justificable i un pas net cap a `R3`.

La sessió `7` ha de demostrar que el codi queda una mica més clar i mantenible sense convertir el repte en una reescriptura arquitectònica completa.
