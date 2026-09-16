# Guia docent R1S2: model d'entorn amb Docker Compose

## Per a què servix

Esta guia acompanya [R1S2. Entorn executable, landing inicial i tancament de R1](programacio_aula_r1s2_entorn_executable_punt_entrada.md). El professorat porta un **exemple executable propi** per mostrar les peces de l'entorn i la manera de verificar-les. Cada alumne o parella crea o adapta la configuració en el seu repositori i explica les decisions que ha pres. L'exemple docent no és una entrega que s'haja de copiar sense entendre-la.

La fitxa de consolidació `dwes-microreptes-autocorreccio/consolidation-drafts/r1m2.md` conté un exemple complet de `docker-compose.yml` i `public/index.php`. Cal obrir-la en eixe repositori.

## Abans de la classe

1. Crea **fora dels repositoris de l'alumnat** una carpeta de demostració amb `docker-compose.yml` i `public/index.php`. Pots partir dels dos fitxers de la fitxa de consolidació i personalitzar el nom del producte i el text de la landing.
2. Comprova que Docker Engine o Docker Desktop està en marxa i que `docker compose version` respon.
3. Des de la carpeta de demostració, executa:

   ```sh
   docker compose config --quiet
   docker compose up -d
   docker compose ps
   ```

4. Obri `http://localhost:8080` i `http://localhost:8081`. Entra a phpMyAdmin amb l'usuari i la clau **demo** de l'exemple i comprova que es veu la base de dades. La landing encara no consulta eixa base de dades.
5. Modifica un text de `public/index.php`, recarrega la landing i comprova que canvia. Després executa `docker compose down`. No uses `down -v` si vols conservar les dades del volum.
6. Guarda una captura de la landing i una eixida breu de `docker compose ps` per si falla la connexió durant la demostració. Prepara també un error senzill i reversible, per exemple posar temporalment un port host ocupat, per mostrar com es consulten `docker compose ps` i `docker compose logs --tail=30`.

Els ports `8080` i `8081` són els de l'exemple. Si estan ocupats, canvia el port host en el model i actualitza les URL que mostraràs. Les claus del model són només per a una pràctica local.

## Guió de modelatge de 15 minuts

| Temps | Acció docent | Pregunta a l'alumnat |
|---|---|---|
| 0–3 min | Mostra la carpeta i localitza `docker-compose.yml` i `public/index.php`. | Quin fitxer declara els serveis i quin genera la pàgina? |
| 3–6 min | Recorre `web`, `db` i `phpmyadmin`; assenyala ports, muntatge de `public/` i volum de dades. | Quin port s'obri al navegador? Per què phpMyAdmin usa `db`? |
| 6–9 min | Executa `config`, `up -d` i `ps`; obri la landing i phpMyAdmin. | Què demostra `config`? Què falta comprovar després? |
| 9–12 min | Canvia un text de la landing i recarrega. | Com arriba el canvi del fitxer local al navegador? |
| 12–15 min | Provoca o mostra un error de port i consulta `ps` i `logs`; desfés-lo. | Quina és la hipòtesi i la pròxima comprovació? |

`web` servix PHP amb Apache; `db` guarda les dades en un volum; `phpmyadmin` es connecta a `db` per la xarxa interna de Compose. El port de MariaDB no necessita publicar-se al host per a esta demostració. El model no inclou encara connexió PDO des del producte, formularis ni persistència funcional: això pertany als reptes posteriors.

## Treball que fa l'alumnat

Després del modelatge, cada equip recupera el seu repositori, crea o adapta **personalment** el fitxer Compose i la landing segons la decisió tècnica de R1M1, arranca els serveis i documenta les ordres i URL reals en el README. El professorat pot mostrar l'exemple, fer preguntes i ajudar a interpretar errors; no cal repartir una configuració final idèntica a tots els projectes.

Per comprovar l'autoria i la comprensió, demana a cada equip que assenyale: (1) quin servei respon a la petició de la landing, (2) quin fitxer PHP s'executa, (3) quin port host publica el web i (4) com verificarà que l'entorn es pot reproduir. Si no arranca, accepta el bloqueig només si inclou log, hipòtesi i pròxima acció concreta, segons R1S2.

En la plantilla de treball de l'alumnat, l'agent d'IA té prohibit crear o modificar fitxers Docker Compose; pot explicar-los i ajudar a detectar problemes. Per això l'alumne ha de fer el canvi al fitxer ell mateix.

## Referències tècniques

- [Docker Compose: introducció i cicle de vida](https://docs.docker.com/compose/)
- [Docker Compose: guia inicial](https://docs.docker.com/compose/gettingstarted/)
