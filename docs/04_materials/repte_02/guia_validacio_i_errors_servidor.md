# Guia de validació i errors del servidor

## Finalitat
Assegurar que el Repte 2 no es resol només amb un flux aparentment funcional, sinó amb un comportament de servidor coherent davant dades incorrectes, credencials invàlides i accessos no permesos.

Esta guia s'ha d'usar per decidir què es valida al backend, com es responen els errors i quines comprovacions mínimes s'han de deixar registrades com a evidència autèntica del repte.

## Contingut operatiu

### Què validar al servidor
Com a mínim, el servidor ha de validar:
- presència dels camps obligatoris del registre o del login
- format bàsic dels camps que tinguen restriccions clares
- coherència mínima de credencials i identificació de l'usuari
- intents d'accés a rutes protegides sense sessió o estat equivalent vàlid
- dades buides, mal formades o inconsistents que puguen afectar el flux
- restriccions bàsiques que el domini exigisca per donar d'alta o autenticar usuari

Criteri pràctic:
- la validació ha d'estar al servidor encara que existisca ajuda al client
- els errors han de ser interpretables per l'equip i per qui revise el repte
- les comprovacions mínimes han de respondre a casos reals del flux, no a llistes teòriques desconnectades

### Tractament mínim d'errors
El tractament d'errors del Repte 2 ha d'incloure:
- missatges o respostes coherents per camps obligatoris absents o invàlids
- resposta clara per credencials incorrectes
- resposta clara per accés no autenticat a operació protegida
- tractament consistent d'errors repetits, sense respostes contradictòries
- absència d'informació tècnica innecessària cap a l'usuari final

Mínim exigible:
- diferenciar error de validació, error d'autenticació i error d'accés
- mantindre un format de resposta o de feedback recognoscible
- registrar o poder reproduir què ha passat quan apareix una incidència

### Casos correctes i casos límit
Casos correctes mínims:
- registre vàlid
- login vàlid
- accés vàlid a una operació protegida
- logout i comprovació posterior d'estat no autenticat

Casos límit mínims:
- camp obligatori absent
- camp amb format invàlid o massa dèbil segons la regla definida
- credencials incorrectes
- accés a recurs protegit sense sessió
- intent de reutilitzar un estat que ja no hauria de ser vàlid després del logout

### Evidències esperades
S'espera trobar evidències com:
- matriu curta o llistat de validacions mínimes aplicades
- registre de casos correctes i casos límit executats
- commits que mostren ajustos en validació o tractament d'errors
- documentació tècnica actualitzada amb comportaments rellevants
- proves automatitzades, peticions registrades o verificacions equivalents segons l'stack
- AI log si la IA ha ajudat a definir regles, missatges o proves

### Transició al Repte 3
El Repte 2 hauria d'acabar amb estes pistes clares per al pas següent:
- quines validacions s'han de moure des del flux superficial cap al model o al cas d'ús
- quins errors convé tractar de manera més centralitzada i coherent
- quins casos límit afectaran directament l'arquitectura i la persistència del Repte 3

## Errors habituals o riscos
- confiar en validació del client i no repetir-la al servidor
- usar missatges genèrics que no permeten entendre què falla
- mesclar en la mateixa resposta errors de camps, credencials i permisos
- mostrar traces o informació interna que no aporta valor funcional
- provar només el cas correcte i oblidar casos límit del flux
- deixar validacions definides en documentació però no aplicades en el codi real

## Checklist final
- el servidor valida camps obligatoris i dades clarament invàlides
- es diferencien errors de validació, autenticació i accés
- hi ha casos correctes i casos límit executats i registrats
- la documentació o les proves reflectixen el comportament real del backend
- els errors són comprensibles i compatibles amb un entorn professional realista
- el tractament actual deixa base clara per encapsular validacions i errors al Repte 3
