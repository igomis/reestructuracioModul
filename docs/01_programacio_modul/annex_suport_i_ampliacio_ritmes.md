# Annex de suport i ampliació segons ritmes d'aprenentatge

## Finalitat del document
Separar en una peça reusable les estratègies de suport, consolidació i ampliació del curs perquè el professorat puga intervenir sobre ritmes diferents sense desfer la seqüència general ni convertir el mòdul en diversos recorreguts paral·lels.

Este annex complementa [guia_sessio_a_sessio_20_setmanes.md](guia_sessio_a_sessio_20_setmanes.md) i [programacio_aula_per_repte.md](programacio_aula_per_repte.md). La guia sessió a sessió diu què convé fer cada setmana; esta peça diu com sostenir eixa seqüència quan els equips no avancen al mateix ritme.

## Perfil d'alumnat endarrerit
Es considera alumnat endarrerit, a efectes docents del mòdul, aquell que mostra una o més d'estes situacions:
- no arriba al mínim funcional no trivial del repte actual
- acumula errors de base que li impedixen aprofitar el bloc següent
- no pot defensar què ha fet ni on està el seu producte real
- presenta traçabilitat pobra, `README` desactualitzat o proves inexistents
- depén massa d'ajuda externa, inclosa IA, sense capacitat de contrast ni explicació

Lectura docent:
- no és només qüestió de “lentitud”
- és sobretot qüestió de no tindre base suficient per mantindre el fil del producte

## Perfil d'alumnat al ritme previst
Es considera alumnat al ritme previst aquell que:
- completa el mínim funcional no trivial de cada repte dins del bloc previst
- deixa evidències reproduïbles i documentació operativa bàsica
- pot avançar al repte següent sense arrossegar bloquejos crítics
- usa la IA, si la usa, amb rastre mínim i capacitat de defensa

Este perfil no implica excel·lència tècnica, sinó continuïtat viable del producte dins de la seqüència del curs.

## Perfil d'alumnat avançat
Es considera alumnat avançat aquell que:
- arriba abans d'hora al mínim funcional del repte
- mostra autonomia real en proves, documentació o millora de decisions tècniques
- pot ampliar el cas d'ús del producte sense desconnectar-se del repte central
- manté qualitat d'evidències i capacitat de defensa, no només velocitat

Risc típic:
- convertir l'avantatge de ritme en treball paral·lel desconnectat del producte base o de la seqüència comuna

## Estratègies d'intervenció docent
Intervencions recomanades per a alumnat endarrerit:
- reduir abast al flux principal del repte
- revisar primer el producte real abans que el discurs o la intenció de l'equip
- imposar microcheckpoint curt amb evidència mínima obligatòria
- prioritzar correcció de validació, proves, `README` i traçabilitat per damunt d'afegir noves funcions
- fer modelatge curt d'un únic bloqueig, no una reexplicació global del tema

Intervencions recomanades per a alumnat al ritme previst:
- mantindre checkpoints normals
- usar els apunts reals com a guia de tancament operatiu
- reforçar defensa i verificació en cada canvi de repte
- evitar ampliar abast si encara no hi ha evidència sòlida del mínim

Intervencions recomanades per a alumnat avançat:
- donar ampliacions lligades al mateix flux funcional
- reforçar proves, documentació, errors, observabilitat o defensa tècnica
- permetre una regla de negoci addicional o una millor qualitat del mateix producte
- revisar que l'ampliació no trenque calendari ni exigència comuna

## Mínim funcional exigible per no perdre el fil del curs
Per mantindre's dins del curs, cada equip hauria de sostindre com a mínim:
- `R1`: repositori usable, `README`, primera peça funcional real i primer registre de dades
- `R2`: flux autenticat o equivalent amb una operació de negoci real i errors mínims controlats
- `R3`: una funcionalitat del producte ja persistent i explicable amb arquitectura més mantingible
- `R4`: una part rellevant del producte exposada com a `API` usable i provada
- `R5`: una integració o flux híbrid amb valor real i defensa final preparada

Regla docent:
- si un equip no sosté este mínim, no convé empényer-lo al repte següent només per calendari

## Estratègies d'ampliació sense desconnectar del producte base
Ampliacions recomanables:
- afegir proves més completes del mateix flux
- millorar tractament d'errors i missatges del servidor
- documentar millor contracte, decisions o consum d'`API`
- afegir una regla de negoci addicional coherent amb el domini
- ampliar control d'accés o permisos sobre una funcionalitat que ja existix
- reforçar la integració final amb millor traçabilitat o control d'incidències

Ampliacions no recomanables:
- obrir un subprojecte nou
- canviar de domini o focus del producte a meitat de curs
- afegir tecnologia nova sense impacte clar en el producte central
- convertir l'ampliació en treball ornamental per “ocupar temps”

## Moments en què convé reagrupar o reconduir equips
Convé reagrupar o reconduir quan:
- després de `R1` un equip no ha passat d'esquelet a primera funcionalitat real
- després de `R2` no hi ha operació de negoci protegida reproduïble
- a l'entrada de `R4` la persistència encara no és prou estable
- abans de `R5` el grup continua arrossegant incidències bàsiques de `R3` o `R4`
- hi ha un desequilibri intern fort entre membres que impedix la defensa tècnica del treball

Reconducció recomanada:
- reduir abast
- fixar una sola evidència obligatòria de recuperació
- ajornar tota ampliació no nuclear
- revisar responsabilitats internes de l'equip

## Criteris per simplificar sense perdre RA
Simplificar és acceptable quan:
- es manté el resultat d'aprenentatge nuclear del repte
- el flux funcional continua sent real i defensable
- la simplificació reduïx quantitat, no veracitat del producte
- es continua podent revisar validació, evidències i autoria

Exemples de simplificació acceptable:
- menys camps en un formulari
- menys entitats o relacions en `R3`
- menys endpoints en `R4`, si continuen sent nuclears
- una integració més curta en `R5`, si continua resolent una necessitat real

Exemples de simplificació no acceptable:
- substituir un flux real per una demo preparada
- eliminar proves o documentació essencial
- deixar el repte en infraestructura sense cas d'ús
- compensar falta de producte amb presentació o discurs

## Criteris per ampliar sense convertir-ho en treball paral·lel desconnectat
Una ampliació és acceptable si:
- millora el mateix producte base
- manté el mateix repte i la mateixa seqüència
- no debilita la capacitat de tancament dins de les dues primeres avaluacions
- es pot revisar amb les mateixes evidències i instruments del curs

Una ampliació és problemàtica si:
- obri un segon recorregut que el professorat no pot seguir
- exigix instruments nous només per a eixe equip
- posa en risc el tancament del producte principal
- desplaça l'atenció des de la defensa del producte real cap a una peça lateral

## Definition of done del document
Este annex es considera completat quan:
- diferencia amb claredat alumnat endarrerit, alumnat al ritme previst i alumnat avançat
- oferix criteris docents de suport, reconducció i ampliació sense trencar la seqüència comuna
- fixa el mínim funcional exigible per no perdre el fil del curs
- explica quan simplificar i quan ampliar sense perdre resultats d'aprenentatge
- és reusable com a complement directe de la guia sessió a sessió i de la programació per repte
