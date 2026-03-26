# Guia de flux d'usuari i sessions

## Finalitat

Convertir el Repte 2 en un flux funcional clar i verificable d'accés d'usuari, de manera que l'equip puga implementar la primera funcionalitat real del producte sense desconnectar-se del projecte base ni del treball per reptes.

Esta guia s'ha d'usar per ordenar la seqüència mínima de registre, autenticació, estat de sessió i accés protegit. El valor no està en afegir opcions, sinó en aconseguir que el flux base siga coherent, defensable i reutilitzable en el pas posterior al Repte 3.

## Contingut operatiu

### Flux base

El flux mínim del Repte 2 ha de cobrir estes quatre situacions:

1. **Registre o alta d'usuari**
   El sistema rep dades bàsiques d'usuari, valida camps obligatoris, comprova restriccions mínimes i crea l'usuari o retorna errors interpretables.

2. **Login**
   El sistema comprova credencials, inicia sessió o establix estat equivalent i deixa preparada l'autenticació per a operacions protegides.

3. **Logout**
   El sistema tanca la sessió o invalida l'estat autenticat i deixa el comportament posterior en estat no autenticat.

4. **Accés protegit**
   Almenys una ruta, acció o recurs del domini triat ha d'exigir autenticació i respondre de manera coherent si l'usuari no té sessió vàlida.

Flux mínim recomanat de treball:

- definir quin tipus d'usuari o actor té sentit dins del domini triat
- concretar quina operació del producte quedarà protegida
- implementar registre i validació d'entrada
- implementar login i persistència de sessió o estat equivalent
- implementar logout i comprovació posterior
- provar accés autoritzat i accés denegat

### Punts de control del servidor

El servidor ha de controlar com a mínim:

- recepció i validació de camps obligatoris
- tractament consistent de credencials incorrectes
- creació o recuperació segura de l'usuari
- inici i tancament correcte de sessió o mecanisme equivalent
- comprovació d'usuari autenticat abans d'accedir a la part protegida
- resposta clara quan no hi ha autenticació o quan l'estat és invàlid
- coherència entre el que diu la documentació i el que realment fa el backend

Punts de revisió útils:

- què passa si l'usuari intenta repetir un registre no vàlid
- què passa si fa login amb dades incorrectes
- què passa si fa logout i intenta tornar a accedir al recurs protegit
- què passa si intenta accedir directament al recurs sense autenticar-se

### Evidències esperades

Per considerar el flux ben resolt, s'espera trobar:

- issue o microtasques que identifiquen registre, login, logout i accés protegit
- seqüència de commits que mostre construcció real del flux
- demostració funcional o registre verificable dels casos correctes i incorrectes
- prova o evidència de comprovació de sessió abans i després del logout
- documentació tècnica actualitzada del mòdul o del `README`
- AI log si la IA s'ha utilitzat per generar esquelets, resoldre errors o proposar validacions

### Transició al Repte 3

El tancament del Repte 2 hauria de deixar identificat:

- quina part del flux està massa acoblada i haurà de passar a arquitectura per capes o equivalent
- quines validacions i errors convé centralitzar o encapsular millor
- quina operació protegida del domini serà el primer cas d'ús a reorganitzar al Repte 3

## Errors habituals o riscos

- implementar només login i oblidar registre, logout o accés protegit
- validar només al client o de manera superficial i no al servidor
- confondre "usuari autenticat" amb "usuari autoritzat" sense deixar-ho clar
- deixar una sessió aparentment oberta o tancada sense comprovar l'estat real
- protegir una ruta de manera nominal però sense verificació efectiva del servidor
- presentar captures o descripcions sense evidència executable del flux complet

## Checklist final

- existix registre o alta d'usuari amb validació mínima
- existix login funcional amb comprovació de credencials
- existix logout funcional amb comprovació posterior
- existix almenys una operació protegida del domini
- el servidor diferencia accés autoritzat i accés no autoritzat
- hi ha evidències reals del flux complet i dels errors principals
- el resultat queda preparat per ser reorganitzat al Repte 3 sense reconstruir-lo des de zero
