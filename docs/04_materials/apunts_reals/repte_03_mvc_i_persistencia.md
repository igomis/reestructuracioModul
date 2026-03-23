# Apunts reals del Repte 3. Arquitectura, persistència i qualitat tècnica

## Finalitat del document
Convertir el Repte 3 en un apunt de treball real, curt i executable, pensat perquè professorat i alumnat tinguen clara la seqüència mínima per transformar el backend funcional del Repte 2 en una base mantenible: arquitectura per capes o equivalent, persistència real del domini, validacions coherents i primer nivell de qualitat tècnica defensable.

## Què sap ja l'alumnat
- ja té un flux funcional mínim del producte amb autenticació i operació protegida
- ja coneix el domini triat i els primers casos d'ús que tenen valor real
- ja sap què és una evidència autèntica, què ha d'explicar al `README` i quan toca registrar un `AI log`
- ja té base prèvia de Git/GitHub; per tant, ací només es revisa com a metodologia de treball i traçabilitat, no com a iniciació

## Què s'ha de recordar breument
- el repte no consistix a "ordenar carpetes", sinó a deixar una base que es puga mantindre i ampliar
- una arquitectura només compta si separa responsabilitats reals i ajuda a entendre on passa cada cosa
- la persistència ha de substituir l'estat provisional o massa acoblat, no duplicar-lo
- la IA pot ajudar a refactoritzar o modelar, però s'ha de poder justificar per què s'ha acceptat una estructura i no una altra

## Què ha d'explicar el professorat
- quin és el mínim exigible de separació de responsabilitats segons l'itinerari triat
- quina diferència hi ha entre una persistència aparent i una persistència realment integrada al producte
- com es relacionen model de dades, validacions, errors i casos d'ús principals
- per què este repte es tanca només si deixa preparada una base estable per publicar i consumir API al Repte 4

## Què s'ha de modelar en directe
- una refactorització curta d'un flux existent per separar entrada, lògica i accés a dades
- la incorporació d'una entitat persistent del domini amb operacions bàsiques de creació i consulta
- una validació lligada al model i no només a l'entrada superficial del formulari o la petició
- una comprovació breu que el flux funcional del Repte 2 continua funcionant després del canvi
- una anotació curta al `README` o a l'`AI log` explicant una decisió d'arquitectura o persistència

## Què treballa l'alumnat amb autonomia
- decidir quines peces del Repte 2 cal refactoritzar primer
- definir un model de dades mínim coherent amb el producte triat
- passar d'estat temporal o acoblat a persistència funcional real
- reorganitzar el codi en capes o patró equivalent segons l'itinerari
- provar els casos crítics i actualitzar documentació i traçabilitat

## Exemple mínim orientatiu
Exemple orientatiu de recorregut mínim:
1. Identificar una entitat principal del domini, per exemple `incidencia`, `reserva` o `recurs`.
2. Crear una estructura persistent amb camps mínims i identificador clar.
3. Separar la recepció de la petició de la lògica de negoci i de l'accés a dades.
4. Permetre crear una entitat i recuperar-la amb persistència real.
5. Rebutjar dades incoherents o incompletes amb resposta interpretable.
6. Tornar a provar el flux protegit del Repte 2 per confirmar que no s'ha trencat.

Criteri docent:
- l'exemple no s'ha de copiar literalment
- servix per entendre el mínim que s'ha de poder demostrar en qualsevol domini o stack

## Errors habituals
- confondre refactorització amb canvi cosmètic de carpetes o noms de fitxer
- mantindre lògica de negoci, validació i persistència barrejades al mateix punt d'entrada
- afegir base de dades o ORM, però continuar depenent d'estat temporal o de dades inconsistents
- modelar dades sense pensar quines operacions reals s'han de fer després
- no comprovar regressions del Repte 2 després de reorganitzar el projecte
- acceptar una proposta d'estructura generada amb IA sense entendre si encaixa realment amb l'itinerari triat

## Com es verifica que funciona
Per donar el repte per verificat, cal poder demostrar com a mínim:
- existix una arquitectura recognoscible per capes o equivalent
- existix una entitat principal amb persistència funcional real
- es poden crear i recuperar dades del domini amb coherència bàsica
- el sistema rebutja dades inexistents, incompletes o incoherents en els casos mínims rellevants
- el flux funcional principal del Repte 2 continua actiu després de la refactorització
- el producte queda prou estable per identificar recursos i operacions que després seran API

Formats de verificació acceptables:
- proves automatitzades bàsiques sobre casos crítics
- verificacions manuals reproduïbles descrites al `README`
- col·lecció de peticions o comprovacions guardades
- revisió docent amb repositori obert, execució funcional i defensa tècnica de l'estructura triada

## Evidències que s'han d'entregar
- repositori amb traçabilitat recognoscible del pas de flux funcional a estructura mantenible
- `README` actualitzat amb com provar la persistència i quins components estructuren el projecte
- evidència de creació i recuperació de dades del domini amb persistència real
- prova o registre de validacions, errors i regressions mínimes
- justificació tècnica breu de l'arquitectura o patró equivalent adoptat
- `AI log` si s'ha utilitzat IA en refactorització, modelat, persistència o depuració

## Checklist final del repte
- [ ] existix una separació recognoscible entre entrada, lògica i persistència, o equivalent segons l'itinerari
- [ ] existix almenys una entitat principal del domini amb persistència funcional real
- [ ] les validacions mínimes estan lligades al model i no només a l'entrada superficial
- [ ] el sistema gestiona com a mínim dades inexistents, incompletes o incoherents
- [ ] el flux principal del Repte 2 continua funcionant després de la reorganització
- [ ] hi ha almenys una prova o verificació clara de persistència i regressió
- [ ] el `README` explica com reproduir el Repte 3 i quina estructura s'ha adoptat
- [ ] l'ús de la IA, si existix, està registrat i contrastat

## Connexió amb el Repte 4
El Repte 3 no queda tancat només quan "guarda dades", sinó quan deixa clara una base estable per exposar recursos com a API. En concret, hauria de deixar identificat:
- quines entitats o casos d'ús passen a ser recursos publicables
- quines validacions i errors hauran de formar part del contracte API
- quina estructura del projecte ja és prou estable per suportar endpoints, documentació i proves de consum

Lectura de transició:
- si el Repte 3 deixa una arquitectura defensable i una persistència coherent, el Repte 4 pot centrar-se en contracte, publicació i consum
- si el Repte 3 només reorganitza aparença o guarda dades sense criteri, el Repte 4 naixerà amb una API inestable
