# Pla de derivació del repositori d’alumnat

## 1. Finalitat del document

Este document definix com derivar un nou repositori orientat a alumnat a partir del repositori actual de reestructuració del mòdul.

La derivació no s’ha d’entendre com una còpia mecànica de carpetes, sinó com una operació de selecció, simplificació i reescriptura.

L’objectiu és que el nou repositori servisca a l’alumnat per a:

- entendre el curs
- seguir els reptes
- consultar materials útils
- saber què s’espera de cada lliurament
- preparar checkpoints i defenses
- navegar el projecte sense soroll documental intern

---

## 2. Diagnòstic de partida

El repositori actual ja té una estructura rica i funcional, amb accessos per perfil i per tipus d’ús.

La seua estructura principal inclou:

- `docs/alumnat/`
- `docs/professorat/`
- `docs/01_programacio_modul/`
- `docs/02_reptes/`
- `docs/03_avaluacio/`
- `docs/04_materials/`
- `docs/05_projectes_tecnics/`
- `docs/06_plantilles/`
- `docs/07_presentacions/`
- `docs/08_materials_compartibles/`
- `docs/09_paquets_ús_directe/`

A més, el repositori ja declara que la web per a alumnat i professorat, els materials compartibles i els paquets d’ús directe ja queden publicats com a accessos curts per a ús real, i que la web ja és usable com a entorn final de consulta per perfil.

Això implica que el nou repositori d’alumnat no ha de nàixer des de zero, sinó com una reorganització específica d’una part del que ja està construït.

---

## 3. Objectiu del nou repositori d’alumnat

El nou repositori ha de ser un entorn clar, lleuger i orientat a execució.

No ha de presentar-se com a repositori de redisseny curricular ni com a espai de presa de decisions docents, sinó com a espai de treball per a alumnat.

### Objectius específics

- donar una visió clara del recorregut del curs
- oferir una versió neta dels reptes
- fer visibles evidències, lliurables i checkpoints
- donar accés als materials realment útils
- reduir càrrega de documentació interna o meta
- facilitar navegació ràpida i ús real en aula

---

## 4. Principis de derivació

### 4.1 Selecció, no còpia total

No s’ha de copiar el repositori complet.

S’han de seleccionar només aquelles peces que aporten valor directe a l’alumnat.

### 4.2 Reescriptura orientada a acció

Els textos no han de quedar en clau de disseny curricular intern, sinó en clau de:

- què has de fer
- què has d’entregar
- com es comprovarà
- què has de preparar per a la defensa

### 4.3 Simplicitat de navegació

La navegació del repo d’alumnat ha de ser més curta i més plana que la del repositori docent.

### 4.4 Coherència amb el repositori docent

El repo d’alumnat ha d’estar alineat amb la seqüència i amb la documentació docent, però no ha de reproduir-ne totes les capes.

### 4.5 Revisió documental completa

Cada document exportat s’ha de revisar abans de publicar-se en el nou repo.

No s’ha d’assumir que un document útil en el repo docent és automàticament útil per a alumnat.

---

## 5. Què ha d’entrar al repositori d’alumnat

### 5.1 Blocs que convé aprofitar com a base

### `docs/alumnat/`

És el punt de partida més natural per al nou repositori, perquè ja està pensat com a accés sintètic per a alumnat.

### `docs/02_reptes/`

S’han d’aprofitar les fitxes dels reptes, però en versió revisada i netejada per a alumnat.

### `docs/03_avaluacio/`

Només les peces que siguen directament útils per a alumnat, com:

- rúbriques visibles
- checklists de lliurament
- guies d’evidències
- pautes de checkpoints i defenses

### `docs/04_materials/`

Només els materials realment útils per seguir els reptes.

### `docs/08_materials_compartibles/`

És una font especialment útil per al repositori d’alumnat perquè ja conté peces curtes donables i d’ús real.

### `docs/09_paquets_ús_directe/`

També és molt aprofitable perquè agrupa materials per moment del curs i això encaixa molt bé amb l’ús per part de l’alumnat.

### `docs/05_projectes_tecnics/`

Ha d’entrar només en la part que dona context de projecte base i ajuda a entendre el producte del curs.

---

## 6. Què no ha d’entrar al repositori d’alumnat tal com està

### 6.1 Blocs d’ús principalment docent o intern

### `docs/01_programacio_modul/`

No és un bloc pensat principalment per a alumnat.

### `docs/06_plantilles/`

És útil per a professorat i per a construcció documental, però no com a capa principal del repo d’alumnat.

### `docs/professorat/`

No ha d’entrar al repositori d’alumnat, excepte si en algun moment es deriva una peça concreta i reescrita explícitament per a ús d’alumnat.

### Matrius de coherència vertical

No són materials prioritaris per a alumnat.

### Documents de govern del redisseny

No aporten valor directe a l’execució del curs per part de l’alumnat.

### Documentació de calibratge docent

Tampoc hauria d’entrar com a part del recorregut normal d’alumnat.

---

## 7. Estructura recomanada del nou repositori

Es recomana una estructura pròpia, més simple que l’actual.

```text
docs/
  00_inici/
  01_com_funciona_el_curs/
  02_reptes/
  03_com_s_avalua/
  04_materials/
  05_projecte_base/
  06_checkpoints_i_defenses/
  07_recursos_rapid/
```

Esta estructura hauria de permetre que l’alumnat puga entrar al repositori i entendre ràpidament:

- on començar
- què ha de fer cada setmana o fase
- què ha d’entregar
- com es revisarà
- on trobar ajuda útil

---

## 8. Matriu operativa de derivació

| Origen en el repo docent | Destí recomanat en el repo d’alumnat | Operació necessària | Prioritat |
|---|---|---|---|
| `docs/alumnat/index.md` | `docs/00_inici/index.md` | reescriure com a portada principal del nou repo | Alta |
| `docs/alumnat/com_funciona_el_curs.md` | `docs/01_com_funciona_el_curs/com_funciona_el_curs.md` | adaptar en clau d’ús i recorregut real | Alta |
| `docs/alumnat/com_es_valora.md` | `docs/03_com_s_avalua/com_es_valora.md` | mantindre i revisar en clau de lliurables i evidències | Alta |
| `docs/alumnat/com_fer_servir_la_ia.md` | `docs/01_com_funciona_el_curs/com_fer_servir_la_ia.md` | mantindre com a guia curta d’ús verificable | Alta |
| `docs/alumnat/reptes/*.md` | `docs/02_reptes/` | usar com a base curta i sincronitzar amb les fitxes docents | Alta |
| `docs/02_reptes/*.md` | `docs/02_reptes/` | reescriure i simplificar en versió alumnat, sense meta curricular sobrant | Alta |
| `docs/03_avaluacio/rubrica_base_reptes.md` | `docs/03_com_s_avalua/rubrica_reptes.md` | resumir i traduir a lectura comprensible per a alumnat | Alta |
| `docs/03_avaluacio/rubrica_defensa_tecnica.md` | `docs/06_checkpoints_i_defenses/rubrica_defensa.md` | mantindre visible com a peça de preparació de defensa | Alta |
| `docs/03_avaluacio/checklist_revisio_repo.md` | `docs/03_com_s_avalua/checklist_revisio_repo.md` | adaptar com a checklist de lliurament | Alta |
| `docs/03_avaluacio/sistema_evidencies.md` | `docs/03_com_s_avalua/evidencies_i_lliurables.md` | sintetitzar per a alumnat | Alta |
| `docs/03_avaluacio/plantilla_ai_log.md` | `docs/03_com_s_avalua/ai_log_minim.md` | mantindre si s’explica com usar-la | Mitjana |
| `docs/04_materials/materials_comuns/` | `docs/04_materials/` | seleccionar només materials reutilitzables i freqüents | Alta |
| `docs/04_materials/repte_02/` a `repte_05/` | `docs/04_materials/` | reagrupar per repte o necessitat | Alta |
| `docs/alumnat/consulta_tecnica/*.md` | `docs/07_recursos_rapid/` | mantindre com a consulta tècnica curta | Alta |
| `docs/05_projectes_tecnics/enunciat_projecte_base.md` | `docs/05_projecte_base/enunciat.md` | exportar quasi directe amb revisió de to | Alta |
| `docs/05_projectes_tecnics/projectes_base_concretats.md` | `docs/05_projecte_base/projectes_base.md` | resumir i deixar com a catàleg usable | Mitjana |
| `docs/08_materials_compartibles/*.md` | `docs/06_checkpoints_i_defenses/` i `docs/04_materials/` | repartir segons ús real | Alta |
| `docs/09_paquets_ús_directe/*.md` | `docs/00_inici/` i `docs/06_checkpoints_i_defenses/` | convertir en paquets d’entrada, pas i tancament | Alta |

---

## 9. Criteris editorials de reescriptura

Cada document que passe al repositori d’alumnat hauria de complir estes regles:

- començar amb una finalitat clara i operativa
- dir què ha de fer l’alumnat amb eixe document
- evitar llenguatge de planificació interna o calibratge docent
- reduir referències a matrius, distribucions SA → RA o debats de disseny
- fer visibles lliurables, checkpoints, evidències i riscos habituals
- mantindre el mateix nivell d’exigència, però amb menys soroll conceptual
- conservar enllaços només a peces útils per a alumnat
- evitar duplicacions entre portada, reptes i materials

En la reescriptura convé passar de frases com:

- “este document justifica curricularment...”
- “per mantindre coherència amb la programació vigent...”

a frases com:

- “en este repte has de deixar...”
- “per superar este punt has de poder demostrar...”
- “abans del checkpoint convé tindre preparat...”

---

## 10. Procés d’execució recomanat

### Fase 1. Inventari i classificació

Cal revisar els documents candidats i classificar-los en quatre grups:

- exportació quasi directa
- exportació amb reescriptura
- fusió amb altres peces
- exclusió del repo d’alumnat

### Fase 2. Definició d’arquitectura d’informació

Cal crear l’estructura final del repo d’alumnat i decidir:

- quina serà la portada
- quin serà l’itinerari de lectura inicial
- com es veuran els reptes
- on aniran rúbriques, checklists i defenses
- com s’organitzaran els recursos tècnics curts

### Fase 3. Reescriptura per blocs

L’ordre recomanat de producció és:

1. `00_inici/`
2. `01_com_funciona_el_curs/`
3. `02_reptes/`
4. `03_com_s_avalua/`
5. `05_projecte_base/`
6. `06_checkpoints_i_defenses/`
7. `04_materials/` i `07_recursos_rapid/`

### Fase 4. Enllaçat i neteja

Cal revisar:

- enllaços interns
- coherència de noms
- duplicitats
- documents massa llargs
- punts on encara aparega veu docent interna

### Fase 5. Validació d’ús real

Abans de donar el nou repo per bo, convé fer una prova simple de navegació:

- una alumna o alumne nou sap per on començar
- troba el repte actual en pocs clics
- entén què ha d’entregar
- localitza com es valora
- troba materials de suport sense entrar en documents interns

---

## 11. Prioritats de construcció

Si la derivació s’ha de fer per fases i no tota de colp, l’ordre recomanat és este:

### Prioritat 1. Nucli imprescindible

- portada del repo
- com funciona el curs
- com es valora
- repte 1 a repte 5 en versió alumnat
- projecte base

### Prioritat 2. Acompanyament d’execució

- checkpoints i defenses
- guies d’evidències
- ús de la IA
- checklists de lliurament

### Prioritat 3. Suport i refinament

- recursos tècnics curts
- paquets per moment del curs
- materials de reforç o consulta avançada

---

## 12. Riscos de derivació que convé vigilar

Els riscos principals són:

- copiar massa documentació i reproduir el soroll del repo docent
- simplificar tant que es perda exigència o precisió
- deixar documents duplicats amb versions divergents
- exportar peces de professorat sense reescriptura
- convertir el repo d’alumnat en un simple mirall dels fitxers actuals
- trencar enllaços o itineraris de lectura

La decisió clau és esta:

El repositori d’alumnat ha de ser més curt, però no més ambigu.

---

## 13. Criteris de validació abans de publicar

El nou repositori d’alumnat hauria de considerar-se preparat quan:

- té una portada clara i usable
- un alumne sap què llegir primer
- cada repte mostra objectiu, lliurables, evidències i preparació de defensa
- la manera d’avaluar-se és visible sense llegir documentació docent interna
- els materials útils estan accessibles en pocs clics
- no hi ha matrius docents ni documents de calibratge en el recorregut normal
- els enllaços funcionen
- la relació amb el producte base és clara

---

## 14. Definition of done del pla de derivació

El pla es considerarà complet quan permeta executar una derivació real del repositori amb estes garanties:

- el nou repo naix com a selecció i reescriptura, no com a còpia total
- la font principal d’exportació és identificable per blocs i per documents
- queda definida una estructura final clara
- s’explicita què entra, què no entra i què necessita reescriptura
- queda definit un ordre de treball executable
- hi ha criteris de validació previs a la publicació
- el futur repo d’alumnat es pot entendre com un producte documental propi, alineat amb el repositori docent però no subordinat a totes les seues capes internes

---
