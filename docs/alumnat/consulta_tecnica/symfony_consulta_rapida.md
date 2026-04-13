# Symfony: consulta ràpida

## Què és

És una guia curta per localitzar les peces de `Symfony` que més et fan falta en este curs. No substituïx la documentació oficial: t'ajuda a entendre com encaixa `Symfony` amb el teu projecte i amb els reptes del tram de framework.

## Quan la necessites en el curs

- a partir de `R3`, quan entra el contrast de frameworks
- en `R3`, per separar controladors, serveis, entitats i persistència
- en `R4`, per publicar una `API` mantinguda amb criteri
- en `R5`, per mantindre el mateix projecte en integració i tancament

## Què has de saber sí o sí

- `Controller` coordina la petició, però no ha de contindre tota la lògica
- `Entity`, `Repository` i `Service` han de tindre rols clars
- la configuració i les migracions formen part del projecte, no d'un apèndix
- seguretat, validació i persistència han d'estar alineades amb el flux real del domini

## Errors habituals

- confiar-ho tot a `maker` sense entendre què s'ha generat
- posar negoci dins del controlador
- tindre entitats o migracions que no reflectixen el flux real
- separar carpetes però no responsabilitats

## On ampliar

- Material del curs: [Guia de bootstrap Symfony](../../04_materials/itineraris/symfony/guia_bootstrap_symfony.md)
- Material del curs: [Guia d'auth i persistència Symfony](../../04_materials/itineraris/symfony/guia_auth_i_persistencia_symfony.md)
- Symfony Docs: [Controllers](https://symfony.com/doc/current/controller.html)
- Symfony Docs: [Security](https://symfony.com/doc/current/security.html)
- Symfony Docs: [Doctrine](https://symfony.com/doc/current/doctrine.html)
