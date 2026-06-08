# R2S6. Proves, depuracio i checkpoint tecnic

## Finalitat de la sessio

Esta sessio comprova el flux complet de `R2`: entrada, validacio, reintent, guardat funcional, regla del projecte, estat i operacio protegida. El focus és provar, depurar, documentar i deixar una demo reproduïble abans de refactoritzar.

L'objectiu no és afegir funcionalitats noves, sinó demostrar que el que ja existeix funciona amb casos positius, negatius i d'invalidacio.

## Encaix dins del Repte 2

- **Repte**: `R2. Processament bàsic, estat, autenticació i primera funcionalitat protegida`
- **Microrepte**: `R2M6`
- **Sessio**: `R2S6`
- **Duracio orientativa**: `3 hores`
- **Focus**: checklist de proves, depuracio, documentacio i demo reproduïble
- **No entra encara**: refactoritzacio profunda, noves pantalles grans o migracio a framework

## Relacio amb RA i criteris de treball

| Element | Concrecio en el microrepte |
|---|---|
| `RA4.f` | prova, depuracio i documentacio del comportament real |
| Evidencia central | taula de proves executada i README actualitzat |
| Verificacio docent | execucio d'un cas triat pel professorat i contrast amb documentacio |

## Producte esperat

Una bateria mínima de proves amb:

- cas vàlid;
- cas invàlid per validacio;
- reintent amb dades conservades;
- regla del projecte amb dos resultats;
- estat recuperat i invalidat;
- accés no autenticat denegat;
- accés autenticat permés;
- logout o invalidacio i nou intent denegat;
- incidencies detectades o confirmacio explícita que no n'hi ha;
- README o guia de reproduccio actualitzada.

## Preparacio previa del professorat

Convé preparar:

- plantilla de taula amb entrada, passos, resultat esperat, resultat real i incidencia;
- exemple d'ús de navegador, terminal, logs, `curl` o eina equivalent;
- criteri de prioritzacio d'incidencies bloquejants;
- recordatori que primer es reprodueix l'error i després es corregeix.

## Seqüencia d'aula de 3 hores

### 0:00-0:25. Bateria mínima comuna

Presentar la bateria i els camps de registre.

Resultat: cada equip té una taula o checklist preparada.

### 0:25-0:45. Modelatge de registre i depuracio

Mostrar com anotar:

- entrada;
- passos;
- resultat esperat;
- resultat real;
- incidencia;
- correccio i nova prova.

Resultat: l'alumnat sap què vol dir provar de manera reproduïble.

### 0:45-1:35. Execucio de proves

Tasques:

- executar els casos mínims;
- registrar resultat real;
- marcar bloquejos;
- capturar o descriure evidencies si cal.

Resultat: hi ha una primera bateria executada.

### 1:35-2:15. Depuracio guiada

Tasques:

- corregir primer errors que trenquen el flux;
- repetir el cas fallit;
- deixar constancia de la correccio;
- no obrir funcionalitats noves.

Resultat: els bloquejos principals queden resolts o documentats.

### 2:15-2:40. Documentacio mínima

Tasques:

- actualitzar `README`;
- afegir usuaris de prova;
- indicar operacio protegida;
- indicar com provocar error, cas correcte i denegacio;
- marcar zona candidata a refactoritzar en `R2M7`.

Resultat: la demo és reproduïble.

### 2:40-3:00. Checkpoint tecnic

El professorat tria un cas de la taula i demana executar-lo.

Pregunta: quins casos demostren que el flux complet és reproduïble amb errors, estat i permisos controlats?

## Tasques concretes de l'alumnat

- Preparar checklist o taula de proves.
- Executar casos positius i negatius.
- Registrar incidencies.
- Depurar bloquejos.
- Repetir proves fallides.
- Actualitzar README.
- Marcar una zona per a `R2M7`.

## Evidencies minimes

| Evidencia | Minim acceptable |
|---|---|
| Taula | casos amb entrada, passos i resultats |
| Cas vàlid | flux accepta dades correctes |
| Cas invàlid | error interpretable i correccio |
| Estat | recuperacio i invalidacio provades |
| Auth | cas no autenticat i autenticat |
| Incidencies | errors registrats o absencia explícita |
| README | demo reproduïble |

## Criteris d'exit

- No es prova només el camí feliç.
- La documentacio permet repetir la demo.
- Els casos registrats coincideixen amb el comportament real.
- Els errors bloquejants estan corregits o identificats.
- Hi ha una zona concreta per refactoritzar.

## Que no és suficient

- Llista de proves sense executar.
- Captures sense passos.
- README desactualitzat.
- Corregir sense reproduir.
- Afegir funcionalitats noves en lloc de tancar el flux.

## Us de la IA

La IA pot ajudar a generar casos addicionals o interpretar errors. Control: la bateria mínima comuna ha d'estar executada i els resultats han de ser reals, no només generats.

## Suport per alumnat amb més dificultat

Reduir a cinc casos: vàlid, invàlid, estat invalidat, no autenticat i autenticat. Exigir passos clars i resultat real.

## Ampliacio per alumnat avançat

- Proves automatitzades simples.
- Col·leccio de peticions.
- Logs o captures comparatives.
- Matriu d'incidencies prioritzades.

## Checklist de tancament

- [ ] He executat cas vàlid.
- [ ] He executat cas invàlid.
- [ ] He provat reintent.
- [ ] He provat estat i invalidacio.
- [ ] He provat accés denegat.
- [ ] He provat accés permés.
- [ ] He registrat incidencies.
- [ ] He actualitzat README.
- [ ] He triat zona per a refactoritzar.

## Connexio amb R2M7

`R2M7` parteix d'un flux provat. La pregunta de pas és:

Quina part del codi funciona però és més difícil de mantindre del que hauria?

