# Autenticació i autorització

## Què és
Autenticació és demostrar qui eres. Autorització és decidir què pots fer. En el curs les dos coses només tenen valor si protegixen una operació real del producte.

## Quan la necessites en el curs
- en `R2`, com a nucli del primer flux de negoci protegit
- en `R3`, quan roles, restriccions i persistència han de quedar coherents
- en `R4`, quan exposes endpoints que no pot usar qualsevol actor

## Què has de saber sí o sí
- no n'hi ha prou amb fer `login`; has de protegir una acció amb sentit de negoci
- necessites com a mínim un actor clar i una operació que puga ser denegada
- els permisos han d'estar lligats al domini: aprovar moviments, confirmar reserves, assignar incidències
- l'autorització s'ha de comprovar al servidor
- has de poder ensenyar un cas correcte i un cas denegat

Exemples útils:
- inventari: només qui té rol adequat pot aprovar una operació o generar un token
- reserves: no qualsevol persona pot forçar una reserva o canviar estat fora del flux previst
- incidències: no qualsevol actor pot prioritzar, assignar o tancar

## Errors habituals
- confondre autenticació amb autorització
- fer un rol `admin` sense cap justificació funcional
- protegir pantalles, però no la lògica real del backend
- no provar accessos denegats
- generar esquelets d'auth amb IA o scaffolding i no saber què comproven de veritat

## On consultar-ho bé
- [Repte 2. Sessions, autenticació i primera funcionalitat](../../02_reptes/repte_02_sessions_i_autenticacio.md)
- [Apunts reals del Repte 2](../../04_materials/apunts_reals/repte_02_sessions_i_autenticacio.md)
- [Materials de sessió de `R2`](../../04_materials/materials_aula/repte_02_materials_sessio.md)
- [Projectes base concretats](../../05_projectes_tecnics/projectes_base_concretats.md)
