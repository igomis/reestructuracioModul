# R1. Programació d'aula — Kickoff backend

## Finalitat del document

Este document baixa `R1` a una seqüència operativa d'aula perquè el professorat puga conduir l'arrancada del backend sense inflar el repte ni confondre infraestructura amb producte.

La programació manté els `4` microreptes com a unitats de progrés, però cada microrepte queda redactat com una unitat d'aula executable. Si el centre compacta el repte en `2` sessions de `3` hores, el docent pot executar `MP1` i l'inici de `MP2` en la primera sessió, i el tancament de `MP2`, `MP3` i `MP4` en la segona. Si el grup necessita més temps, `MP4` pot convertir-se en una tercera sessió formal de defensa i checkpoint.

## Finalitat del repte

- entendre el model client/servidor aplicat al producte del curs
- distingir els models d'execució de codi en client web i servidor
- assumir una base tècnica guiada sobre `Docker`, `PHP` i servidor web
- posar en marxa una base executable mínima i reproduïble
- adaptar-la al projecte propi i completar-la amb base de dades i phpMyAdmin
- deixar un primer punt d'entrada funcional del backend
- documentar i verificar la base creada
- preparar un pas net cap a `R2`

## Relació entre microreptes i sessions

| Sessió base | Duració | Microreptes implicats | Focus principal | Evidència clau |
|---|---:|---|---|---|
| `1` | `3h` | `MP1` + inici de `MP2` | model client/servidor, decisió inicial i arrencada de l'entorn | fitxa inicial, explicació client vs servidor, decisió tècnica i base mínima començada |
| `2` | `3h` | tancament de `MP2` + `MP3` + `MP4` | entorn complet, primera funcionalitat mínima i documentació del repte | entorn arrancable, punt d'entrada funcional, README i documentació en repositori |
| `3` | opcional | reforç de `MP4` | defensa, execució real i revisió de traçabilitat | defensa tècnica o acta de checkpoint |

## Mapa de criteris d'avaluació per microrepte

| Microrepte | Focus | CA associats |
|---|---|---|
| `MP1` | model client/servidor i decisió tècnica inicial | `RA1a`, `RA1b`, `RA1c`, `RA1g` |
| `MP2` | base executable amb Docker, PHP, servidor web, BBDD i phpMyAdmin | `RA1c`, `RA1d`, `RA1e`, `RA1f` |
| `MP3` | primer punt d'entrada funcional del backend | `RA1b`, `RA1e`, `RA1f` |
| `MP4` | documentació tècnica, verificació i checkpoint | `RA1d`, `RA1g` |

## MP1 — Model client/servidor i decisió tècnica inicial

### Objectiu operatiu

Al final de la unitat, cada alumne o parella ha de poder explicar, sobre el seu producte, què s'executarà al navegador, què s'executarà al servidor, quin paper tindrà el backend i amb quina base tècnica inicial començarà el repte.

### Relació amb RA

- `RA1a`: diferenciació dels models d'execució en servidor i client web.
- `RA1b`: identificació inicial del valor de generar respostes dinàmiques des del servidor.
- `RA1c`: reconeixement dels mecanismes d'execució de codi en servidor web.
- `RA1g`: exploració guiada d'eines i frameworks de programació en entorn servidor.

### Criteris d'èxit visibles

- La fitxa d'exploració tècnica inicial està completa i no és una llista genèrica d'eines.
- El repartiment client/servidor està escrit amb exemples del producte propi.
- La decisió tècnica inicial inclou una opció preferent, una alternativa descartada i un dubte o límit real.
- L'alumne pot respondre oralment: "què passa al navegador?" i "què passa al servidor?" sense llegir la fitxa.

### Seqüència temporal de la unitat

- `0:00-0:10`: obertura del repte. El professorat mostra el producte final esperat de `R1`: repo, entorn, primer punt d'entrada i documentació.
- `0:10-0:25`: explicació guiada del flux client/servidor amb un exemple concret: navegador demana una URL, servidor executa codi, servidor retorna resposta, navegador la mostra.
- `0:25-0:40`: modelatge docent de la fitxa. El professorat ompli en veu alta un cas simple, per exemple una agenda, una reserva o un catàleg.
- `0:40-1:10`: treball individual inicial. Cada alumne escriu el repartiment client/servidor del seu producte i identifica tecnologies de client i servidor.
- `1:10-1:30`: contrast per parelles. Cada alumne explica el seu repartiment i l'altra persona marca una incoherència o pregunta pendent.
- `1:30-1:55`: exploració guiada d'opcions. L'alumnat consulta materials del curs i, si usa IA, demana diferències bàsiques entre opcions com `PHP`, `Laravel`, `Symfony` o `NestJS` dins del marc docent.
- `1:55-2:20`: decisió tècnica inicial. Cada parella tanca una opció de partida i una alternativa descartada amb un motiu curt.
- `2:20-2:45`: posada en comú curta. Tres o quatre equips expliquen el repartiment client/servidor i el professorat corregeix confusions.
- `2:45-3:00`: checkpoint `CP-R1.1`. El professorat revisa fitxes, fa una pregunta oral i marca qui pot passar a iniciar `MP2`.

Si esta unitat es compacta dins de la sessió `1`, el docent pot reduir la posada en comú a `10` minuts i iniciar `MP2` immediatament després.

### Modelatge docent

El professorat mostra una fitxa ja començada i verbalitza decisions reals:

- "El client mostrarà el formulari i farà interaccions visuals simples."
- "El servidor rebrà la petició, executarà codi `PHP` i prepararà la resposta."
- "Encara no obrim autenticació ni persistència completa; això vindrà després."
- "Trie esta base perquè és assumible per al curs i perquè després podrà créixer cap a sessions, dades i API."

També modela una mala resposta i la corregeix: "Usarem Laravel perquè és popular" no és suficient; cal dir quin problema resol, què aporta al backend i per què és assumible ara.

### Tasques concretes de l'alumnat

- Escriure el producte que vol iniciar i una frase sobre el paper del backend.
- Completar la taula de tecnologies de client i servidor.
- Redactar `3` exemples del seu producte: una acció del client, una acció del servidor i una resposta generada.
- Comparar de manera curta `2` o `3` opcions tècniques dins del marc del curs.
- Tancar una primera decisió tècnica orientativa.
- Registrar un dubte tècnic que encara no haja quedat resolt.

### Cooperatiu estructurat o responsabilitat individual

- Treball individual: cada alumne ha de poder explicar el model d'execució encara que treballe en parella.
- Parella de contrast: una persona fa de "client" i pregunta què veu o envia; l'altra fa de "servidor" i explica què rep, executa i retorna. Després intercanvien rols.
- Responsabilitat mínima individual: cada alumne respon una pregunta oral del docent o deixa un àudio/text breu de `4-5` línies amb el seu repartiment client/servidor.

### Evidència observable

- `fitxa_exploracio_tecnica_inicial.md` o document equivalent completat.
- Explicació escrita del model client/servidor aplicada al producte.
- Decisió tècnica inicial amb alternativa descartada.
- Dubte o límit tècnic registrat.

### Mecanisme de verificació

El professorat revisa en `2-3` minuts:

- si la fitxa parla del producte concret o només d'eines;
- si l'alumne diferencia navegador, servidor web, runtime i backend;
- si la decisió inicial és coherent amb el curs;
- si pot respondre oralment una pregunta de transferència: "quina part canviaria si el client fora una app mòbil i no un navegador?"

### Ús de la IA i control

La IA està permesa per explorar diferències entre tecnologies i ajudar a formular dubtes. L'alumnat ha d'indicar en la fitxa si l'ha usada i què ha verificat amb materials del curs o amb explicació pròpia.

No s'accepta substituir la fitxa per captures de conversa. El control es fa amb pregunta oral i amb una revisió de coherència: si la fitxa usa conceptes que l'alumne no pot explicar, cal reescriure-la amb llenguatge propi.

### Dificultats habituals i plans B

- Dificultat: l'alumnat confon frontend amb navegador i backend amb base de dades. Pla B: tornar a un flux de petició-resposta dibuixat en quatre caixes: navegador, servidor web, `PHP`, dades.
- Dificultat: la comparativa de frameworks es fa massa llarga. Pla B: limitar a `2` opcions i obligar a escriure només avantatge, límit i encaix amb el curs.
- Dificultat: decisió per moda o preferència. Pla B: demanar que la decisió responga a tres criteris: arranca en local, es pot explicar i prepara `R2`.
- Dificultat: ús d'IA massa abstracte. Pla B: demanar una reformulació manual de `5` línies sense IA i una pregunta oral immediata.

## MP2 — Base executable amb Docker, PHP, servidor web, BBDD i phpMyAdmin

### Objectiu operatiu

Al final de la unitat, el projecte ha d'arrancar en local amb un entorn reproduïble, adaptat al producte propi, amb `PHP`, servidor web, base de dades i phpMyAdmin identificables, i amb un `README` inicial que permeta repetir l'arrencada.

### Relació amb RA

- `RA1c`: identificació del mecanisme d'execució de codi en servidor web.
- `RA1d`: reconeixement de la integració entre servidor d'aplicacions, servidor web i serveis auxiliars.
- `RA1e`: caracterització de tecnologies de programació web en entorn servidor.
- `RA1f`: verificació inicial de la integració entre resposta web i codi de servidor.

### Criteris d'èxit visibles

- El repositori té estructura mínima, issue mare i primers commits significatius.
- `docker compose up` o equivalent arranca els serveis definits.
- El `README` diu com arrancar, com parar i com comprovar cada servei.
- El projecte no és una còpia plana: nom, ports, estructura o resposta inicial estan adaptats.
- L'alumne pot explicar què fa cada servei: servidor web, `PHP`, base de dades i phpMyAdmin.

### Seqüència temporal de la unitat

- `0:00-0:15`: recuperació de `MP1`. Cada equip obri la fitxa i diu amb quina base començarà.
- `0:15-0:35`: modelatge docent d'un entorn mínim. El professorat mostra fitxers, serveis i ordre d'arrencada sense entregar una solució final tancada.
- `0:35-0:55`: creació o revisió del repositori. L'alumnat crea issue mare de kickoff, estructura bàsica i primer commit.
- `0:55-1:35`: adaptació de l'entorn mínim. Cada equip ajusta nom del projecte, carpeta pública, port, servei web i resposta inicial.
- `1:35-2:05`: completació amb base de dades i phpMyAdmin. L'alumnat incorpora serveis, variables bàsiques i comprovació d'accés.
- `2:05-2:25`: redacció del `README` inicial amb passos reals d'arrencada i verificació.
- `2:25-2:45`: prova creuada. Una altra parella intenta seguir el `README` o llig els passos i detecta omissions.
- `2:45-3:00`: checkpoint `CP-R1.2`. El professorat comprova arrencada o, si no és possible per temps, revisa error, log i pla de correcció.

Si `MP2` queda partit entre sessions, la primera sessió tanca com a mínim repositori, estructura i entorn començat; la segona comença amb arrencada real i completació de BBDD/phpMyAdmin.

### Modelatge docent

El professorat projecta una execució mínima i verbalitza:

- quin fitxer defineix els serveis;
- quin servei rep la petició HTTP;
- on s'executa `PHP`;
- com es comprova que la base de dades està disponible;
- per què phpMyAdmin és una eina de gestió i no "la base de dades";
- com escriure un `README` que no amague passos.

El modelatge inclou un error controlat, per exemple un port ocupat o una variable mal escrita, i mostra com llegir el missatge abans de demanar ajuda a la IA.

### Tasques concretes de l'alumnat

- Crear o netejar el repositori del projecte.
- Obrir issue mare de `R1` amb microtasques de MP2, MP3 i MP4.
- Crear o adaptar `docker-compose.yml` o configuració equivalent.
- Definir servei web, execució de `PHP`, base de dades i phpMyAdmin.
- Fer una primera prova d'arrencada i registrar resultat.
- Escriure `README` inicial amb requisits, arrencada, comprovació i parada.
- Fer un commit amb missatge significatiu.
- Registrar una incidència o decisió tècnica curta: port canviat, nom de servei, estructura de carpetes o error resolt.

### Cooperatiu estructurat o responsabilitat individual

- Rols de parella durant `30` minuts: "pilot" toca fitxers i terminal; "navegant" llig errors, comprova README i anota decisions. Canvi de rol a mitja unitat.
- Revisió creuada: una altra parella ha de dir si podria arrancar el projecte només amb el `README`.
- Responsabilitat individual: cada alumne explica un servei diferent de l'entorn i què passaria si no arrancara.

### Evidència observable

- Repositori amb issue mare i commits.
- Fitxers d'entorn adaptats.
- Serveis arrancables o error documentat amb pla de correcció.
- `README` inicial executable.
- Incidència, dubte o decisió tècnica registrada.

### Mecanisme de verificació

El docent usa una comprovació curta:

- executar o observar `docker compose up`;
- obrir la URL del servei web;
- obrir phpMyAdmin o comprovar que el servei està definit i accessible;
- llegir el `README` i buscar passos ocults;
- demanar a l'alumne que explique què ha adaptat respecte del model docent.

Si l'entorn no arranca, no es dona per perdut el treball: l'evidència mínima passa a ser log d'error, hipòtesi de causa, canvi intentat i pròxima acció concreta.

### Ús de la IA i control

La IA pot ajudar a diagnosticar errors de configuració, explicar missatges de Docker o proposar fragments. L'alumnat ha de copiar al `AI log` o al registre de treball només les consultes rellevants i, sobretot, la verificació feta després.

Control docent:

- demanar que l'alumne explique una línia concreta de la configuració;
- demanar un microcanvi en viu, com canviar un missatge o un port documentat;
- comparar el `README` amb l'execució real.

### Dificultats habituals i plans B

- Dificultat: Docker no arranca per port ocupat. Pla B: canviar port, documentar-lo i comprovar que el `README` reflectix el canvi.
- Dificultat: l'equip copia una configuració que no sap explicar. Pla B: reduir a serveis mínims i fer una taula "servei, per a què servix, com el comprove".
- Dificultat: base de dades i phpMyAdmin apareixen però no es comproven. Pla B: exigir una prova visible d'accés o un log de servei correcte.
- Dificultat: massa temps en estructura perfecta. Pla B: congelar carpetes i tancar només arrencada, comprovació i documentació.

## MP3 — Primer punt d'entrada funcional del backend

### Objectiu operatiu

Al final de la unitat, el backend ha de respondre amb una primera peça funcional simple i coherent amb el producte: una ruta, vista, endpoint, landing mínima o healthcheck que es puga executar i explicar.

### Relació amb RA

- `RA1b`: reconeixement del valor de generar una resposta dinàmica des del servidor.
- `RA1e`: ús inicial d'una tecnologia de servidor per produir comportament observable.
- `RA1f`: integració entre codi de servidor i resposta web o equivalent.

### Criteris d'èxit visibles

- Hi ha una URL, ruta o endpoint que respon en execució.
- La resposta no és només decorativa: fa referència al producte o al seu estat inicial.
- El punt d'entrada està documentat al `README`.
- L'alumne pot explicar quin fitxer intervé i què passa quan s'accedeix a la ruta.
- Hi ha un commit associat a la funcionalitat.

### Seqüència temporal de la unitat

- `0:00-0:10`: recordatori del criteri "infraestructura no és funcionalitat".
- `0:10-0:25`: modelatge docent d'una resposta mínima: ruta `/`, `/health` o pàgina inicial que mostra nom del producte, estat i pròxim flux.
- `0:25-0:45`: decisió de l'equip. Cada parella tria quin punt d'entrada farà i escriu què ha de demostrar.
- `0:45-1:30`: implementació guiada. L'alumnat crea o adapta el fitxer de resposta i comprova l'execució.
- `1:30-1:50`: prova funcional. Cada equip obri la ruta, captura o registra resultat i anota com es comprova.
- `1:50-2:10`: microcanvi en viu. L'equip modifica un text, estat o dada simple i comprova que la resposta canvia.
- `2:10-2:35`: documentació. S'afegeix al `README` la ruta, què mostra i com provar-la.
- `2:35-3:00`: checkpoint `CP-R1.3`. El docent revisa una demo curta i fa una pregunta sobre el flux servidor.

Si esta unitat es compacta amb `MP2` i `MP4`, el docent pot reduir la implementació a una única ruta i reservar `20` minuts finals per documentar i verificar.

### Modelatge docent

El professorat mostra una primera resposta funcional i assenyala:

- URL que es demana;
- fitxer o controlador que respon;
- codi que s'executa al servidor;
- resposta que rep el navegador;
- diferència entre una maqueta estàtica i una resposta servida pel backend.

El docent fa un microcanvi en directe, refresca el navegador i mostra que la resposta ve del codi del servidor.

### Tasques concretes de l'alumnat

- Triar una opció mínima: `/`, `/health`, `/estat`, landing inicial o endpoint bàsic.
- Escriure una resposta connectada amb el producte: nom, propòsit, estat inicial o pròxim flux.
- Fer que la resposta siga visible en execució local.
- Registrar una prova: captura, log, URL o instrucció de comprovació.
- Actualitzar el `README` amb el punt d'entrada.
- Fer commit de la funcionalitat.

### Cooperatiu estructurat o responsabilitat individual

- Parella: una persona implementa i l'altra prepara la prova i la pregunta de defensa.
- Revisió ràpida entre parelles: l'equip visitant ha de poder obrir la ruta i dir què demostra.
- Responsabilitat individual: cada alumne explica una part del flux: petició, execució o resposta.

### Evidència observable

- Ruta, vista, endpoint o healthcheck funcional.
- Prova visible de la resposta.
- `README` actualitzat amb instrucció de comprovació.
- Commit associat.

### Mecanisme de verificació

El docent comprova:

- la ruta en execució;
- que la resposta canvia si es fa un microcanvi controlat;
- que el `README` indica com provar-la;
- que l'alumne pot explicar què passa al servidor quan entra la petició.

### Ús de la IA i control

La IA pot suggerir l'esquelet de la ruta o ajudar amb errors sintàctics. El control és la prova en directe i el microcanvi: si l'alumne no pot modificar una línia simple i predir el resultat, la funcionalitat no es considera defensada.

### Dificultats habituals i plans B

- Dificultat: l'equip fa només una pàgina estàtica sense execució de servidor. Pla B: convertir-la en una resposta servida des de l'entorn `PHP` i demostrar el canvi en viu.
- Dificultat: volen començar formularis, login o persistència. Pla B: retallar a una ruta d'estat o landing funcional i deixar el flux per a `R2`.
- Dificultat: la ruta funciona però no està documentada. Pla B: parar implementació i escriure tres línies al `README`: URL, què mostra i com comprovar-la.
- Dificultat: error tècnic bloquejant. Pla B: fer `/health` amb resposta mínima i registrar el bloqueig del punt més ambiciós.

## MP4 — Documentació, verificació i checkpoint de pas a R2

### Objectiu operatiu

Al final de la unitat, el repte ha de quedar verificat i defensable: una altra persona ha de poder localitzar la documentació, arrancar el projecte amb el `README`, comprovar el punt d'entrada i entendre quines decisions preparen el pas a `R2`.

### Relació amb RA

- `RA1d`: explicació de la integració entre serveis de l'entorn.
- `RA1g`: justificació de les eines triades a partir de l'experiència real del kickoff.

### Criteris d'èxit visibles

- El `README` executa el projecte sense passos ocults.
- Hi ha directori de documentació dins del repositori amb fitxes o documents del repte.
- Un índex o pàgina visible enllaça la documentació.
- Hi ha justificació tècnica curta o ADR inicial.
- La defensa oral mostra comprensió, no lectura memorística.
- L'ús de IA, si n'hi ha, queda registrat i verificat.

### Seqüència temporal de la unitat

- `0:00-0:15`: llistat de tancament. El professorat mostra la checklist final: arrencada, punt d'entrada, README, docs, decisió i defensa.
- `0:15-0:40`: revisió del `README`. L'alumnat comprova requisits, arrencada, parada, serveis i ruta funcional.
- `0:40-1:05`: organització documental. Es crea directori de documentació, s'incorpora la fitxa de `MP1`, la decisió tècnica i les incidències.
- `1:05-1:25`: índex o pàgina visible. L'equip enllaça els documents perquè el professorat els puga trobar sense buscar manualment.
- `1:25-1:50`: preparació de defensa. Cada alumne prepara una explicació de `2` minuts: decisió, entorn, punt d'entrada, verificació i pas a `R2`.
- `1:50-2:25`: checkpoint per mostreig o per torns curts. El docent executa README, obri ruta i fa preguntes de transferència.
- `2:25-2:45`: correcció immediata de buits: passos que falten, enllaços trencats, documentació incoherent o AI log absent.
- `2:45-3:00`: tancament. Cada equip escriu què queda pendent per a `R2` i quin primer flux voldrà protegir o ampliar.

Si hi ha poc temps, esta unitat pot convertir-se en sessió `3` opcional. No convé eliminar-la: sense verificació i defensa, `R1` queda incomplet.

### Modelatge docent

El professorat agafa un repo d'exemple i fa la revisió com ho faria al checkpoint:

- obri el `README`;
- executa els passos indicats;
- comprova serveis;
- obri el punt d'entrada;
- localitza la fitxa inicial i la decisió tècnica;
- fa una pregunta sobre una alternativa descartada;
- demana quin pas natural connecta amb `R2`.

El docent mostra també un README insuficient i el corregeix: substitueix frases generals per ordres reals, URLs, comprovacions i criteris de resultat esperat.

### Tasques concretes de l'alumnat

- Revisar el `README` amb una prova real.
- Crear o ordenar `docs/`, `documentacio/` o carpeta equivalent dins del repositori del projecte.
- Incorporar fitxa d'exploració, decisió tècnica, incidència o bloqueig i comprovació d'arrencada.
- Crear un índex que enllace els documents del repte.
- Escriure una justificació tècnica curta o ADR inicial.
- Completar AI log si s'ha usat IA de manera rellevant.
- Preparar i fer defensa tècnica breu.

### Cooperatiu estructurat o responsabilitat individual

- Parella: una persona fa de revisora del `README` i l'altra fa de responsable de documentació; després intercanvien tasques.
- Revisió creuada: un altre equip intenta localitzar documentació i punt d'entrada en menys de `3` minuts.
- Responsabilitat individual: cada alumne defensa una decisió o explica una part de l'entorn sense suport de la parella.

### Evidència observable

- `README` final executable.
- Directori de documentació amb fitxes i decisions.
- Índex o pàgina visible amb enllaços.
- Justificació tècnica o ADR curt.
- Registre d'incidències i verificacions.
- AI log quan corresponga.
- Defensa oral o acta de checkpoint.

### Mecanisme de verificació

El checkpoint docent inclou:

- arrancar o revisar l'arrencada seguint només el `README`;
- obrir el punt d'entrada funcional;
- comprovar que la documentació es localitza des d'un índex;
- contrastar decisió tècnica, commits i resultat final;
- fer una pregunta individual sobre el paper de cada servei;
- demanar el primer pas tècnic previst per a `R2`.

### Ús de la IA i control

La IA pot ajudar a polir el `README`, resumir la decisió tècnica o revisar claredat. El control consisteix a comparar el text amb el sistema real: qualsevol instrucció generada que no funcione s'ha de corregir abans del tancament.

La defensa no es pot delegar. Si l'alumne no pot explicar una decisió, ha de simplificar la documentació i reescriure-la amb llenguatge propi.

### Dificultats habituals i plans B

- Dificultat: README bonic però no executable. Pla B: substituir-lo per una checklist curta amb ordres, URL i resultat esperat.
- Dificultat: documentació dispersa o fora del repo. Pla B: crear un directori únic i un índex amb `4` enllaços mínims.
- Dificultat: defensa memorística. Pla B: fer preguntes sobre el repo o demanar un microcanvi en viu.
- Dificultat: no hi ha temps per totes les defenses. Pla B: defensa per mostreig en aula i lliurament d'un guió individual curt, amb sessió opcional per als casos dubtosos.

## Evidències globals del Repte 1

- fitxa breu d'exploració tècnica inicial
- explicació del model d'execució client vs servidor aplicat al producte
- decisió tècnica inicial
- repositori usable
- historial de commits significatiu
- entorn executable amb `Docker`, `PHP`, servidor web, BBDD i phpMyAdmin
- README executable
- primer punt d'entrada funcional del backend
- directori de documentació dins del repositori
- fitxes o documents del repte penjats al repositori
- índex o pàgina visible que enllaça la documentació
- justificació tècnica breu
- AI log quan hi haja ús rellevant d'IA
- defensa tècnica breu o checkpoint quan corresponga

## Criteri pràctic de tancament

`R1` queda preparat quan el professorat pot veure una decisió tècnica guiada, una base executable adaptada i completada, un primer punt d'entrada funcional del backend i una documentació dins del repositori suficient per revisar el procés i continuar cap a `R2` sense tornar a començar.
