# Guia docent R1S2: model d'entorn amb Docker Compose

## Per a què servix

Esta guia acompanya [R1S2. Entorn executable, landing inicial i tancament de R1](programacio_aula_r1s2_entorn_executable_punt_entrada.md). El professorat porta un **exemple executable propi** per mostrar les peces de l'entorn i la manera de verificar-les. Cada alumne o parella crea o adapta la configuració en el seu repositori i explica les decisions que ha pres. L'exemple docent no és una entrega que s'haja de copiar sense entendre-la.

La demostració comença amb una pàgina estàtica servida per Nginx. Després es traslladen els mateixos conceptes a la base PHP del repte amb el segon exemple d'esta guia. En R1S2 només cal PHP i servidor web: la base de dades i phpMyAdmin s'introduïxen quan es treballe la persistència en R2M9.

## Exemple inicial per a tractar a l'aula: una pàgina estàtica

Crea esta carpeta **fora dels repositoris de l'alumnat**:

```text
demo-compose/
├── docker-compose.yml
└── public/
    └── index.html
```

Contingut de `docker-compose.yml`:

```yaml
services:
  web:
    image: nginx:stable-alpine
    ports:
      - "127.0.0.1:8090:80"
    volumes:
      - ./public:/usr/share/nginx/html:ro
```

Contingut de `public/index.html`:

```html
<!doctype html>
<html lang="ca">
<head>
  <meta charset="utf-8">
  <title>Prova de Compose</title>
</head>
<body>
  <h1>La pàgina es veu des del contenidor</h1>
  <p>Canvia este text i recarrega el navegador.</p>
</body>
</html>
```

Des de `demo-compose/`, amb Docker en marxa:

```sh
docker compose config --quiet
docker compose up -d
docker compose ps
docker compose logs --tail=30
```

Obri `http://localhost:8090`, canvia el paràgraf de `public/index.html` i recarrega. En acabar, executa `docker compose down`. `config --quiet` valida la configuració, però només la comprovació al navegador demostra que la pàgina es servix. El port `8090` és del teu ordinador; el `80` és del contenidor. El muntatge `./public` fa visible el fitxer local dins de Nginx i `:ro` impedix que el contenidor el modifique.

Pregunta: «Si la pàgina no respon, què miraries primer: el port publicat, l'estat del servei o els logs? Quina prova faria falta per confirmar la hipòtesi?» Es pot provocar un error controlat ocupant el port `8090` amb un altre servei i després restaurar-lo. Este primer exemple només ensenya Compose, publicació de ports, muntatge i comprovació; no és l'entorn que ha d'entregar l'alumnat en R1M2.

## Model PHP per a R1M2

En una altra carpeta, prepara un segon exemple:

```text
demo-php/
├── docker-compose.yml
└── public/
    └── index.php
```

Contingut de `docker-compose.yml`:

```yaml
services:
  web:
    image: php:8.3-apache
    ports:
      - "127.0.0.1:8080:80"
    volumes:
      - ./public:/var/www/html:ro
```

Contingut de `public/index.php`:

```php
<?php
$producte = 'Material Viu';
?>
<!doctype html>
<html lang="ca">
<head>
  <meta charset="utf-8">
  <title><?= htmlspecialchars($producte, ENT_QUOTES, 'UTF-8') ?></title>
</head>
<body>
  <h1><?= htmlspecialchars($producte, ENT_QUOTES, 'UTF-8') ?></h1>
  <p>Un punt de trobada per compartir material del centre.</p>
  <p>Esta pàgina l'ha generada PHP al servidor.</p>
</body>
</html>
```

La variable `$producte` permet comprovar que PHP s'executa. Obri `http://localhost:8080`, canvia el valor i recarrega: el navegador ha de mostrar el nou títol. Si es veu el codi PHP com a text, la petició no passa per l'intèrpret de PHP. Este model només necessita el servei `web` i no crea cap base de dades.

## Abans de la classe

1. Prepara i prova `demo-compose/` amb els dos fitxers de l'exemple inicial.
2. En una **altra carpeta**, prepara `demo-php/` amb el model PHP anterior. Personalitza el nom del producte i el text de la landing. No mescles els dos fitxers Compose en la mateixa carpeta.
3. Comprova que Docker Engine o Docker Desktop està en marxa i que `docker compose version` respon.
4. Des de la carpeta del model PHP, executa:

   ```sh
   docker compose config --quiet
   docker compose up -d
   docker compose ps
   ```

5. Obri `http://localhost:8080` i comprova que la landing respon. Consulta `docker compose ps` per confirmar que el servei `web` està en execució.
6. Modifica un text de `public/index.php`, recarrega la landing i comprova que canvia. Després executa `docker compose down`.
7. Guarda una captura de la landing i una eixida breu de `docker compose ps` per si falla la connexió durant la demostració. Prepara també un error senzill i reversible per mostrar com es consulten `docker compose ps` i `docker compose logs --tail=30`.

El port `8080` és el del model PHP. Si està ocupat, canvia el port host i actualitza la URL que mostraràs.

## Guió de modelatge de 15 minuts

| Temps | Acció docent | Pregunta a l'alumnat |
|---|---|---|
| 0–3 min | Mostra `demo-compose/`: servei `web`, imatge, port i muntatge. Executa `config` i `up -d`. | Quin fitxer declara el servei? Què representen `8090` i `80`? |
| 3–5 min | Obri la pàgina, canvia el paràgraf i recarrega; consulta `ps` i `logs`. | Com arriba el canvi del fitxer local al navegador? |
| 5–8 min | Obri el model PHP i identifica les mateixes peces: servei web, port i muntatge de `public/`. | Què es manté i què canvia respecte de l'exemple Nginx? |
| 8–12 min | Arranca el model PHP, obri la landing i identifica el fitxer `public/index.php`. | Com saps que Apache servix la pàgina i PHP l'executa? |
| 12–15 min | Mostra un error de port preparat i consulta `ps` i `logs`; desfés-lo. | Quina és la hipòtesi i la pròxima comprovació? |

`web` servix PHP amb Apache. El model no inclou connexió PDO, formularis ni persistència funcional. MariaDB i phpMyAdmin no formen part d'esta demostració; s'afegiran quan facen falta en R2M9.

## Treball que fa l'alumnat

Després del modelatge, cada equip recupera el seu repositori, crea o adapta **personalment** el fitxer Compose i la landing segons la decisió tècnica de R1M1, arranca els serveis i documenta les ordres i URL reals en el README. El professorat pot mostrar l'exemple, fer preguntes i ajudar a interpretar errors; no cal repartir una configuració final idèntica a tots els projectes.

Per comprovar l'autoria i la comprensió, demana a cada equip que assenyale: (1) quin servei respon a la petició de la landing, (2) quin fitxer PHP s'executa, (3) quin port host publica el web i (4) com verificarà que l'entorn es pot reproduir. Si no arranca, accepta el bloqueig només si inclou log, hipòtesi i pròxima acció concreta, segons R1S2.

En la plantilla de treball de l'alumnat, l'agent d'IA té prohibit crear o modificar fitxers Docker Compose; pot explicar-los i ajudar a detectar problemes. Per això l'alumne ha de fer el canvi al fitxer ell mateix.

## Referències tècniques

- [Docker Compose: introducció i cicle de vida](https://docs.docker.com/compose/)
- [Docker Compose: guia inicial](https://docs.docker.com/compose/gettingstarted/)
