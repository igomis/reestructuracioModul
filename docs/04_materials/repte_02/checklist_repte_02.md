# Checklist del Repte 2

## Finalitat

Esta checklist servix per revisar si el Repte 2 ja aporta un flux funcional prou clar, verificable i preparat per passar després a refactorització arquitectònica al Repte 3.

## Contingut operatiu

La revisió final del Repte 2 s'ha de fer comprovant no només el cas feliç del flux, sinó també la solidesa mínima de validació, errors, conservació funcional de la informació, autenticació, proves i documentació.

Transició al Repte 3:

- el tancament del repte ha de deixar clar què s'ha de reorganitzar en capes o components equivalents
- també ha de deixar identificades les validacions, errors i punts de persistència que convindrà encapsular millor
- també ha de deixar visible una primera regla o comprovació encapsulada en una classe simple i provada automàticament
- la persistència pot aparéixer ja com a suport funcional, però encara no és el focus principal d'avaluació

La sessió `7` ha de servir per introduir POO mínima, Composer/autoload i una prova unitària inicial sobre una regla real del flux, no per reconstruir `R2` amb l'arquitectura completa de `R3`.

## Conceptes mínims que s'han de poder defensar

- **Identificació**: com l'usuari declara qui és.
- **Autenticació**: com el sistema comprova eixa identitat i crea o reconeix sessió vàlida.
- **Autorització**: com el sistema decidix si una persona autenticada pot executar una operació concreta.
- **Estat**: quina informació temporal permet continuar el flux entre peticions.
- **Sessió**: quin mecanisme manté part d'eixe estat associat a un client.

El repte no es considera prou verificat si l'equip usa estos termes com a sinònims o no pot assenyalar en el codi on es comprova cada cosa.

### Flux de dades i reutilització

- [ ] existix una entrada de dades útil dins del domini
- [ ] el backend mostra errors de validació de manera interpretable
- [ ] l'usuari pot corregir la dada i repetir el flux
- [ ] la informació correcta queda conservada amb un mecanisme simple o controlat
- [ ] el projecte pot tornar a mostrar, recuperar o llistar eixa informació

### Primera peça testable

- [ ] existeix `composer.json` o alternativa equivalent amb autoload
- [ ] existeix una classe simple del domini o servei
- [ ] la classe no depén directament de `$_POST`, `$_SESSION`, `$_COOKIE` ni HTML
- [ ] existeix una prova unitària mínima o script automàtic equivalent
- [ ] el test s'ha executat i el resultat queda documentat
- [ ] si apareixen més classes, llibreries externes o API, es presenten com a ampliació o pont cap als reptes següents

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
- [ ] s'ha executat un cas invàlid per validació, amb error interpretable i possibilitat de correcció
- [ ] s'ha executat un cas no autenticat contra una operació protegida
- [ ] s'ha executat un cas amb sessió caducada, tancada o estat invàlid
- [ ] s'ha executat un cas d'accés a operació protegida que comprove la restricció definida
- [ ] les verificacions deixen rastre al repositori o a la documentació tècnica

Taula mínima recomanada:

| Cas | Entrada o situació | Resultat esperat | Resultat obtingut | Incidència o ajust |
|---|---|---|---|---|
| cas vàlid |  |  |  |  |
| cas invàlid per validació |  |  |  |  |
| cas no autenticat |  |  |  |  |
| sessió caducada o estat invàlid |  |  |  |  |
| accés a operació protegida |  |  |  |  |

### README actualitzat

- [ ] el `README` o documentació equivalent explica com provar el mòdul
- [ ] les instruccions descriuen l'estat real del codi

### AI log si s'ha usat IA

- [ ] existix AI log o registre equivalent si s'ha utilitzat assistència
- [ ] l'ús de IA queda validat amb execució, prova o contrast tècnic
- [ ] queda indicat si la IA s'ha usat per esquelets inicials, interpretació d'errors, millora de proves o documentació
- [ ] l'equip pot explicar què ha acceptat, què ha descartat i què ha modificat del suggeriment de la IA

### Preparació per al Repte 3

- [ ] la sessió `7` deixa clar què s'ha pogut provar unitàriament en `R2` i què encara queda reservat per a `R3`
- [ ] estan identificats punts a reorganitzar en MVC o arquitectura equivalent
- [ ] estan identificades validacions o errors que convindrà encapsular millor
- [ ] el resultat actual es pot refactoritzar sense reconstruir la funcionalitat des de zero
