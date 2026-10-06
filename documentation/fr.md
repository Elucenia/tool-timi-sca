<!-- ELUCENIA technical documentation · timi-sca · fr · no clinical/professional/rights approval -->

# Score TIMI (SCA sans sus-décalage ST)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/timi-sca)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Âge ≥ 65 ans

`idade`

### ≥ 3 facteurs de risque de coronaropathie

`fr`

### Sténose coronaire connue ≥ 50 %

`dac`

### Prise d’aspirine au cours des 7 derniers jours

`aas`

### ≥ 2 épisodes d’angor en 24 heures

`angina`

### Déviation du ST ≥ 0,5 mm

`st`

### Marqueur de nécrose élevé

`marc`

## Édition de la méthode

TIMI UA/NSTEMI/Antman 2000 : 7 facteurs 0–1, total 0–7 ; sans TIMI STEMI

## Formule documentée

Un point par item présent (total de 0 à 7).

## Limites et population

Cette version du TIMI a été développée pour l’angor instable et l’infarctus sans sus-décalage ST, avec des critères composites à 14 jours ; ce n’est pas la version TIMI pour le STEMI. Les facteurs ont des définitions temporelles et cliniques précises. Les taux des essais historiques ne déterminent pas le risque individuel ou le traitement actuel sans évaluation et recommandation correspondantes.

## Références

- [Antman EM et al. The TIMI risk score for unstable angina/non–ST elevation MI. JAMA, 2000.](https://doi.org/10.1001/jama.284.7.835)

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

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Bénéfice d'une stratégie invasive précoce

| Détails du résultat | |
| --- | --- |
| Décès, IDM ou revascularisation urgente dans les 14 jours | 13,2% |


### 2

Bénéfice d'une stratégie invasive précoce

| Détails du résultat | |
| --- | --- |
| Décès, IDM ou revascularisation urgente dans les 14 jours | 26,2% |


### 3

Risque faible

| Détails du résultat | |
| --- | --- |
| Décès, IDM ou revascularisation urgente dans les 14 jours | 4,7% |

