# Guia d'integració externa i flux híbrid

## Finalitat

Ajudar a convertir el Repte 5 en una integració amb valor real, on l'API del curs deixe de ser només un backend publicat i passe a formar part d'un flux complet amb consum extern, automatització o procés híbrid verificable.

Esta guia no busca una demo vistosa. El seu objectiu és que l'equip trie una integració defensable, puga descriure clarament les dades que entren i ixen del flux i deixe evidència real de funcionament i de gestió d'incidències.

## Què és una integració externa amb valor real

Una integració externa amb valor real és aquella que:

- partix d'un cas de negoci recognoscible del producte
- reutilitza l'API pròpia com a contracte estable
- connecta amb un servei extern, webhook, eina d'automatització o procés equivalent amb utilitat clara
- genera una eixida observable: notificació, actualització, sincronització, registre o automatització de tasca
- es pot provar en camí correcte i en camí de fallada

No és suficient:

- una crida ornamental a un servei extern sense impacte funcional
- una integració fictícia no connectada amb el domini
- un flux que només es veu en captures però no deixa rastre executable

## Criteris per triar una integració adequada

Convé triar una integració quan complix, com a mínim, estos criteris:

- aprofita un endpoint real publicat al Repte 4
- aporta valor a una operació del domini: incidència, reserva, recurs o estat intern
- es pot explicar de punta a punta sense zones opaques
- es pot provar amb dades controlades
- permet detectar errors i documentar-los

Preguntes útils de selecció:

- quin esdeveniment del producte dispara el flux?
- quin actor o servei rep el resultat?
- què passa si el servei extern no respon o respon malament?
- el flux ajuda a entendre millor el producte o només afegix superfície?

## Dades d'entrada i eixida del flux

Abans d'implementar res, l'equip hauria de mapar:

- esdeveniment d'entrada del flux
- endpoint o recurs de l'API que participa
- dades que s'envien al servei extern o a l'automatització
- transformacions necessàries
- resposta esperada o efecte final del procés
- registre o evidència observable del resultat

Mapatge mínim recomanat:

- origen de la dada
- format d'entrada
- pas de transformació si n'hi ha
- destí final
- resposta o eixida del flux

## Control mínim d'errors i incidències

El flux híbrid ha de controlar, com a mínim:

- fallada d'autenticació o accés a l'API pròpia
- dada d'entrada invàlida o incompleta
- error del servei extern o de l'eina d'orquestració
- resposta inesperada o timeout
- possibilitat de reintentar, registrar o diagnosticar la incidència

Criteri pràctic:

- no cal observabilitat avançada, però sí una traça mínima de què ha fallat
- una integració sense camí de fallada provat no és prou defensable
- el registre d'incidència ha de permetre explicar el problema i la correcció

## Evidències a aportar

S'espera trobar evidències com:

- definició clara del cas d'integració triat
- diagrama simple o descripció explícita del flux híbrid
- proves de funcionament correcte i de fallada rellevant
- registre d'entrada, eixida i punts de control del procés
- documentació de manteniment o incidències detectades
- AI log si la IA ha ajudat a dissenyar el flux, mapar payloads o resoldre errors

## Errors habituals

- triar una integració només perquè és fàcil de mostrar, no perquè tinga valor real
- no definir clarament quina dada entra, quina es transforma i quina ix
- usar l'API pròpia només com a excusa i no com a contracte central del flux
- no provar escenaris d'error del servei extern o del workflow
- confondre automatització visual amb integració funcional
- documentar un flux idealitzat que no coincidix amb l'execució real

## Checklist final

- la integració triada té relació clara amb el domini i amb l'API del curs
- les dades d'entrada i eixida del flux estan identificades
- existix com a mínim un camí correcte i un camí de fallada provats
- el flux deixa rastre usable per debugging o manteniment
- la integració és prou clara per defensar-la tècnicament davant l'equip o el professorat
- el resultat prepara el tancament professional del producte del curs
