<!-- ELUCENIA technical documentation · qsofa · fr · no clinical/professional/rights approval -->

# qSOFA (SOFA rapide)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/qsofa)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Fréquence respiratoire ≥ 22 respirations/min

`fr`

### Altération de l’état mental (Glasgow \< 15)

`mental`

### Pression systolique ≤ 100 mmHg

`pas`

## Édition de la méthode

qSOFA/Sepsis-3/Seymour 2016 : FR≥22/PAS≤100/altération mentale, 0–3 ; pas de dépistage isolé recommandé SSC 2021

## Formule documentée

Un point chacun : fréquence respiratoire ≥ 22/min, altération mentale et pression systolique ≤ 100 mmHg. Positif à 2 ou plus.

## Limites et population

qSOFA 2016 est un outil d’évaluation du risque chez les adultes ayant une suspicion d’infection, et non un diagnostic ni un test isolé permettant d’exclure un sepsis. Un score faible n’élimine pas la suspicion clinique. La SSC 2021 recommande de ne pas utiliser qSOFA comme seul outil de dépistage ; les recommandations officielles SSC 2026 continuent de privilégier d’autres outils pour le dépistage hospitalier. L’évaluation et le traitement d’urgence ne doivent pas attendre le score. Ce seuil adulte n’établit pas une application pédiatrique.

## Références

- [Seymour CW et al. Assessment of clinical criteria for sepsis: for the Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0288)

- [Singer M et al. The Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0287)

- [Evans L et al. Surviving sepsis campaign: international guidelines for management of sepsis and septic shock 2021. Intensive Care Med, 2021.](https://doi.org/10.1007/s00134-021-06506-y)

- [SSC adult guidelines2021](https://www.sccm.org/clinical-resources/guidelines/guidelines/surviving-sepsis-guidelines-2021)

- [SSC adult guidelines2026, current official page as observed2026-10-03](https://www.sccm.org/survivingsepsiscampaign/guidelines-and-resources/surviving-sepsis-campaign-adult-guidelines)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
