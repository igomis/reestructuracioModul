# Guia de bootstrap NestJS

## Finalitat

Oferir una base operativa perquè l'itinerari `NestJS` puga arrancar amb criteri tècnic a partir de `R3`, sense separar l'entrada al framework dels objectius reals del projecte base del curs.

Esta guia no és un resum general del framework. El seu objectiu és deixar una arrancada prou clara perquè l'equip puga construir un backend mantenible, autenticable, persistent i preparat per publicar API i integrar-se després amb fluxos híbrids.

## Contingut operatiu

### Quan té sentit usar NestJS dins del projecte

Convé usar `NestJS` quan:

- l'equip entra al contrast de frameworks a partir de `R3`
- es vol una via de backend TypeScript compatible amb el projecte base del curs
- el domini triat necessita una evolució clara des de autenticació i persistència fins a API i integració
- l'equip pot explicar amb criteri les peces de `NestJS` i no només el que genera la `CLI`

No té sentit usar-lo si:

- el projecte depén només de plantilles, generadors o snippets no entesos
- l'equip no sap seguir el recorregut mínim entre entrada HTTP, lògica, persistència i resposta
- es delega tota la comprensió del framework a la `CLI` o a la IA

### Estructura mínima del projecte

Per al curs, un projecte usable per esta via hauria de tindre com a mínim:

- arrencada funcional del servidor
- configuració clara d'entorn i dependències
- capa d'entrada recognoscible: rutes, controladors o mòduls HTTP
- separació mínima entre exposició, lògica de negoci i persistència
- model o esquema mínim del domini
- validació mínima de dades d'entrada
- proves o verificacions equivalents sobre fluxos crítics

Estructura orientativa en `NestJS`:

- `src/main.ts`
- `src/app.module.ts`
- `src/<domini>/<domini>.module.ts`
- `src/<domini>/<domini>.controller.ts`
- `src/<domini>/<domini>.service.ts`
- `src/<domini>/dto/`
- `src/<domini>/entities/` o adaptació equivalent
- `test/`

### Peces clau que cal entendre

L'equip hauria d'entendre, com a mínim:

- punt d'arrancada del servidor: `main.ts`
- capa d'exposició: `controllers`
- capa de negoci: `services` o casos d'ús equivalents
- capa de persistència: repositoris, models o accés a dades
- configuració d'entorn: variables, connexió a base de dades i ports
- capa de proves o verificacions mínimes

Criteri docent:

- no cal desplegar tota la infraestructura possible del stack
- sí que cal entendre què rep la petició, on es valida, on es resol la lògica i on es persistix
- qualsevol peça generada amb CLI o IA ha de ser explicable i revisable

### Criteri propi de l'itinerari NestJS

`NestJS` oferix una estructura guiada amb `module`, `controller`, `service`, `guard`, `pipe` i `dto`.

Criteri de tria:

- és vàlid si l'equip entén la maquinària mínima del framework i no el convertix en una capa opaca
- la comparabilitat docent es mesura per evidències, qualitat i defensa tècnica, no per quantitat de fitxers

### Evidències mínimes

S'espera trobar evidències com:

- projecte `Node.js` que arranca amb instruccions reproduïbles
- `README` actualitzat amb instal·lació, scripts i execució mínima
- estructura recognoscible d'entrada, negoci i dades
- primera verificació funcional del flux inicial
- commits que mostren una arrancada real i no una pujada compactada final
- AI log si la IA ha ajudat a triar estructura, configuració o comandaments

## Errors habituals d'arrancada

- generar un projecte `NestJS` i no entendre què fan `module`, `controller` o `service`
- barrejar configuració, rutes, lògica i persistència en el mateix punt d'entrada
- no distingir entre codi d'infraestructura del framework i codi propi del domini
- no deixar clar quin camí del projecte serà API, quin serà autenticació i quin serà persistència
- adoptar una estructura suggerida per IA sense provar que realment encaixa amb el projecte del curs

## Checklist final

- el projecte `NestJS` arranca i es pot reproduir amb instruccions clares
- l'equip entén el recorregut mínim entre entrada HTTP, negoci i persistència
- la via triada (`NestJS`) està justificada amb criteri tècnic
- hi ha evidències reals d'arrancada i primera verificació
- la base queda preparada per connectar-se amb autenticació, persistència, API i integració en els reptes següents
