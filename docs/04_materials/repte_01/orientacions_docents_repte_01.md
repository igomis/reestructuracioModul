# Orientacions docents del Repte 1

## Finalitat del document

Esta guia reunix els missatges docents que convé remarcar durant `R1` perquè el grup entenga què s'està construint i què no s'hauria de perdre en el repte.

## Missatges clau que convé repetir en aula

- `R1` obri el projecte. No és una pràctica solta ni una excusa per instal·lar eines.
- Client i servidor no fan el mateix. El navegador mostra una part del flux, però és el backend qui rep, tracta i respon.
- Encara no toca un framework complet. Primer convé entendre el flux base i fer-lo visible sobre la base comuna en `PHP`.
- Entorn executable vol dir que el projecte arranca de veritat, es pot provar i una altra persona pot reproduir els passos bàsics.
- El `README` forma part del producte del repte. Si no explica què has posat en marxa i com provar-ho, el repte està incomplet.
- Una primera funcionalitat real no és una maqueta ni un `hello world`. Ha de tindre relació amb el domini i deixar veure una interacció útil.
- La IA pot ajudar a explorar, revisar o proposar codi, però no pot substituir la comprensió ni la defensa del flux construït.

## Explicacions que convé fer visibles en directe

- mostrar amb un exemple del propi projecte on acaba el client i on comença el servidor
- ensenyar el punt d'entrada del backend i la seua resposta inicial
- explicar com entra una dada al servidor i on es valida
- ensenyar què passa quan la dada és correcta i què passa quan no ho és
- remarcar on queda el primer rastre de la informació correcta

## Quan convé tallar una deriva

- si el grup dedica massa temps a comparar frameworks i encara no pot arrancar el projecte
- si hi ha pantalla o maqueta, però el servidor encara no rep cap dada real
- si s'obrin dos o tres fluxos alhora i no n'hi ha cap de tancat
- si el `README` i la traçabilitat continuen buits perquè “ja es faran després”
- si s'està usant IA per generar peces que ningú del grup sap explicar

## Preguntes curtes de control per a classe o checkpoint

- Quina és la primera dada útil que entra al teu producte?
- On es veu el tractament d'eixa dada en el servidor?
- Quina validació mínima has decidit aplicar i per què?
- Què veu la persona usuària quan la dada no és correcta?
- On queda registrada o guardada la dada correcta?
- Quin serà el primer flux que voldràs protegir després en `R2`?

## Què s'ha de poder defendre al final de `R1`

- quin producte s'està començant i per què s'ha triat eixe domini
- com arranca el projecte i què necessita una altra persona per provar-lo
- quin és el primer flux real que ja funciona
- què es valida i com es mostra l'error
- què es registra o persistix de manera mínima
- què ha ajudat a resoldre la IA, si s'ha usada, i com s'ha verificat

## Criteri docent de tancament

Si el grup encara només pot ensenyar infraestructura, encara no ha tancat `R1`. Si pot ensenyar una entrada funcional del producte, una dada tractada pel servidor, un error visible i un rastre bàsic de la dada correcta, el repte ja queda ben encarat per passar a `R2`.
