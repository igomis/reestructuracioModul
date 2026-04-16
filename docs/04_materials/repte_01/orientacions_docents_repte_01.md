# Orientacions docents del Repte 1

## Finalitat del document

Esta guia reunix els missatges docents que convé remarcar durant `R1` perquè el grup entenga què s'està construint i què no s'hauria de perdre en el repte.

## Marc temporal que convé fer explícit

- `R1` està calibrat com a proposta base de `12` hores.
- Això equival a `4` sessions de `3` hores.
- Cada sessió es correspon amb un microrepte docent concret.

## Missatges clau que convé repetir en aula

- `R1` obri el projecte. No és una pràctica solta ni una excusa per instal·lar eines.
- Client i servidor no fan el mateix. El navegador mostra una part del flux, però és el backend qui rep, tracta i respon.
- Encara no toca un framework complet. Primer convé entendre el flux base i fer-lo visible sobre la base comuna en `PHP`.
- La seqüència del repte és curta i tancada: model client/servidor, entorn executable, primer punt d'entrada funcional i checkpoint.
- Entorn executable vol dir que el projecte arranca de veritat, es pot provar i una altra persona pot reproduir els passos bàsics.
- El `README` forma part del producte del repte. Si no explica què has posat en marxa i com provar-ho, el repte està incomplet.
- Una primera funcionalitat real no és una maqueta ni un `hello world`. Ha de tindre relació amb el domini i deixar veure una interacció útil.
- La IA pot ajudar a explorar, revisar o proposar codi, però no pot substituir la comprensió ni la defensa del flux construït.

## Explicacions que convé fer visibles en directe

- mostrar amb un exemple del propi projecte on acaba el client i on comença el servidor
- explicar què aixeca `Docker`, què executa `PHP` i què fa el servidor web
- ensenyar el punt d'entrada del backend i la seua resposta inicial
- remarcar com el `README` ha de permetre repetir l'arrencada i la prova
- fer visible què haurà d'estar preparat al checkpoint `R1 -> R2`

## Quan convé tallar una deriva

- si el grup dedica massa temps a comparar frameworks i encara no pot arrancar el projecte
- si hi ha una pantalla o maqueta, però el backend encara no respon amb una peça funcional real
- si s'obrin dos o tres fluxos alhora i no n'hi ha cap de tancat
- si el `README` i la traçabilitat continuen buits perquè “ja es faran després”
- si s'està usant IA per generar peces que ningú del grup sap explicar

## Preguntes curtes de control per a classe o checkpoint

- On acaba el client i on comença el servidor en el teu producte?
- Per què esta base tècnica és assumible per al curs?
- Què aixeca `Docker`, què executa `PHP` i què aporta el servidor web?
- Quin és el primer punt d'entrada funcional que ja pots ensenyar?
- Com arranca el projecte una altra persona només amb el `README`?
- Quin serà el primer flux que voldràs protegir després en `R2`?

## Què s'ha de poder defendre al final de `R1`

- quin producte s'està començant i per què s'ha triat eixe domini
- com arranca el projecte i què necessita una altra persona per provar-lo
- quin és el primer punt d'entrada funcional que ja funciona
- quin paper juguen `Docker`, `PHP` i el servidor web en l'arrencada
- com està documentada la base tècnica del repte
- què ha ajudat a resoldre la IA, si s'ha usada, i com s'ha verificat

## Criteri docent de tancament

Si el grup encara només pot ensenyar infraestructura, encara no ha tancat `R1`. Si pot ensenyar una decisió tècnica guiada, un entorn executable, un primer punt d'entrada funcional del backend i un `README` que permet repetir la prova, el repte ja queda ben encarat per passar a `R2`.
