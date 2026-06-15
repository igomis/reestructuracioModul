# Planificació de microtallers dins dels reptes

## Finalitat

Els microtallers són intervencions curtes de `45-75` minuts dins de sessions de repte. No creen microreptes nous ni notes separades: reforcen punts tècnics que solen bloquejar l'alumnat i ajuden a convertir el repte en una evidència més defensable.

## Criteris d'ús

- usar-los quan el grup arriba al punt del repte on la decisió tècnica és necessària;
- mantindre'ls com a suport pràctic, no com a classe teòrica llarga;
- tancar cada microtaller amb una evidència menuda al repositori;
- vincular-los a defensa individual, procés i verificació;
- no afegir-los tots obligatòriament si el grup necessita més temps de construcció.

## Microtallers fixos recomanats

| Codi | Moment | Microtaller | Duració | Evidència mínima |
|---|---|---|---:|---|
| `MT01` | `R1S1` | Projecte no CRUD | `60 min` | domini amb actors, regles i primer flux |
| `MT02` | `R1S2` | README executable i commit defensable | `45 min` | README amb arrencada i commit explicable |
| `MT03` | `R2S1-R2S2` | Validació de servidor amb casos roïns | `60 min` | taula de casos vàlids/invàlids i prova |
| `MT04` | `R2S4` | Sessió, cookies i estat | `45 min` | decisió sobre què es guarda i on |
| `MT05` | `R2S5-R2S6` | Auth mínima defensable | `60 min` | cas permés, cas denegat i explicació del control |
| `MT06` | `R2S7` | Debugging i prova curta | `45 min` | prova reproduïble abans de dir que funciona |
| `MT07` | `R3S1` | Migrar un cas d'ús a framework | `60 min` | mapa entre flux antic i flux en framework |
| `MT08` | `R3S2` | Migracions, seeders i dades de prova | `60 min` | projecte arrancable amb dades inicials |
| `MT09` | `R3S3-R3S4` | On pose la lògica | `60 min` | decisió controller/service/model documentada |
| `MT10` | `R4S1` | Dissenyar endpoint abans de programar | `60 min` | contracte d'endpoint abans del codi |
| `MT11` | `R4S5` | Provar i documentar una API | `60 min` | peticions reproduïbles i documentació alineada |
| `MT12` | `R5S1` | Triar una integració amb valor | `60 min` | mapa de valor i frontera entre sistemes |
| `MT13` | `R5S2` | Secrets, `.env` i claus | `45 min` | configuració segura sense secrets al repo |
| `MT14` | `R5S3` | Mapping de resposta externa | `60 min` | transformació de dades externa a model propi |
| `MT15` | `R5S5` | Defensa tècnica curta | `60 min` | guió de defensa i pregunta crítica preparada |

## Microtallers opcionals o d'ampliació

| Codi | Moment | Microtaller | Quan activar-lo |
|---|---|---|---|
| `MT16` | `R3S2B` | Portabilitat entre frameworks | si hi ha comparació real entre Laravel, Symfony i NestJS |
| `MT17` | `R4S6` | Tokens funcionals del backend | si el projecte necessita confirmació, invitació, accés puntual o traçabilitat |
| `MT18` | `R5S6` | Actius digitals tokenitzats | si el grup pot treballar ampliació avançada sense especulació |
| `MT19` | transversal | IA responsable aplicada al repte | abans d'un checkpoint o quan aparega delegació excessiva |

## Ordre recomanat

No cal fer-los tots. La seqüència mínima recomanada és:

1. `MT01`
2. `MT02`
3. `MT03`
4. `MT05`
5. `MT08`
6. `MT09`
7. `MT10`
8. `MT11`
9. `MT13`
10. `MT15`

## Presentacions associades

Les presentacions estan en `docs/07_presentacions/microtallers/` i seguixen el format de micro-presentació docent breu.

## Regla de tancament

Cada microtaller ha d'acabar amb una pregunta verificable:

> Què pots ensenyar ara en el repositori que no podies ensenyar abans del microtaller?
