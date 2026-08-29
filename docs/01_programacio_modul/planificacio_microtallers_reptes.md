# Planificació de microtallers dins dels reptes

## Finalitat

Els microtallers són intervencions curtes dins de sessions de repte. No creen microreptes nous ni notes separades: reforcen punts tècnics que solen bloquejar l'alumnat i ajuden a convertir el repte en una evidència més defensable.

La duració no ha de ser sempre la mateixa. Si el taller només introdueix criteri o dona una pauta de revisió, pot ocupar `15-30` minuts. Si exigeix posar en marxa codi, proves, configuració o una decisió tècnica amb evidència al repositori, ha d'ocupar `35-60` minuts. `R3S2B` forma part de la programació base; `R2S10` és una sessió d'ampliació intermodular sense microrepte propi, i les altres variants opcionals només s'activen si aporten valor al projecte real.

## Criteris d'ús

- usar-los el dia en què el producte necessita eixa decisió o tècnica, no abans;
- reservar-los dins de la seqüència de la sessió de `3` hores, sense afegir hores noves al repte;
- mantindre'ls com a suport pràctic, no com a classe teòrica llarga;
- tancar cada microtaller amb una evidència menuda al repositori;
- vincular-los a defensa individual, procés i verificació;
- reduir-los a explicació de `15-20` minuts quan no cal posar res en funcionament;
- ampliar-los fins a `45-60` minuts quan hi ha codi, proves, configuració o revisió tècnica real.

## Mapa operatiu de temporalització

| Codi | Sessió i moment d'aula | Microtaller | Temps calibrat | Per què eixe temps | Teoria o material relacionat | Presentació | Evidència mínima |
|---|---|---|---:|---|---|---|---|
| `MT19` | `R1S0`, dins del bloc `1:20-2:00` | IA responsable aplicada al repte | `25 min` inicials + recordatoris de `10 min` abans de checkpoints | és criteri d'ús i verificació, no implementació tècnica | [Guia d'ús verificable de la IA](../04_materials/materials_comuns/guia_ús_verificable_ia.md) | [MT19](../07_presentacions/microtallers/mt19_ia_responsable_repte.md) | primera pauta d'AI log i criteri de defensa |
| `MT01` | `R1S1`, `0:35-1:10` | Projecte no CRUD | `35 min` | cal modelar domini i primer flux, però no desenvolupar encara | [Apunts R1](../04_materials/apunts_reals/repte_01_kickoff_backend.md) i [materials R1](../04_materials/repte_01/mapa_materials_repte_01.md) | [MT01](../07_presentacions/microtallers/mt01_projecte_no_crud.md) | domini amb actors, regles i primer flux |
| `MT02` | `R1S2`, `2:05-2:35` | README executable i commit defensable | `30 min` | revisió guiada de documentació i traçabilitat sobre treball ja fet | [Guia README i nota tècnica de decisió](../04_materials/materials_comuns/guia_readme_i_adr.md) i [Guia Git](../04_materials/materials_comuns/guia_git_i_flux_treball.md) | [MT02](../07_presentacions/microtallers/mt02_readme_commit_defensable.md) | instruccions d'arrancada i commit explicable |
| `MT03` | `R2S1`, `1:20-2:05`; reforç curt en `R2S2`, `0:00-0:10` | Validació de servidor amb casos roïns | `45 min` + `10 min` de represa | inclou taula de casos i primera prova manual; el reforç de `R2S2` evita repetir teoria | [Guia de validació i errors](../04_materials/repte_02/guia_validacio_i_errors_servidor.md) | [MT03](../07_presentacions/microtallers/mt03_validacio_servidor_casos_roins.md) | casos vàlids/invàlids i prova reproduïble |
| `MT04` | `R2S4`, `0:35-1:10` | Sessió, cookies i estat | `35 min` | combina explicació curta i decisió aplicada al flux propi | [Guia de flux d'usuari i sessions](../04_materials/repte_02/guia_flux_usuari_i_sessions.md) | [MT04](../07_presentacions/microtallers/mt04_sessions_cookies_estat.md) | decisió sobre què es guarda i on |
| `MT05` | `R2S5`, `0:30-1:20`; represa en `R2S6`, `0:00-0:10` | Auth mínima defensable | `50 min` + `10 min` de represa | cal implementar o revisar cas permés, cas denegat i frontera de control | [Apunts R2](../04_materials/apunts_reals/repte_02_sessions_i_autenticacio.md) | [MT05](../07_presentacions/microtallers/mt05_auth_minima_defensable.md) | cas permés, cas denegat i explicació del control |
| `MT06` | `R2S7`, `0:25-1:00` | Debugging i prova curta | `35 min` | és pràctic, però acotat a una prova reproduïble i un error controlat | [Guia testing i debugging](../04_materials/materials_comuns/guia_testing_i_debugging.md) | [MT06](../07_presentacions/microtallers/mt06_debugging_prova_curta.md) | prova reproduïble abans de dir que funciona |
| `MT07` | `R3S1`, `0:45-1:25` | Migrar un cas d'ús a framework | `40 min` | cal fer mapa de migració abans de tocar massa codi nou | [Apunts R3](../04_materials/apunts_reals/repte_03_mvc_i_persistencia.md) i itinerari triat | [MT07](../07_presentacions/microtallers/mt07_migrar_cas_us_framework.md) | mapa entre flux antic i flux en framework |
| `MT08` | `R3S2`, `0:30-1:20` | Migracions, seeders i dades de prova | `50 min` | implica executar migracions o equivalent i deixar dades inicials reproduïbles | [Guia de persistència i modelat](../04_materials/repte_03/guia_persistencia_i_modelat_dades.md) i itinerari triat | [MT08](../07_presentacions/microtallers/mt08_migracions_seeders_dades_prova.md) | projecte arrancable amb dades inicials |
| `MT16` | `R3S2B`, sessió completa entre `R3S2` i `R3S3` | Portabilitat entre frameworks | `3h` | és auditoria comparativa obligatòria per assegurar que l'alumnat entén equivalències entre stacks abans del primer flux fort | [Model d'itineraris tecnològics](model_itineraris_tecnologics.md) i itineraris | [MT16](../07_presentacions/microtallers/mt16_portabilitat_frameworks.md) | taula d'equivalències i decisió de portabilitat |
| `MT09` | `R3S3`, `0:30-1:05`; reforç curt en `R3S4`, `0:00-0:10` | On pose la lògica | `35 min` + `10 min` de represa | és decisió arquitectònica aplicada a un flux, no classe llarga de patrons | [Guia de refactorització MVC o equivalent](../04_materials/repte_03/guia_refactoritzacio_mvc_o_equivalent.md) | [MT09](../07_presentacions/microtallers/mt09_on_pose_la_logica.md) | decisió controller/service/model documentada |
| `MT10` | `R4S1`, `0:30-1:05` | Dissenyar endpoint abans de programar | `35 min` | és disseny de contracte; el temps fort queda per implementar després | [Guia de contracte i disseny API](../04_materials/repte_04/guia_contracte_i_disseny_api.md) i [Apunts R4](../04_materials/apunts_reals/repte_04_api_i_consum.md) | [MT10](../07_presentacions/microtallers/mt10_dissenyar_endpoint_abans_programar.md) | contracte d'endpoint abans del codi |
| `MT11` | `R4S5`, `0:35-1:20` | Provar i documentar una API | `45 min` | cal executar peticions, contrastar errors i ajustar documentació | [Guia de proves i documentació API](../04_materials/repte_04/guia_proves_i_documentacio_api.md) | [MT11](../07_presentacions/microtallers/mt11_provar_documentar_api.md) | peticions reproduïbles i documentació alineada |
| `MT17` | `R4S6` o, si no hi ha sessió extra, `R4S3`, `2:00-3:00` | Tokens funcionals del backend | `60 min` opcional | només té sentit si es dissenya i es prova un flux tokenitzat real | [Guia de contracte i disseny API](../04_materials/repte_04/guia_contracte_i_disseny_api.md) | [MT17](../07_presentacions/microtallers/mt17_tokens_funcionals_backend.md) | cicle de vida del token i cas autoritzat/denegat |
| `MT12` | `R5S1`, `0:30-1:00` | Triar una integració amb valor | `30 min` | és decisió de producte i frontera entre sistemes, sense codi encara | [Guia d'integració externa i flux híbrid](../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md) i [Apunts R5](../04_materials/apunts_reals/repte_05_integracio_hibrida.md) | [MT12](../07_presentacions/microtallers/mt12_integracio_amb_valor.md) | mapa de valor i frontera entre sistemes |
| `MT13` | `R5S2`, `0:25-1:00` | Secrets, `.env` i claus | `35 min` | inclou criteri de seguretat i revisió real de configuració | [Guia d'integració externa i flux híbrid](../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md) | [MT13](../07_presentacions/microtallers/mt13_secrets_env_claus.md) | configuració segura sense secrets al repo |
| `MT14` | `R5S3`, `0:35-1:20` | Mapping de resposta externa | `45 min` | cal transformar una resposta externa en model propi i comprovar-la | [Guia d'integració externa i flux híbrid](../04_materials/repte_05/guia_integracio_externa_i_flux_hibrid.md) | [MT14](../07_presentacions/microtallers/mt14_mapping_resposta_externa.md) | transformació de dades externa a model propi |
| `MT15` | `R5S5`, `0:25-1:00` | Defensa tècnica curta | `35 min` | prepara defensa i pregunta crítica sense llevar temps al tancament tècnic | [Guió de defensa individual](../08_materials_compartibles/guio_defensa_individual_breu.md) i [guió de tancament](../08_materials_compartibles/guio_tancament_producte_i_defensa_final.md) | [MT15](../07_presentacions/microtallers/mt15_defensa_tecnica_curta.md) | guió de defensa i pregunta crítica preparada |
| `MT18` | `R5S6` o, si no hi ha sessió extra, `R5S4`, `2:10-3:00` | Actius digitals tokenitzats | `50 min` opcional | és ampliació conceptual aplicada; només requereix més temps si es prototipa | [Guia d'orquestració i automatització](../04_materials/repte_05/guia_orquestracio_i_automatitzacio.md) | [MT18](../07_presentacions/microtallers/mt18_actius_digitals_tokenitzats.md) | decisió justificada sobre si tokenitzar aporta valor |

## Microtallers opcionals o d'ampliació

| Codi | Moment preferent | Quan activar-lo | Com encaixar-lo sense desquadrar |
|---|---|---|---|
| `R2S10` | després de `R2S6` | si cal deixar la mini API d'autenticació preparada per al consum de `DWEC` | sessió completa d'ampliació intermodular, sense microrepte propi |
| `MT17` | després de definir protecció d'API en `R4S3` | si el projecte necessita confirmació, invitació, accés puntual o traçabilitat | `60 min` dins de `R4S3` o sessió ampliada `R4S6` si es prototipa |
| `MT18` | després de tindre integració funcional en `R5S4` | si el grup pot treballar ampliació avançada sense especulació | `50 min` dins de `R5S4` o sessió ampliada `R5S6` si es prototipa |
| `MT19` | `R1S0` i abans de checkpoints | quan aparega delegació excessiva en IA o evidències poc defensables | `25 min` inicials i recordatoris de `10 min`, sense sessió nova |

## Ordre recomanat

No cal fer-los tots. La seqüència mínima recomanada és:

1. `MT01`
2. `MT02`
3. `MT03`
4. `MT05`
5. `MT08`
6. `MT16`
7. `MT09`
8. `MT10`
9. `MT11`
10. `MT13`
11. `MT15`

## Presentacions associades

Les presentacions estan en `docs/07_presentacions/microtallers/` i seguixen el format de micro-presentació docent breu.

## Regla de tancament

Cada microtaller ha d'acabar amb una pregunta verificable:

> Què pots ensenyar ara en el repositori que no podies ensenyar abans del microtaller?
