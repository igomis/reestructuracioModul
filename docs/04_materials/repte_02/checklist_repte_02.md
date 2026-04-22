# Checklist del Repte 2

## Finalitat

Esta checklist servix per revisar si el Repte 2 ja aporta un flux funcional prou clar, verificable i preparat per passar després a refactorització arquitectònica al Repte 3.

## Contingut operatiu

La revisió final del Repte 2 s'ha de fer comprovant no només el cas feliç del flux, sinó també la solidesa mínima de validació, errors, conservació funcional de la informació, autenticació, proves i documentació.

Transició al Repte 3:

- el tancament del repte ha de deixar clar què s'ha de reorganitzar en capes o components equivalents
- també ha de deixar identificades les validacions, errors i punts de persistència que convindrà encapsular millor
- la persistència pot aparéixer ja com a suport funcional, però encara no és el focus principal d'avaluació

Si el professorat obri un tram final de refactorització lleu, esta revisió ha de servir per netejar i fer més mantenible el que ja funciona, no per reconstruir `R2` amb l'arquitectura completa de `R3`.

### Flux de dades i reutilització

- [ ] existix una entrada de dades útil dins del domini
- [ ] el backend mostra errors de validació de manera interpretable
- [ ] l'usuari pot corregir la dada i repetir el flux
- [ ] la informació correcta queda conservada amb un mecanisme simple o controlat
- [ ] el projecte pot tornar a mostrar, recuperar o llistar eixa informació

### Refactorització final opcional

- [ ] si s'ha activat, la revisió final millora claredat o mantenibilitat sense trencar el flux funcional
- [ ] s'ha reduït duplicació, barreja excessiva de `HTML + PHP` o acoblament innecessari
- [ ] hi ha una justificació breu del abans/després
- [ ] si apareixen classes, objectes o persistència més formal, es presenten com a tast o pont cap a `R3`

## Errors habituals o riscos

- donar per tancat el repte només perquè el login funciona una vegada
- no comprovar l'accés protegit després del logout
- deixar validacions i errors com a comportament implícit, no documentat ni provat
- arribar al Repte 3 sense saber quin cas d'ús es refactoritzarà primer

## Checklist final

### Autenticació funcional

- [ ] existix registre o alta d'usuari amb comportament operatiu
- [ ] existix login funcional amb comprovació de credencials
- [ ] existix logout funcional
- [ ] hi ha almenys una operació del domini protegida per autenticació

### Sessió o estat equivalent

- [ ] el backend conserva o reconeix l'estat autenticat de manera coherent
- [ ] el backend comprova l'estat abans de permetre accés a una operació protegida
- [ ] després del logout, l'estat deixa de ser vàlid per al recurs protegit

### Validacions mínimes

- [ ] el servidor valida camps obligatoris del registre o del login
- [ ] hi ha tractament de dades invàlides o inconsistents
- [ ] si el cas d'ús ho demana, hi ha control bàsic d'imatge o fitxer
- [ ] les regles mínimes estan alineades amb el comportament real del flux

### Tractament d'errors

- [ ] existixen respostes o missatges coherents per validació incorrecta
- [ ] existixen respostes o missatges coherents per credencials incorrectes
- [ ] existixen respostes o missatges coherents per accés no autoritzat o no autenticat

### Proves mínimes executades

- [ ] s'ha executat almenys un cas correcte complet del flux
- [ ] s'ha executat almenys un cas d'error rellevant
- [ ] s'ha comprovat l'accés protegit abans o després del logout
- [ ] les verificacions deixen rastre al repositori o a la documentació tècnica

### README actualitzat

- [ ] el `README` o documentació equivalent explica com provar el mòdul
- [ ] les instruccions descriuen l'estat real del codi

### AI log si s'ha usat IA

- [ ] existix AI log o registre equivalent si s'ha utilitzat assistència
- [ ] l'ús de IA queda validat amb execució, prova o contrast tècnic

### Preparació per al Repte 3

- [ ] estan identificats punts a reorganitzar en MVC o arquitectura equivalent
- [ ] estan identificades validacions o errors que convindrà encapsular millor
- [ ] el resultat actual es pot refactoritzar sense reconstruir la funcionalitat des de zero
