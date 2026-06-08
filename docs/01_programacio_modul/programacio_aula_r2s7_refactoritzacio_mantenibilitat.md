# R2S7. Refactoritzacio i millora de mantenibilitat

## Finalitat de la sessio

Esta sessio tanca `R2` millorant codi que ja funciona. La refactoritzacio no és una reescriptura ni un canvi de framework: és una millora acotada de responsabilitats, noms, duplicacio, imports i representacio mínima d'una entitat del domini.

L'objectiu és arribar a `R3` amb una base funcional provada i una primera decisio de mantenibilitat defensable.

## Encaix dins del Repte 2

- **Repte**: `R2. Processament bàsic, estat, autenticació i primera funcionalitat protegida`
- **Microrepte**: `R2M7`
- **Sessio**: `R2S7`
- **Duracio orientativa**: `3 hores`
- **Focus**: refactoritzacio acotada, fitxer comú, funcions reutilitzables, objecte simple del domini i no regressio
- **No entra encara**: MVC complet, ORM, reescriptura en framework o POO extensa obligatoria

## Relacio amb RA i criteris de treball

| Element | Concrecio en el microrepte |
|---|---|
| `RA3.d` | funcions i organitzacio del codi amb responsabilitat més clara |
| `RA3.g` | comentaris o justificacions útils quan aporten claredat |
| `RA4.f` | prova de no regressio després de canvis |
| Evidencia central | comparativa abans/després i flux complet encara funcional |
| Verificacio docent | revisio de diff, execucio de proves i defensa de la millora |

## Producte esperat

Una millora acotada que incloga:

- zona de codi triada a partir de `R2M6`;
- problema de mantenibilitat identificat;
- extraccio de funcio, fitxer comú o configuracio compartida;
- ús de `include`, `require`, `include_once` o `require_once` amb sentit;
- objecte simple del domini si aporta claredat;
- comparativa abans/després;
- prova de no regressio del flux;
- nota de què queda per reorganitzar en `R3`.

## Preparacio previa del professorat

Convé preparar:

- exemple de refactoritzacio xicoteta;
- exemple de fitxer comú importat;
- exemple d'objecte simple sense arquitectura completa;
- criteri per aturar reescriptures grans;
- bateria mínima de no regressio de `R2M6`.

## Seqüencia d'aula de 3 hores

### 0:00-0:25. Seleccio de zona

Tasques:

- revisar bateria de `R2M6`;
- triar una zona que funciona;
- identificar duplicacio, noms confusos o barreja excessiva;
- definir millora concreta.

Resultat: refactoritzacio acotada i verificable.

### 0:25-0:55. Modelatge docent

Mostrar:

- abans/després curt;
- extraccio de funcio;
- import amb `require_once`;
- objecte simple si ajuda;
- prova posterior.

Resultat: queda clar que més fitxers no és automàticament millor.

### 0:55-1:45. Refactoritzacio

Tasques:

- extraure funcions o configuracio;
- separar preparacio de dades i renderitzat quan siga viable;
- millorar noms;
- reduir duplicacio;
- introduir entitat simple si té sentit.

Resultat: el codi queda més clar en una zona concreta.

### 1:45-2:15. Prova de no regressio

Tasques:

- repetir casos clau de `R2M6`;
- comprovar operacio protegida;
- revisar estat i invalidacio;
- corregir regressions.

Resultat: la refactoritzacio no trenca el flux.

### 2:15-2:40. Comparativa i justificacio

Tasques:

- escriure abans/després;
- explicar responsabilitat millorada;
- indicar què queda per a `R3`;
- registrar ús d'IA si ha influït.

Resultat: la decisio és defensable.

### 2:40-3:00. Checkpoint final

Cada equip mostra:

- diff o comparativa;
- fitxer comú o funcio extreta;
- objecte simple si aplica;
- prova de no regressio;
- justificacio de mantenibilitat.

Pregunta: quina responsabilitat queda ara més clara i com has comprovat que el flux continua funcionant?

## Tasques concretes de l'alumnat

- Triar zona provada.
- Identificar problema de mantenibilitat.
- Fer refactoritzacio xicoteta.
- Importar fitxer comú o reutilitzar funcions.
- Afegir objecte simple si ajuda.
- Repetir proves.
- Documentar abans/després.

## Evidencies minimes

| Evidencia | Minim acceptable |
|---|---|
| Zona triada | part del flux que ja funcionava |
| Canvi | funcio, fitxer comú, import o objecte simple |
| Millora | responsabilitat, nom o duplicacio més clara |
| Prova | no regressio del flux |
| Comparativa | abans/després documentat |
| Pas a R3 | pendents arquitectonics identificats |

## Criteris d'exit

- El canvi no és només moure codi.
- La responsabilitat millora.
- El flux continua funcionant.
- La millora és acotada.
- L'alumnat pot defensar el canvi.

## Que no és suficient

- Crear fitxers sense criteri.
- Reescriure-ho tot.
- Introduir POO que no s'entén.
- Trencar la demo.
- No repetir proves.
- Presentar arquitectura completa com a mínim obligatori.

## Us de la IA

La IA pot suggerir noms, detectar duplicacio o proposar extraccions. Control: cap proposta es dona per bona sense prova de no regressio i justificacio pròpia.

## Suport per alumnat amb més dificultat

Extraure una funcio de validacio o missatge a un fitxer comú i repetir dos casos de prova. Escriure només una comparativa curta.

## Ampliacio per alumnat avançat

- Entitat simple del domini amb propietats i mètode clar.
- Separacio més neta de plantilles i logica.
- Proves automatitzades de no regressio.
- ADR breu de pas a `R3`.

## Checklist de tancament

- [ ] He triat codi que ja funcionava.
- [ ] He identificat un problema de mantenibilitat.
- [ ] He fet una millora acotada.
- [ ] He usat funcio, fitxer comú o import amb criteri.
- [ ] He incorporat objecte simple si aporta claredat.
- [ ] He repetit proves clau.
- [ ] He escrit abans/després.
- [ ] He indicat què queda per a `R3`.

## Connexio amb R3

`R3` aprofitarà este tancament per reconstruir el projecte amb arquitectura i persistencia més sòlides. La pregunta de pas és:

Quina part del flux necessita ara una estructura més professional perquè siga mantenible a llarg termini?

