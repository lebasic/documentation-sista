# Potentiel agro-industriel

Question de recherche :

**Est-ce qu'il y a sur le territoire étudié les industries de transformation agro-alimentaires nécessaires pour transformer les matières agricoles nécessaires pour nourrir sa population ?**

## Bases de données
- **Prodcom** : production en volume à l'échelle France
- **Esane** : emplois IAA échelle France
- **Sirene** : emplois IAA modélisés à l'échelle communale
- **Parcel** : besoin alimentaires en équivalent matière première
- **Basic** : proportion d'aliments transformés dans la consommation humaine


## Calcul
On commence par calculer une intensité en emploi par secteur d'activité :

**Intensité en emploi = Emploi (Esane) / Production (Prodcom) / Coefficient équivalent matière première (Basic)**

L'unité est en ETP par kg équivalent matière première.

On multiplie ensuite cette intensité en emploi par les besoins de la population avec la formule suivante :

**Besoin agro-industriel = Besoin alimentaire en equivalent matière première (Parcel) * Proportion d'aliments consommés transformés (Basic) * Intensité en emploi (Basic)** en ETP pour le territoire, par catégorie de produit

On compare ensuite ce besoin en ETP agro-industriels aux ETP présents sur le territoire, modélisés à partir de la base Sirene.

## Nomenclatures
Une nomenclature spéciale permettant le regroupement par secteur industriel a été créée pour cette modélisation : https://outil-sources-interne.basic.coop/#/table/acteurs.potentiel_agroindustriel

## Limites
# /!\ Attention
Le coefficient *proportion d'aliments transformés dans la consommation humaine* stocké dans la table *proportion_consommation_transformee* semble contenir quelque chose d'un peu différent. À analyser de plus près.

## Implémentation
La modélisation est implémentée dans ce fichier : https://github.com/lebasic/outil-analyse-durabilite/blob/master/modele_tat/DURABILITE/Potentiel%20agro-industriel.sql