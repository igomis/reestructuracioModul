# Guia de bootstrap Laravel

## Finalitat

Oferir una base operativa perquè l'itinerari `Laravel` es puga arrancar amb criteri tècnic, sense convertir l'entrada al framework en un problema separat dels reptes del curs.

Esta guia no busca cobrir tot Laravel. El seu objectiu és deixar una arrancada prou neta perquè l'equip puga connectar el projecte base amb els Reptes 2, 3, 4 i 5 dins d'un entorn professional realista, amb evidències autèntiques i marge de manteniment.

## Contingut operatiu

### Quan usar Laravel dins del projecte

Convé usar `Laravel` quan:

- l'equip treballa en l'itinerari `PHP + Laravel` autoritzat pel model d'itineraris
- es vol una base estructurada per controlar autenticació, persistència, validació i publicació d'API
- el domini triat del projecte base necessita un backend mantenible amb convencions clares
- l'equip pot defensar l'ús de `Laravel` com a stack real i no només com a generador d'esquelets

No té sentit usar-lo si:

- l'equip no entén el recorregut bàsic entre ruta, controlador, model, validació i base de dades
- es delega tota la comprensió al framework o a la IA
- el projecte només es pot explicar per màgia de plantilla i no per decisions pròpies

### Estructura mínima del projecte

Per al curs, un projecte `Laravel` usable hauria de tindre com a mínim:

- arrencada funcional de l'aplicació
- configuració clara de `.env` i connexió de base de dades
- rutes web o API separades segons el tipus de lliurable
- almenys un controlador o equivalent per al cas d'ús principal
- models del domini mínimament recognoscibles
- migracions per a usuaris i entitat principal del domini
- capa de validació mínima amb `Form Request` o validació equivalent en controlador
- proves mínimes o verificacions equivalents per als fluxos crítics

Estructura orientativa:

- `routes/web.php` o `routes/api.php`
- `app/Http/Controllers/`
- `app/Models/`
- `app/Http/Requests/` si s'usa validació desacoblada
- `database/migrations/`
- `tests/Feature/` i, quan tinga sentit, `tests/Unit/`

### Peces clau que cal entendre

L'equip hauria de saber per a què servixen, com a mínim:

- `routes/web.php` i `routes/api.php`: punt d'entrada del contracte d'exposició
- `app/Http/Controllers/`: coordinació de peticions i resposta
- `app/Models/`: representació del model i relacions bàsiques
- `database/migrations/`: evolució controlada de l'esquema
- `.env`: configuració de base de dades, aplicació i serveis
- `config/`: paràmetres del framework quan afecten execució o integració
- `tests/`: comprovacions reproduïbles del comportament crític

Criteri docent:

- no cal dominar totes les capes avançades de `Laravel`
- sí que cal entendre el recorregut mínim des de petició fins a persistència i resposta
- qualsevol peça generada automàticament ha de ser explicable i revisable

### Criteri propi de l'itinerari Laravel

Convé aprofitar les convencions fortes de `Laravel` quan realment ajuden al projecte:

- `Controller` com a punt d'entrada recognoscible
- `Model` i `Eloquent` com a capa persistent del domini
- `Form Request` quan aporte claredat en validació
- `migrations` i relacions per controlar evolució de l'esquema
- `middleware` per aplicar autenticació i control d'accés sense barrejar-ho tot al controlador

Criteri comú:

- no s'ha d'acceptar scaffolding només perquè existeix
- cal entendre quines parts són infraestructura del framework i quines parts són decisions pròpies del projecte
- la base ha de quedar preparada per continuar cap a persistència, API i integració sense reescriptura crítica

### Evidències mínimes

S'espera trobar evidències com:

- projecte que arranca localment amb instruccions reproduïbles
- `README` actualitzat amb posada en marxa, dependències i comandaments mínims
- commits que mostren l'arrancada real del projecte i no una pujada opaca final
- estructura mínima recognoscible de rutes, controlador, model i migracions
- almenys una verificació funcional del flux inicial
- AI log si la IA ha ajudat a triar comandaments, configuració o organització inicial

## Errors habituals d'arrancada

- arrancar un projecte `Laravel` però no entendre quines peces s'estan generant
- barrejar rutes web i API sense criteri
- deixar la configuració de base de dades només "aparentment" preparada
- treballar sobre un esquelet per defecte sense adaptar-lo al domini del curs
- no distingir què és infraestructura del framework i què és lògica pròpia del projecte
- acceptar comandaments o configuracions suggerides per IA sense provar-les realment al repositori

## Checklist final

- el projecte `Laravel` arranca i es pot reproduir amb instruccions clares
- l'estructura mínima del projecte està adaptada al domini del curs
- l'equip entén rutes, controladors, models, migracions i configuració bàsica
- l'ús de convencions pròpies de `Laravel` està justificat i és defensable
- hi ha evidències reals d'arrancada i de primera verificació
- la base queda preparada per connectar-se amb autenticació, persistència i API en els reptes següents
