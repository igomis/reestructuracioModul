# MT17. Tokens funcionals del backend

Micro-presentació docent breu per a `R4S6`. Equival aproximadament a `6` diapositives.

## Diapositiva 1. Idea central

- un token funcional permet una operació puntual
- no és `OAuth`, ni `JWT` professional, ni blockchain
- ha d'estar lligat a un cas real del domini

## Diapositiva 2. Exemples

- confirmar una reserva
- cancel·lar una cita
- consultar una incidència externa
- acceptar una invitació
- validar una entrega d'inventari

## Diapositiva 3. Cicle de vida

- generació
- associació a recurs
- caducitat
- validació
- consum
- registre o revocació

## Diapositiva 4. Errors habituals

- token sense caducitat
- token amb massa permisos
- no registrar el consum
- confondre token funcional amb login
- no provar token invàlid

## Diapositiva 5. Evidència del dia

- flux tokenitzat documentat
- cas vàlid
- cas invàlid o caducat
- decisió sobre ús únic
- nota sobre riscos

## Diapositiva 6. Tancament

- el token ha de limitar, no obrir tot el sistema
- si no pots explicar què permet i què no, encara no està ben dissenyat
- pregunta final: què podria fer una persona amb este token?
