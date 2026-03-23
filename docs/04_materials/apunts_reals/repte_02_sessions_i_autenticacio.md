# Apunts reals del Repte 2. Sessions i autenticació

## Finalitat del document
Convertir el Repte 2 en un apunt de treball real, curt i executable, pensat perquè professorat i alumnat tinguen clara la seqüència mínima per construir la primera funcionalitat sòlida del producte: registre, autenticació, estat equivalent, validacions bàsiques, errors previsibles i evidències verificables.

Este repte no consistix a "fer un login". El que s'espera és obrir el primer flux funcional real del producte amb autenticació, control d'accés i una operació de negoci recognoscible que es puga provar i defensar.

## Què sap ja l'alumnat
- ja ha triat domini i stack al Repte 1
- ja té repositori actiu, entorn funcional i primer `README`
- ja coneix el criteri del curs sobre traçabilitat, evidències i `AI log`
- ja té base prèvia de Git/GitHub; per tant, ací només es revisa com a metodologia de treball i no com a iniciació

## Què s'ha de recordar breument
- el repte no consistix a "fer un login", sinó a obrir el primer flux real del producte
- el servidor ha de validar i respondre amb criteri mínim, encara que hi haja ajuda al client
- un flux només compta si es pot reproduir i defensar
- la IA és admissible com a suport, però s'ha de poder explicar què ha suggerit i què s'ha verificat després

## Què ha d'explicar el professorat
- quin és el mínim funcional exigible: registre o alta, login, logout i una operació de negoci protegida
- diferència entre autenticació, autorització i estat de sessió o equivalent
- què s'espera com a evidència: flux funcional, casos límit, proves bàsiques, `README` actualitzat i traçabilitat del procés
- per què este repte es tancarà només si deixa una base refactoritzable per al Repte 3

## Què s'ha de modelar en directe
- una alta d'usuari amb validació bàsica de camps obligatoris
- un login amb resposta clara en cas correcte i incorrecte
- una comprovació d'accés a una ruta o operació protegida amb valor real dins del domini
- una restricció simple de rol, permís o condició de negoci quan tinga sentit
- un exemple breu de prova o verificació manual reproduïble del flux
- un exemple curt d'anotació al `README` o a l'`AI log` després d'un canvi rellevant

## Què treballa l'alumnat amb autonomia
- decidir quin actor o usuari té sentit en el domini triat
- implementar registre, login, logout o estat equivalent
- protegir una operació real del producte i definir la seua regla mínima d'accés
- validar dades d'entrada i gestionar errors mínims
- deixar rastre de proves, correccions i actualització de documentació

## Exemple mínim orientatiu
Exemple orientatiu de recorregut mínim:
1. Crear usuari amb `nom`, `email` i `password`.
2. Rebutjar registre si falta un camp obligatori.
3. Permetre login només amb credencials correctes.
4. Donar accés autenticat a una operació del domini, per exemple:
   - crear una incidència
   - reservar una cita
   - consultar un recurs intern protegit
5. Bloquejar eixa operació si l'usuari no està autenticat.
6. Després del logout, tornar a provar l'operació protegida i verificar que ja no és accessible.

Criteri docent:
- l'exemple no s'ha de copiar literalment
- servix per entendre la seqüència mínima que s'ha de poder demostrar
- el punt no és només autenticar, sinó demostrar que el producte ja resol una primera acció de negoci amb sentit

## Errors habituals
- resoldre només el cas feliç i no provar dades incorrectes
- deixar la validació només al client
- tindre login aparent però sense protecció real d'una operació
- deixar l'autenticació desconnectada d'una necessitat real del domini
- no comprovar què passa després del logout
- mostrar captures o vídeo, però no una execució reproduïble
- usar IA per generar fluxos o controladors sense revisar què fa realment el servidor

## Com es verifica que funciona
Per donar el repte per verificat, cal poder demostrar com a mínim:
- registre correcte
- registre incorrecte amb error interpretable
- login correcte
- login incorrecte
- accés autoritzat a una operació protegida amb valor funcional real
- accés denegat sense autenticació o amb estat ja invalidat
- comportament coherent d'una restricció bàsica de rol, permís o condició de negoci quan s'haja definit
- logout i comprovació posterior

Formats de verificació acceptables:
- proves automatitzades bàsiques
- peticions guardades o col·lecció de proves
- registre manual clar i reproduïble al `README`
- demostració tècnica en revisió docent amb repositori i aplicació oberts

## Evidències que s'han d'entregar
- repositori amb traçabilitat recognoscible del flux implementat
- `README` actualitzat amb com provar el Repte 2
- prova o registre de casos correctes i casos límit
- operació del domini realment protegida
- evidència de la regla mínima d'accés o restricció aplicada al flux principal
- resposta coherent del servidor en errors mínims
- `AI log` si s'ha utilitzat IA en decisions, esquelets, depuració o validacions

## Checklist final del repte
- [ ] existix registre o alta d'usuari amb validació mínima al servidor
- [ ] existix login funcional amb comprovació de credencials
- [ ] existix logout funcional o invalidació equivalent d'estat
- [ ] existix almenys una operació del domini protegida i lligada a una funcionalitat real del producte
- [ ] existix una regla mínima de rol, permís o restricció recognoscible quan el cas d'ús ho demana
- [ ] el servidor diferencia cas correcte, validació incorrecta i accés no autoritzat
- [ ] hi ha almenys una prova o verificació clara del flux complet
- [ ] el `README` explica com reproduir el repte
- [ ] l'ús de la IA, si existix, està registrat i contrastat

## Connexió amb el Repte 3
El Repte 2 no queda tancat només quan "funciona", sinó quan deixa preparat el pas a arquitectura i persistència. En concret, hauria de deixar identificat:
- quina part del flux convé refactoritzar primer
- quines validacions s'han de moure o encapsular millor
- quina operació protegida serà el primer cas d'ús a reorganitzar amb persistència

Lectura de transició:
- si el flux del Repte 2 és real però encara massa acoblat, el Repte 3 tindrà sentit
- si el flux del Repte 2 és només una demo, el Repte 3 quedarà construït sobre una base falsa
