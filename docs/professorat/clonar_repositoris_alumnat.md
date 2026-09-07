# Clonar i actualitzar els repositoris de l’alumnat

Una mateixa ordre descarrega els repositoris que falten i actualitza els que ja tens. Executa-la **al teu ordinador**, des del repositori `dwes-microreptes-autocorreccio`.

## Preparació inicial

Necessites Git, Node.js 20 o posterior i accés amb el teu compte de GitHub als repositoris privats de l’alumnat. Si uses GitHub CLI, autentica Git una vegada:

```bash
gh auth login
gh auth setup-git
```

Si ja tens Git autenticat per HTTPS, no cal repetir-ho. Si treballes amb claus SSH autoritzades en GitHub, afegeix `--ssh` a les ordres de sincronització per als clons nous.

Si encara no tens l’autocorrector en este ordinador:

```bash
git clone https://github.com/igomis/dwes-microreptes-autocorreccio.git
cd dwes-microreptes-autocorreccio
```

Si ja el tens, entra en la seua carpeta i actualitza’l amb `git pull --ff-only`. L’script no necessita `npm install`.

## Primera descàrrega i actualitzacions

Pots veure primer quins repositoris processarà, sense descarregar res:

```bash
./scripts/sincronitza-repositoris.sh "$HOME/repositoris-alumnat" --dry-run
```

Per clonar-los o actualitzar-los:

```bash
./scripts/sincronitza-repositoris.sh "$HOME/repositoris-alumnat"
```

**Repeteix esta mateixa ordre abans de revisar treball nou.** Cada repositori queda en `~/repositoris-alumnat/organització/repositori`.

L’script usa `course/student-repositories.txt`, la llista general de l’autocorrector. Només descarrega els repositoris d’esta llista; no busca tots els de l’organització. La creació de repositoris des del tauler actualitza les llistes en la màquina que executa el tauler: si el servidor té una llista més recent que el teu ordinador, copia-la al teu ordinador i usa `--file`.

Per processar només un grup o una llista descarregada del servidor:

```bash
./scripts/sincronitza-repositoris.sh "$HOME/repositoris-alumnat" --group 2DAW-C
./scripts/sincronitza-repositoris.sh "$HOME/repositoris-alumnat" --file "$HOME/Downloads/student-repositories.txt"
```

`--group` i `--file` són alternatives. La llista admet comentaris amb `#`, una entrada `organització/repositori grup` per línia i URLs HTTPS o SSH de GitHub. Els duplicats es processen una sola vegada.

## Què passa amb el treball local

- Si falta el repositori, clona la branca `main`.
- Si ja existeix, comprova `origin`, la branca activa i l’estat local. Descarrega `main` i només l’avança si no hi ha commits locals; és una actualització *fast-forward*, sense crear merges.
- Si hi ha fitxers modificats o sense seguiment, una branca diferent, commits locals, una operació Git pendent o errors d’accés, avisa i continua amb els altres.
- No fa `push`, no elimina repositoris i no executa Docker ni instal·la dependències.

El resum indica quants repositoris s’han processat i quants s’han omés. Si n’hi ha algun amb incidències, l’ordre acaba amb codi 1. En eixe repositori, revisa `git status` i conserva el teu treball abans de tornar a executar-la; no cal esborrar ni forçar res.

`--dry-run` mostra les rutes previstes, però no comprova permisos remots ni garanteix que les actualitzacions siguen possibles. `--ssh` només tria el transport dels clons nous; no canvia l’`origin` de les còpies existents.

## Veure la web d’un alumne

Entra en la carpeta local de l’alumne i segueix el seu README per executar el projecte amb Docker. La sincronització obté el treball integrat en `main`; els canvis que l’alumne encara té només en la branca del microrepte no apareixen en esta vista.

Si dos projectes usen els mateixos ports, para el primer abans d’arrancar el següent. Esta revisió local no modifica les notes ni recupera microreptes: la recuperació continua sent del repte complet.
