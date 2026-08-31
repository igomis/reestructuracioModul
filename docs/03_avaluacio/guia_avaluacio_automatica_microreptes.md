# Guia d'avaluació automàtica dels microreptes

## Classificació documental

Este és un **document canònic d'ús docent**. Regula com s'ha d'utilitzar el projecte `dwes-microreptes-autocorreccio` dins del sistema d'avaluació del mòdul. Depén del [Sistema d'evidències](sistema_evidencies.md), de la [Rúbrica base dels reptes](rubrica_base_reptes.md), dels [Instruments de seguiment docent](instruments_seguiment_docent.md) i del document [Ús de la IA per a professorat i alumnat](../us-ia-professorat-i-alumnat.md).

No substituïx la decisió docent final. L'autocorrecció dona una lectura provisional, traçable i revisable del treball lliurat per l'alumnat.

## Finalitat

L'avaluació automàtica servix per revisar de manera sistemàtica els microreptes, detectar evidències absents, donar feedback ràpid i prioritzar la revisió docent. El seu valor principal és reduir arbitrarietat i temps de triatge, no convertir la qualificació en un procés opac.

El professorat ha d'usar-la per respondre quatre preguntes:

- l'alumne ha deixat el microrepte localitzable i revisable?
- les evidències mínimes demanades apareixen al repositori?
- el treball sembla coherent amb la rúbrica del microrepte?
- cal revisió docent abans de donar per bona la nota provisional?

## Paper de cada repositori

| Repositori | Funció dins de l'avaluació |
|---|---|
| `dwes-restructuracio-modul` | Defineix criteri docent, RA/CA, seqüència, evidències i ús correcte dels instruments. |
| `dwes-documentacio-alumnat` | Explica a l'alumnat què ha de fer, què ha d'entregar i com es valorarà. |
| `dwes-microreptes-autocorreccio` | Conté `challenge.json`, `rubric.json`, `prompt.md`, polítiques globals, scripts i workflows d'autocorrecció. |
| `dwes-microreptes-alumnes` | Dona l'estructura base perquè cada alumne deixe codi, documentació, proves i evidències revisables. |

La regla de coherència és estricta: l'autocorrecció no pot penalitzar res que no s'haja demanat a l'alumnat ni estiga previst en la programació d'aula.

## Flux ordinari de treball

### 1. Abans de llançar la correcció

El professorat comprova:

- quin microrepte està actiu per a cada grup en `course/active-challenges.json`;
- que el microrepte existeix en `dwes-microreptes-autocorreccio/microreptes/`;
- que `challenge.json`, `rubric.json`, `prompt.md`, `expected/README.md` i `tests/README.md` descriuen el mateix abast;
- que la documentació d'alumnat demana les mateixes evidències que després es revisaran;
- que la llista de repositoris d'alumnes està actualitzada en `course/student-repositories*.txt`;
- que la branca ordinària corregible és `main`.

Si algun alumne té una recuperació o incidència, es pot corregir un `challenge_id` o una branca concreta, però ha de quedar registrat com a excepció docent.

### 2. Llançament de la correcció

La via ordinària és usar el workflow o el dashboard del projecte d'autocorrecció.

Opcions recomanades:

- `mode = mock` per comprovar que la tanda pot executar-se sense consum d'IA;
- `mode = openai` per generar feedback real amb IA;
- `target_group` per corregir un grup complet;
- `repositories` per corregir un alumne o una tanda puntual;
- `challenge_id` buit per usar la configuració activa;
- `challenge_id` explícit per a una correcció puntual pactada.

L'execució recull senyals del repositori de l'alumne, construeix el payload d'avaluació, aplica la rúbrica i publica el resultat en `autograde/latest.md` i `autograde/latest.json`.

### 3. Lectura docent del resultat

El resultat s'ha de llegir en este ordre:

1. **Flags i revisió docent requerida.** Si el sistema marca baixa confiança, absència d'evidències o possible incoherència, la nota no s'ha d'aplicar automàticament.
2. **Evidències detectades.** Cal comprovar si el repositori conté `README`, codi, proves, documentació, evidències i `AI log` quan pertoque.
3. **Dimensions de rúbrica.** La puntuació per dimensions ajuda a saber què revisar: funcionalitat, traçabilitat, proves, documentació, autoria o ús d'IA.
4. **Feedback textual.** Servix per orientar l'alumne, però no substituïx la comprovació docent quan hi ha dubte.
5. **Historial.** Si hi ha diverses correccions, compta la versió vigent de `grades/latest-grades.*`, però les execucions anteriors es poden consultar en `grades/history/`.

## Criteri de qualificació

La nota generada és provisional. Es pot acceptar directament només quan es complixen estes condicions:

- el microrepte corregit és el que tocava;
- el repositori és el de l'alumne correcte;
- la branca corregida és `main` o una excepció registrada;
- no hi ha flags greus;
- les evidències mínimes són localitzables;
- el feedback és coherent amb el que el professorat veu al repositori.

Cal revisió docent obligatòria quan aparega qualsevol d'estos casos:

- nota alta amb evidències pobres o no reproduïbles;
- nota baixa causada per problema tècnic del workflow, clonació o configuració;
- `README` absent o genèric que no identifica el microrepte;
- codi aparentment complet però sense proves, passos d'execució ni explicació;
- ús d'IA no registrat quan el treball mostra dependència clara d'IA;
- diferències entre el que demana l'enunciat i el que avalua la rúbrica;
- alumne en recuperació, adaptació o entrega fora del flux ordinari.

## Com convertir el resultat en acció docent

| Senyal del resultat | Acció del professorat |
|---|---|
| Evidències completes i feedback coherent | Acceptar nota provisional o fer revisió lleugera. |
| Falta `README` o instruccions de prova | Demanar correcció documental abans de tornar a avaluar. |
| Funcionalitat present però no executable | Obrir incidència de verificació i demanar passos reproduïbles. |
| Baixa confiança del corrector | Revisar manualment repositori i rúbrica abans de qualificar. |
| Possible delegació excessiva d'IA | Activar defensa curta i contrastar autoria, decisions i proves. |
| Divergència entre rúbrica i documentació d'alumnat | Aturar l'aplicació automàtica i corregir la font de veritat afectada. |

## Revisió per microrepte

Per cada microrepte ordinari, abans de donar-lo per implantat, ha d'existir esta cadena:

| Peça | Pregunta de control |
|---|---|
| Programació d'aula | La sessió explica què es treballa, què s'entrega i què és suficient? |
| Documentació d'alumnat | L'alumne pot entendre què ha de fer i com serà valorat? |
| Autocorrecció | La rúbrica revisa només evidències demanades i observables? |
| Repositori d'alumne | L'estructura permet localitzar entrega, proves, evidències i decisions? |
| Resultat publicat | El feedback ajuda a millorar sense amagar el criteri docent? |

## Ús de la IA en la correcció

La IA pot ajudar a interpretar evidències textuals, detectar incoherències i redactar feedback. No pot resoldre sola autoria, comprensió real ni validesa curricular.

El professorat ha de mantindre estos límits:

- no usar una puntuació automàtica com a única evidència d'acreditació;
- no penalitzar l'ús d'IA si està registrat, verificat i defensat;
- sí penalitzar la delegació excessiva quan l'alumne no pot explicar, provar o modificar el treball;
- revisar manualment qualsevol cas amb flags de confiança, autoria o evidències insuficients.

## Checklist curta per a una tanda

- [ ] He revisat el microrepte actiu en `course/active-challenges.json`.
- [ ] He comprovat que la documentació d'alumnat i la rúbrica demanen el mateix.
- [ ] He actualitzat la llista de repositoris del grup.
- [ ] He fet una prova en `mode = mock` si és una tanda nova o sensible.
- [ ] He llançat la correcció real només quan la configuració era coherent.
- [ ] He revisat flags, evidències i casos de baixa confiança.
- [ ] He registrat excepcions, recuperacions o revisions manuals.
- [ ] He comunicat a l'alumnat què ha de corregir abans d'una nova passada.

## Resultat esperat

Una tanda d'autocorrecció ben usada deixa tres productes útils:

- feedback llegible per a l'alumne en el seu repositori;
- registre central de notes provisionals i històric de tandes;
- criteri docent més clar per decidir acceptació, revisió, recuperació o defensa.

La responsabilitat final continua sent docent: l'autocorrecció accelera la revisió, però l'acreditació es basa en evidències, coherència curricular i capacitat de defensa individual.
