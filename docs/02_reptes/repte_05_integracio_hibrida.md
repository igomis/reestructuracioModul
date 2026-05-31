# Repte 5. Aplicació web híbrida i integració de serveis externs

## Fitxa canònica del repte

- **Funció didàctica principal**: síntesi amb nucli mínim obligatori de `RA9` i ampliació avançada opcional.
- **Objectiu**: integrar fonts o serveis externs dins del projecte base per generar una funcionalitat híbrida amb valor real.
- **Producte esperat**: integració funcional amb consum extern, transformació de dades, tractament mínim d'errors i documentació tècnica.
- **Evidències**: demo del flux complet, proves o verificacions d'integració, documentació tècnica, mapping de dades, comparativa font externa / transformació / resultat final i traçabilitat de treball.
- **Paper de la IA**: ús assistit per IA permés per explorar fonts, connectors o transformacions; els límits i la delegació excessiva depenen de [us-ia-professorat-i-alumnat.md](../us-ia-professorat-i-alumnat.md).
- **Relació amb el projecte base**: obri el projecte base a l'exterior i tanca la seqüència de construcció abans de la defensa tècnica.
- **Checkpoint de control**: selecció justificada de la font externa abans de construir la integració i demo final amb cas positiu, cas d'error, contrast del mapa d'integració i mini defensa.
- **Instrument dominant**: checklist d'integració híbrida amb valor de producte.
- **Instrument de comprensió**: mini defensa tècnica sobre contracte extern, mapping i aportació real al producte.
- **Instrument de control de delegació excessiva**: revisió de commit rellevant comentat, contrast amb `AI log` i prova guiada sobre la transformació o l'orquestració.
- **Instrument de recuperació o millora**: reducció d'abast a una sola font externa, un cas d'ús híbrid i una nova demo completa.

## Justificació docent

- **Evidència principal**: flux híbrid complet amb font externa, transformació i valor observable dins del producte.
- **Evidències secundàries**: mapping de dades, prova d'error, documentació final, traçabilitat de treball i mini defensa.
- **Mínim suficient**: una connexió vistosa o un workflow aïllat no compta; cal integració útil, reproduïble i defensable.
- **Feedback previst**: validació de la font abans de construir i demo final amb cas positiu, fallada rellevant i defensa curta.

## 1. Visió general del repte

**Finalitat del repte**

Construir una funcionalitat híbrida del projecte que combine recursos propis amb serveis, dades o codi de tercers per generar valor nou i útil dins del producte.

Este repte no s’entén com una simple connexió a una API externa ni com una demostració superficial de consum de dades alienes. El seu sentit és integrar informació o serveis heterogenis de manera crítica, transformada i documentada, perquè el sistema faça alguna cosa nova que abans no podia fer.

**Producte principal del repte**

Una funcionalitat híbrid integrada en el projecte, amb:

- consum real d’una o més fonts externes
- tractament o transformació de la informació rebuda
- combinació amb dades o serveis propis del projecte quan siga pertinent
- generació d’una funcionalitat nova amb valor real
- tractament mínim d’errors i incidències d’integració
- proves mínimes o verificacions registrades
- documentació tècnica de la integració

**Context professional simul·lat o realista**

L’equip ja disposa d’un backend funcional, estructurat i capaç d’exposar serveis propis.

Ara ha de demostrar una competència molt habitual en entorns professionals: reutilitzar serveis, fonts de dades o components externs per ampliar el valor del sistema sense reconstruir-ho tot des de zero.

**Relació amb el projecte global del curs**

Este repte reutilitza el sistema construït fins ara i l’obri a l’exterior.

En el Repte 4, el sistema aprenia a exposar serveis propis.

En el Repte 5, el sistema aprén a consumir, integrar, transformar i reaprofitar informació o serveis externs per generar una aplicació híbrida amb sentit.

***
