# Seguretat bàsica de backend

## Què és
És el conjunt mínim de decisions que impedixen que el teu backend accepte qualsevol entrada, expose dades sensibles o deixe operacions crítiques sense control. En el curs no és una capa extra: és part del producte que has de poder defensar.

## Quan la necessites en el curs
- en `R1`, des del moment que rebs dades externes
- en `R2`, quan apareixen credencials, sessions i rutes protegides
- en `R3-R5`, quan persistixes dades, publiques `API` i integres serveis externs

## Què has de saber sí o sí
- valida sempre l'entrada al servidor
- no concatentes SQL ni exposes secrets en codi o `README`
- un error no ha de revelar contrasenyes, claus, traces o estructura interna innecessària
- els permisos s'han de comprovar al backend, no al client
- si un endpoint o `webhook` és sensible, has d'explicar com el protegixes

## Errors habituals
- pujar `.env`, claus o credencials al repositori
- confiar en dades del client sense tornar-les a validar
- fer consultes SQL a mà amb concatenació de cadenes
- deixar endpoints interns oberts perquè en local funcionen
- mostrar errors massa detallats en entorn de producció

## On ampliar
- Material del curs: [Repte 2. Sessions, autenticació i primera funcionalitat](../../02_reptes/repte_02_sessions_i_autenticacio.md)
- Material del curs: [Guia de persistència i modelat de dades](../../04_materials/repte_03/guia_persistencia_i_modelat_dades.md)
- OWASP: [Top 10](https://owasp.org/www-project-top-ten/)
- OWASP Cheat Sheet: [SQL Injection Prevention](https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet.html)
- PHP Manual: [SQL Injection](https://www.php.net/manual/en/security.database.sql-injection.php)
- FastAPI Docs: [Security](https://fastapi.tiangolo.com/tutorial/security/)
