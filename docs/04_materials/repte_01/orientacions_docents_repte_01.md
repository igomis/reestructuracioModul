# Orientacions docents del Repte 1

## Finalitat del document

Esta guia reunix els missatges docents que convé remarcar durant `R1` perquè el grup entenga què s'està construint i què no s'hauria de perdre en el repte.

## Marc temporal que convé fer explícit

- `R1` manté `4` microreptes com a passos lògics.
- La proposta base d'aula és de `6` hores: `2` sessions principals de `3` hores.
- La defensa i la revisió forta d'evidències formen part del tancament de `R1M2`.
- Els microreptes no equivalen necessàriament a sessions separades.

## Missatges clau que convé repetir en aula

- `R1` obri el projecte. No és una pràctica solta ni una excusa per instal·lar eines.
- Client i servidor no fan el mateix. El navegador mostra una part del flux, però és el backend qui rep, tracta i respon.
- Encara no toca un framework complet. Primer convé entendre el flux base i fer-lo visible sobre la base comuna en `PHP`.
- La tria de stack en `R1M1` és una decisió orientativa per arrancar `R1M2`, no una elecció definitiva del framework de tot el curs.
- Si apareixen `Laravel`, `Symfony` o `NestJS`, han d'aparéixer com a opcions comparades o com a futur camí de `R3`, no com a instal·lació obligatòria en `R1`.
- La seqüència del repte és curta i tancada: model client/servidor, entorn executable, landing inicial servida pel backend i checkpoint.
- Entorn executable vol dir que el projecte arranca de veritat, es pot provar i una altra persona pot reproduir els passos bàsics.
- El `README` forma part del producte del repte. Si no explica què has posat en marxa i com provar-ho, el repte està incomplet.
- Les fitxes i documents del repte han de quedar dins del repositori, en un directori de documentació enllaçat des d'un índex o pàgina visible.
- Una primera entrada visible no és una maqueta oberta com a fitxer ni un `hello world`. Ha de tindre relació amb el domini, estar servida pel backend i deixar veure cap a on evolucionarà el producte.
- La IA pot ajudar a explorar, revisar o proposar codi, però no pot substituir la comprensió ni la defensa del flux construït.

## Explicacions que convé fer visibles en directe

- mostrar amb un exemple del propi projecte on acaba el client i on comença el servidor
- modelar una decisió de stack acceptable: base `Docker + PHP + servidor web` per a `R1S2`, alternativa descartada i dubte pendent per a `R3`
- explicar què aixeca `Docker`, què executa `PHP` i què fa el servidor web
- ensenyar la landing inicial servida pel backend i la seua resposta inicial
- remarcar que un `healthcheck` és una comprovació tècnica, no l'entrega principal de `R1M2`
- remarcar com el `README` ha de permetre repetir l'arrencada i la prova
- fer visible què haurà d'estar preparat al checkpoint `R1 -> R2`

## Quan convé tallar una deriva

- si el grup dedica massa temps a comparar frameworks i encara no pot arrancar el projecte
- si la decisió de stack es converteix en debat de preferències i no en una decisió vinculada al producte i a `R1S2`
- si algú vol començar directament amb un framework complet però no sap explicar què farà el servidor en la primera acció útil
- si hi ha una pantalla o maqueta, però el backend encara no respon amb una peça funcional real
- si només hi ha `/health` o un endpoint d'estat però no hi ha landing inicial del producte
- si s'obrin dos o tres fluxos alhora i no n'hi ha cap de tancat
- si el `README` i la traçabilitat continuen buits perquè “ja es faran després”
- si s'està usant IA per generar peces que ningú del grup sap explicar

## Preguntes curtes de control per a classe o checkpoint

- On acaba el client i on comença el servidor en el teu producte?
- Per què esta base tècnica és assumible per al curs?
- Què faràs realment en `R1S2` i què queda ajornat fins a `R3`?
- Quina alternativa has descartat i quin motiu tècnic tens?
- Què aixeca `Docker`, què executa `PHP` i què aporta el servidor web?
- Quina landing inicial del producte ja pots ensenyar?
- Com saps que la landing està servida pel backend i no oberta com a fitxer estàtic?
- Com arranca el projecte una altra persona només amb el `README`?
- On està la documentació del repte dins del repositori i com s'hi arriba?
- Quin serà el primer flux que voldràs protegir després en `R2`?

## Què s'ha de poder defendre al final de `R1`

- quin producte s'està començant i per què s'ha triat eixe domini
- quina decisió tècnica inicial s'ha pres, quina alternativa s'ha descartat i quin dubte queda obert
- com arranca el projecte i què necessita una altra persona per provar-lo
- quina landing inicial servida pel backend ja funciona
- quin paper juguen `Docker`, `PHP` i el servidor web en l'arrencada
- com està documentada la base tècnica del repte dins del repositori
- què ha ajudat a resoldre la IA, si s'ha usada, i com s'ha verificat

## Criteri docent de tancament

Si el grup encara només pot ensenyar infraestructura, encara no ha tancat `R1`. Si pot ensenyar una decisió tècnica guiada, un entorn executable, una landing inicial servida pel backend, un `README` que permet repetir la prova i documentació del repte localitzable dins del repositori, el repte ja queda ben encarat per passar a `R2`.

La decisió tècnica guiada ha de ser prou concreta per arrancar `R1S2` i prou honesta per no prometre un framework complet abans d'hora. El professorat ha de valorar millor una decisió curta, assumible i comprovable que una comparativa llarga que no deixe clar què es farà en la sessió següent.
