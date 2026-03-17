# Guia de persistència i modelat de dades

## Finalitat
Consolidar al Repte 3 un model de dades prou estable perquè el producte deixe de dependre d'estat efímer o estructures improvisades i puga operar amb persistència coherent, segura i revisable.

Esta guia servix per decidir què s'ha de modelar, com es manté consistència bàsica i com s'han de relacionar validacions, errors i operacions de dades dins del domini triat.

## Model de dades mínim del domini
El domini triat ha de quedar representat, com a mínim, amb:
- una entitat d'usuari o equivalent vinculada a autenticació
- una entitat principal del domini: incidència, reserva, cita, recurs o inventari
- atributs mínims necessaris per operar el cas d'ús principal
- identificadors clars i camps obligatoris del model
- relacions bàsiques entre usuari i domini quan el flux ho requerisca

Criteri mínim de modelat:
- cada camp ha de respondre a una necessitat del domini o del flux del repte
- no s'han d'afegir dades ornamentals sense impacte funcional
- la persistència ha de permetre recuperar, actualitzar o protegir els casos d'ús prioritaris

## Persistència segura i consistència bàsica
La persistència del Repte 3 ha de garantir:
- operacions de lectura i escriptura coherents amb el domini
- tractament controlat de dades inexistents, invàlides o fora d'estat
- absència d'acoblaments innecessaris entre codi de persistència i codi de resposta
- consistència mínima quan un canvi afecta més d'una regla del model
- revisió de consultes, transicions o accions que puguen deixar el sistema en estat inconsistent

Punts mínims de control:
- què passa si es demana un recurs que no existix
- què passa si es guarda informació incompleta o incompatible
- què passa si es reutilitzen dades amb un estat ja no vàlid
- què passa si la persistència falla o retorna una situació inesperada

## Validacions lligades al model
Les validacions del Repte 3 ja no han de quedar només com a comprovacions superficials del flux. Han d'estar lligades al model i a les seues regles:
- camps obligatoris
- formats o restriccions bàsiques del domini
- coherència entre estats o relacions
- protecció davant operacions que contradiguen la lògica del model

Criteri pràctic:
- la validació d'entrada no substituïx la validació del model
- si una regla de negoci depén de dades persistides, s'ha de validar prop del model o del cas d'ús que la governa
- el tractament d'errors ha de reflectir si falla el format, la regla del model o l'accés a dades

## Riscos habituals
- modelar dades copiant l'estructura temporal del Repte 2 sense revisar si té sentit persistent
- barrejar consultes, regles de negoci i respostes finals en el mateix mètode
- afegir persistència però sense revisar coherència ni integritat bàsica
- definir validacions en documentació però no aplicar-les en el flux real
- assumir que l'ORM o la llibreria resol automàticament consistència i seguretat
- no deixar clar quines parts del model hauran d'obrir-se després com a API al Repte 4

## Evidències esperades
S'espera trobar evidències com:
- model o esquema de dades recognoscible i alineat amb el domini
- operacions de persistència aplicades als casos d'ús prioritaris
- proves mínimes o verificacions sobre recuperació, creació i errors de dades
- commits que mostren ajustos de model, accés a dades i regles de consistència
- documentació tècnica actualitzada sobre model, persistència i limitacions
- AI log si la IA ha ajudat a definir model, consultes, validacions o proves

## Checklist final
- existix un model de dades mínim i recognoscible del domini
- la persistència és funcional en els fluxos prioritaris
- hi ha control mínim sobre dades inexistents, invàlides o inconsistents
- les validacions rellevants estan lligades al model i no només al punt d'entrada
- el resultat actual és prou estable per exposar endpoints al Repte 4 sense reestructuració crítica
