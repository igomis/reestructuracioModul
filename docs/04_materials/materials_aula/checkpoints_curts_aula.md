# Checkpoints curts d'aula

## Finalitat del document

Donar un format reusable per fer controls ràpids de `2-3` minuts sobre l'estat real d'un equip o d'un bloc de treball sense convertir cada revisió en una defensa completa.

## Quan convé usar esta peça

- a meitat de sessió per comprovar si el grup va pel bon camí
- al final d'un bloc curt abans de donar pas a autonomia
- en equips endarrerits que necessiten microvalidacions freqüents
- com a filtre ràpid abans d'un checkpoint formal

## Estructura reusable de checkpoint curt

- Què hauria d'estar fet:
- Com es verifica en `2-3` minuts:
- Senyal d'alerta:
- Acció correctiva ràpida:

## Plantilla base

```md
Què hauria d'estar fet
- A este punt, el grup hauria de poder ensenyar:

Com es verifica en 2-3 minuts
- Obri:
- Mostra:
- Executa:

Senyal d'alerta
- Si no poden ensenyar això, o només ho expliquen però no ho mostren:

Acció correctiva ràpida
- Abans de continuar, han de:
```

## Exemple per a `R1`

- Què hauria d'estar fet: landing page o equivalent, formulari i `README` mínim
- Com es verifica en `2-3` minuts: arrancar projecte, obrir vista inicial i enviar una dada simple
- Senyal d'alerta: només hi ha esquelet de framework o captura estàtica
- Acció correctiva ràpida: reduir a un sol formulari i deixar registre mínim abans de tocar res més

## Exemple per a `R3`

- Què hauria d'estar fet: una entitat persistent i un flux refactoritzat recognoscible
- Com es verifica en `2-3` minuts: mostrar model, punt d'entrada i prova curta del flux
- Senyal d'alerta: hi ha base de dades però el cas d'ús continua acoblat o fràgil
- Acció correctiva ràpida: congelar noves funcionalitats i tancar només el flux principal

## Exemple per a `R5`

- Què hauria d'estar fet: integració o workflow que resol una necessitat real del producte
- Com es verifica en `2-3` minuts: llançar el flux complet i mostrar entrada, eixida i control bàsic d'error
- Senyal d'alerta: hi ha automatització, però no es pot explicar quin valor aporta
- Acció correctiva ràpida: simplificar el workflow a un únic recorregut útil i documentar-lo
