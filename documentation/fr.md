<!-- ELUCENIA technical documentation · abcd2 · fr · no clinical/professional/rights approval -->

# Score ABCD²

[conditions, sources et autorisations](https://elucenia.org/fr/outils/abcd2)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Âge ≥ 60 ans

`idade`

### Pression artérielle ≥ 140/90 mmHg à la première évaluation

`pa`

### Manifestation clinique

`clinica`

- `0` — Autres symptômes
- `1` — Trouble de la parole sans faiblesse
- `2` — Faiblesse unilatérale

### Durée des symptômes

`duracao`

- `0` — \< 10 min
- `1` — 10 à 59 min
- `2` — ≥ 60 min

### Diabète

`dm`

## Édition de la méthode

ABCD²/Johnston 2007 : âge/tension/clinique/durée/diabète, total 0–7

## Formule documentée

A âge ≥60 : 1 · B tension ≥140/90 : 1 · C clinique : faiblesse unilatérale 2, parole sans faiblesse 1 · D durée : ≥60 min 2, 10 à 59 min 1 · Diabète 1. Total 0 à 7.

## Limites et population

Score pronostique après un diagnostic d’AIT, étudié principalement pour le risque d’AVC à 2 jours, avec des analyses supplémentaires à 7 et 90 jours. Il ne confirme pas le diagnostic d’AIT. Les probabilités observées dans les cohortes originales ne représentent pas une prédiction individuelle universelle.

## Références

- [Johnston SC et al. Validation and refinement of scores to predict very early stroke risk after transient ischaemic attack. Lancet, 2007.](https://doi.org/10.1016/S0140-6736(07)60150-0)

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
