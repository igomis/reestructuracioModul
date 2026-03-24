# Com gestionar ritmes i suport

## Finalitat
Esta guia resumix com intervenir sense trencar la seqüència comuna del curs. La clau no és obrir tres recorreguts diferents, sinó ajustar abast, checkpoints i suport sobre el mateix producte base.

## Alumnat endarrerit
Senyal típica:
- no arriba al mínim funcional no trivial del repte actual
- no pot defensar què ha fet ni on està el producte real
- té traçabilitat pobra, proves inexistents o dependència excessiva de la IA

Resposta docent:
- reduir abast al flux principal
- fixar un microcheckpoint curt amb una sola evidència obligatòria
- prioritzar validació, proves, `README` i traçabilitat
- bloquejar ampliacions fins que el mínim estiga tancat

## Alumnat al ritme previst
Senyal típica:
- completa el mínim funcional de cada repte dins del bloc previst
- deixa evidències reproduïbles
- pot explicar el flux sense improvisació

Resposta docent:
- mantindre checkpoints normals
- reforçar defensa i verificació en cada canvi de repte
- evitar ampliar abast si el mínim encara és feble

## Alumnat avançat
Senyal típica:
- arriba prompte al mínim funcional
- millora proves, documentació o qualitat tècnica sense perdre el focus
- manté capacitat de defensa, no només velocitat

Resposta docent:
- donar ampliacions sobre el mateix flux funcional
- reforçar errors, proves, permisos o observabilitat
- evitar obrir subprojectes o dominis laterals

## Mínim funcional exigible per no perdre el fil
- `R1`: repositori usable, `README`, primera peça funcional i primer registre de dades
- `R2`: flux protegit o equivalent amb una operació de negoci real
- `R3`: funcionalitat persistent i arquitectura explicable
- `R4`: part rellevant del producte exposada com a `API` usable
- `R5`: integració o flux híbrid amb valor real i defensa preparada

## Quan simplificar
És acceptable simplificar si:
- es manté el resultat d'aprenentatge nuclear
- el flux continua sent real i defensable
- es redueix quantitat, no veracitat del producte

No és acceptable simplificar si:
- el flux real es canvia per una demo
- desapareixen proves o documentació essencial
- el repte es queda en infraestructura sense cas d'ús

## Ampliacions sense perdre el producte base
Sí convé:
- afegir una regla de negoci coherent
- reforçar proves, errors o documentació
- millorar permisos o observabilitat del mateix flux

No convé:
- canviar de domini a meitat de curs
- obrir tecnologia nova sense impacte clar
- convertir l'ampliació en treball paral·lel que el professorat no pot seguir
