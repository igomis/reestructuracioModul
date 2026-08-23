# Full de treball del Repte 1

## Objectiu

Deixar obert el projecte amb una base executable i una landing inicial servida pel backend.

## Seqüència base

- `R1M1`: model client/servidor, model d'execució client vs servidor i decisió tècnica inicial orientativa
- `R1M2`: base executable amb Docker, PHP, servidor web, BBDD i phpMyAdmin, landing inicial servida pel backend, documentació tècnica, verificació i checkpoint

Cada microrepte equival a una sessió ordinària de `3` hores. `R1M1` té un pes del `25%` dins del repte i `R1M2` concentra el `75%` restant perquè tanca la base executable, la primera entrada visible del producte i el checkpoint de pas a `R2`.

## Has de fer

- explicar el paper del client i del servidor en el teu producte
- diferenciar què s'executa al client web i què s'executa al servidor
- omplir la [fitxa breu d'exploració tècnica inicial](fitxa_exploracio_tecnica_inicial.md) amb tecnologies identificades, opcions explorades i primera decisió orientativa
- justificar la base tècnica dins del marc del curs
- deixar repositori usable i `README` inicial
- arrancar l'entorn amb Docker, PHP i servidor web
- adaptar el model mínim del professorat al teu projecte
- completar l'entorn amb servei de base de dades i phpMyAdmin
- registrar una decisió tècnica menuda i una incidència, dubte o bloqueig real
- crear una landing inicial del producte servida pel backend, amb HTML i CSS senzill
- usar un `healthcheck` només com a comprovació tècnica auxiliar, si cal
- crear un directori de documentació dins del repositori
- penjar les fitxes o documents del repte al repositori
- crear un índex o pàgina visible que enllace eixa documentació
- preparar una verificació curta i explicable del que ja funciona

## Evidència mínima

- fitxa breu d'exploració tècnica inicial
- explicació del model d'execució client vs servidor aplicada al producte
- repositori obert i recognoscible
- `README` amb com arranca el projecte
- entorn executable amb `Docker`, `PHP`, servidor web, BBDD i phpMyAdmin
- explicació de què fa cada servei i què has adaptat respecte del model inicial
- decisió tècnica curta i incidència o dubte registrat
- landing inicial servida pel backend
- directori de documentació amb fitxes o documents del repte
- índex o pàgina que enllaça la documentació
- justificació tècnica breu i traçabilitat mínima

## Targeta fixa de traçabilitat

- **Criteri/objectiu**: `RA1`, arrencada backend executable i justificable.
- **Descriptor de rúbrica**: resolució funcional mínima, traçabilitat i documentació operativa.
- **Moment d'avaluació**: checkpoint de kickoff.
- **Agent d'avaluació**: professorat amb defensa breu de l'alumne.
- **Tipus d'evidència**: repositori, `README`, demo, fitxa i commit comentat.

## Com ho valides

- ensenya la fitxa i explica què has investigat, què has entés i amb què començaries
- explica quina part del teu producte s'executa al client i quina al servidor
- arranca el projecte davant del professorat
- mostra la landing inicial servida pel backend
- explica què fa `Docker`, què fa `PHP`, què fa el servidor web, què fa la base de dades i per a què uses phpMyAdmin
- explica què has adaptat respecte del model del professorat
- ensenya que el `README` permet repetir la prova
- mostra on està la documentació del repte dins del repositori i com s'hi arriba

## Errors habituals

- convertir la fitxa en un informe llarg o una comparativa eterna
- adjuntar captures de totes les converses amb IA com si això substituïra la fitxa
- quedar-se en l'esquelet del framework
- justificar tecnologia però no el producte
- no saber què fa cada component tècnic
- copiar una configuració completa sense adaptar-la ni comprovar-la
- no tindre cap landing inicial servida pel backend
- quedar-se només en un `healthcheck`
- no actualitzar el `README`

## Si et bloqueges

- reduïx el repte a una landing molt simple del producte
- simplifica l'entorn fins al mínim que realment arranca
- revisa la [consulta ràpida de PHP](../alumnat/consulta_tecnica/php_consulta_rapida.md)
- torna a l'[apunt real de `R1`](../02_reptes/repte_01_kickoff_backend.md)

## Si acabes prompte

- deixa més clar el `README`
- millora l'onboarding tècnic
- reforça la landing amb una pàgina `Sobre el projecte` o una comprovació tècnica millor, sense obrir encara el flux complet de `R2`
