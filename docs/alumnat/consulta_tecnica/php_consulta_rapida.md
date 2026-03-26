# PHP: consulta ràpida

## Què és

És una guia curta per recordar les peces de `PHP` que més et desbloquegen dins del curs. No és un manual del llenguatge: és una fitxa per situar entrada HTTP, funcions, sessions i persistència mínima.

## Quan la necessites en el curs

- en `R1`, per arrancar formulari, ruta o script funcional
- en `R2`, per gestionar `login`, sessions i operacions protegides
- en `R3`, per separar millor accés a dades, serveis i presentació

## Què has de saber sí o sí

- has de distingir dades d'entrada, lògica de negoci i persistència
- `$_GET`, `$_POST`, `$_SERVER` i `$_SESSION` no són el mateix
- convé encapsular funcions i responsabilitats, no omplir un únic fitxer
- `PDO` o equivalent és la base mínima per parlar bé amb la base de dades
- les funcions de sessions i password del nucli de `PHP` ja resolen moltes necessitats del curs

## Errors habituals

- posar-ho tot en un sol fitxer `index.php`
- usar superglobals sense validar ni normalitzar
- barrejar HTML, SQL i control d'accés al mateix bloc
- fer connexions a base de dades sense control d'errors
- inventar utilitats pròpies quan el nucli de `PHP` ja les porta

## On ampliar

- Material del curs: [Repte 1. Kickoff funcional](../../02_reptes/repte_01_kickoff_backend.md)
- Material del curs: [Repte 3. Migració a MVC i persistència segura](../../02_reptes/repte_03_mvc_i_persistencia.md)
- PHP Manual: [Language Reference](https://www.php.net/manual/en/langref.php)
- PHP Manual: [Superglobals](https://www.php.net/manual/en/language.variables.superglobals.php)
- PHP Manual: [PDO](https://www.php.net/manual/en/book.pdo.php)
- PHP Manual: [Sessions](https://www.php.net/manual/en/book.session.php)
