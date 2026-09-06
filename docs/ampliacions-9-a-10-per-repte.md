# Ampliacions 9 a 10 per repte

## Classificació documental

Este és un **document derivat**. Depén de [curs executable](curs-executable.md), [avaluació i evidències](03_avaluacio/index.md), [ús de la IA](us-ia-professorat-i-alumnat.md) i de les fitxes canòniques dels `R1-R5`.

## Finalitat general

Explicar la capa d'ampliacions `9→10` del curs sense convertir-la en una segona programació paral·lela.

## Criteri metodològic adoptat

El model és híbrid:

- cada repte mostra des del principi una via d'excel·lència
- l'ampliació es pot fer en temps sobrant de classe, entre sessions o al tancament del repte
- en algun repte es pot activar una microampliació parcial, però no com a rutina diària obligatòria

## Regla comuna: nucli primer, ampliació després

L'ampliació només computa si:

- el nucli obligatori del repte està complet i validat
- l'ampliació aporta valor tècnic real
- es pot defensar
- queda acreditada amb evidències

No servix per compensar mancances del repte base.

## Fórmula comuna de qualificació

La qualificació final de cada repte ha de separar el nucli obligatori de la via d'excel·lència:

```text
nota_final_repte = 0.9 * nota_nucli_repte + ampliacio_9_10
```

La nota del nucli pot estar excel·lentment resolta, però sense ampliació validada la nota final del repte queda limitada a `9`. La franja `9→10` requerix una ampliació integrada, verificada, traçable i defensable.

L'ampliació pot sumar entre `0` i `1` punt. No s'ha d'aplicar si el nucli obligatori no està complet i validat.

## Sentit de la franja 9→10

La franja `9→10` no són punts extra arbitraris. És la via per demostrar excel·lència tècnica:

- robustesa
- qualitat del codi
- seguretat
- proves
- documentació tècnica
- traçabilitat
- integració
- automatització útil
- mantenibilitat
- qualitat arquitectònica

## Paper de la IA

La IA es pot usar per:

- contrastar enfocaments
- proposar alternatives
- revisar codi
- suggerir proves
- ajudar a documentar
- comparar implementacions

Però no pot substituir:

- la decisió tècnica de l’alumne
- la validació
- la prova
- ni la defensa

## Criteri docent comú

Per verificar una ampliació, el professorat ha de poder reutilitzar instruments ja presents al model:

- checklist curta d’ampliació
- revisió de repositori
- demo funcional
- prova guiada
- mini defensa tècnica

## Remissió a les ampliacions de cada repte

- [Repte 1](02_reptes/repte_01_kickoff_backend.md#13-ampliacio-910)
- [Repte 2](02_reptes/repte_02_sessions_i_autenticacio.md#13-ampliacio-910)
- [Repte 3](02_reptes/repte_03_mvc_i_persistencia.md#13-ampliacio-910)
- [Repte 4](02_reptes/repte_04_api_i_consum.md#13-ampliacio-910)
- [Repte 5](02_reptes/repte_05_integracio_hibrida.md#13-ampliacio-910)

Per a futures variants o adaptacions, es pot reutilitzar la [plantilla docent d'ampliació 9→10](04_materials/plantilla_ampliacio_9_10.md).

## Càlcul i validació de l'ampliació global

Les notes dels microreptes continuen sobre 10 i valoren només el nucli. La nota global del repte es calcula una sola vegada:

```text
nucli = suma(nota_microrepte × pes) / suma(pesos)
nota_repte = 0,9 × nucli + ampliacio_validada
```

El nucli aporta fins a 9 punts i l'ampliació fins a 1. S'arredonix només el resultat final a dos decimals. Les notes curriculars per RA es mantenen separades: no es torna a sumar l'ampliació a cada RA ni a cada microrepte.

| Repte | Únic microrepte que recull l'ampliació | Declaració |
|---|---|---|
| R1 | R1M2 | `docs/r1-ampliacio.md` |
| R2 | R2M9 | `docs/r2-ampliacio.md` |
| R3 | R3M7 | `docs/r3-ampliacio.md` |
| R4 | R4M5 | `docs/r4-ampliacio.md` |
| R5 | R5M5 | `docs/r5-ampliacio.md` |

La declaració identifica l'últim microrepte, explica el valor aportat al repte complet i enllaça implementació, proves, decisions i ús d'IA. L'ampliació pot desenvolupar-se abans, però només es proposa i valida en este punt final. Les activitats d'aprofundiment anteriors no generen punts independents. El taller opcional R2S10 pot aportar evidències a la declaració de R2, sense crear un nou microrepte amb nota.

| Qualitat de l'ampliació | Punts proposats/validats |
|---|---:|
| Absent o no funcional | 0 |
| Parcial, amb mancances importants | 0,25 |
| Funcional, amb verificació o justificació incompleta | 0,50 |
| Completa i verificada, amb una mancança menor | 0,75 |
| Completa, verificada i ben justificada | 1 |

L'autocorrector proposa els punts i assenyala evidències i preguntes per a la presentació. El professorat confirma o ajusta la proposta, comprova els mínims obligatoris del repte i guarda una observació. Sense mínims coberts no es poden sumar punts d'ampliació. Si no hi ha ampliació, el professorat pot validar explícitament 0; l'absència d'una proposta automàtica no impedix la revisió manual.

Pendent de revisió no significa zero: la base és visible, però la nota global queda pendent. Si falten correccions obligatòries, no es pot validar. Una nova correcció que canvie la instantània revisada torna a deixar la validació pendent. Validar l'ampliació tampoc elimina altres avisos de revisió docent del nucli.

Exemples: nucli 10 sense ampliació validada (0) → 9; nucli 10 amb ampliació 1 → 10; nucli 8 amb ampliació 0,5 i mínims confirmats → 7,70. Fer una ampliació no garantix arribar a 9.

Este criteri substituïx la fórmula anterior `min(nucli, 9) + ampliació`: és un canvi d'escala explícit. Les correccions originals dels microreptes es conserven, i una nova agregació aplica la fórmula actual sense inventar validacions docents.
