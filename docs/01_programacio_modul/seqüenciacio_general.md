# Seqüenciació general

## Criteris de seqüenciació

- progressió de menor a major complexitat tècnica
- cada repte hereta artefactes del repte anterior
- prioritat a funcionalitat executable abans d’optimització
- integració gradual de qualitat, seguretat, APIs i automatització
- connexió explícita entre RA, evidències i instrument d’avaluació

## Ordre dels 5 reptes

1. Kickoff tècnic d’un servei web backend
2. Mòdul de gestió d’usuaris i sessions
3. Migració a MVC i persistència segura
4. Publicació i consum d’API
5. Integració híbrida, automatització i manteniment

## Finalitat, RA principals i producte de cada repte

| Repte | Finalitat | RA principals | Producte del repte |
|---|---|---|---|
| 1 | Definir i deixar operativa la base tècnica del curs. | RA1, inici de RA5 | Repositori inicial, entorn funcional, README tècnic i ADR. |
| 2 | Construir funcionalitat de negoci amb sessions i autenticació. | RA2, RA3, RA4 | Mòdul d’usuaris/sessions validat amb proves bàsiques. |
| 3 | Reestructurar a MVC i consolidar persistència i qualitat. | RA5, RA6, RA8 | Backend modular amb accés segur a dades i testing de regressió. |
| 4 | Publicar serveis i consumir APIs amb contractes clars. | RA7, reforç RA6 | API documentada i client de consum integrat. |
| 5 | Integrar automatització i serveis externs per tancar el producte. | RA9, reforç RA7 i RA8 | Solució híbrida amb n8n/serveis externs i pla de manteniment. |

## Dependències entre reptes

- Repte 2 depén del repositori, convencions i entorn establits al Repte 1.
- Repte 3 reutilitza el codi funcional del Repte 2 per refactoritzar-lo a MVC.
- Repte 4 exposa i consumeix funcionalitats que provenen del model de dades del Repte 3.
- Repte 5 integra l’API i el backend madur dels Reptes 3 i 4 per automatitzar fluxos.

## Idea de producte evolutiu del curs

Tot el curs gira al voltant d’un **servei backend únic** que evoluciona de prototip tècnic a producte integrable:

- naix com a esquelet de projecte (Repte 1)
- guanya funcionalitat d’usuari (Repte 2)
- es fa mantenible i robust (Repte 3)
- s’obri a integracions via API (Repte 4)
- es connecta amb automatitzacions i serveis externs (Repte 5)

## Resultats esperats al final de cada repte

- Repte 1: equip amb entorn estable i criteri d’arquitectura justificat.
- Repte 2: funcionalitat backend d’accés d’usuaris operativa i defensable.
- Repte 3: arquitectura MVC amb persistència segura i qualitat observable.
- Repte 4: API usable i documentada, amb consum verificat.
- Repte 5: integració híbrida funcional, mantenible i presentada tècnicament.
