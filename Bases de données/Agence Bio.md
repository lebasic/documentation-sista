# Recensement Parcellaire Graphique

- **Indicateur** : surface agricole bio par type de culture, tailles de cheptel et noms d'opérateurs
- **Échelle géographique** : communes depuis 2019, départements avant
- **Fréquence d'actualisation** : annuelle
- [**Lien Data Gouv**](https://www.data.gouv.fr/fr/organizations/agence-bio/)

## Méthode de collecte des données

Ces données de nombre d'opérateurs, surfaces et de cheptels sont issues des contrôles annuels que les organismes certificateurs agréés, réalisent dans les fermes et les entreprises de transformation, distribution engagées en bio.

### Précision géographique

Les données sont agrégées à l'échelle communale : code insee de la commune du site d'activité ou à défaut du siège d'exploitation.

## Surfaces

### Nomenclatures

L'agence bio donne la nature des cultures des parcelles dans une nomenclature 8 postes:

1. AU : Autres dont (jachères, engrais verts, fleurs, champignons etc…)\*
1. SF : Cultures Fourragères (dont prairies permanentes et temporaires, mais fourragers autres cultures fourragères, parcours ...)
1. FR : Fruits (arboriculture dont fruits à coques, fruits frais et fruis de transformation)
1. GCU : Grandes cultures (y compris légumes secs)
1. LE : Légumes frais (maraichage sous serre ou de pein champ (dont pomme de terre)
1. PP : PPAM
1. VI : Viticulture (dont 4% de raisin de table au niveau national)
1. HSAU : Hors surface agricole utilisée : les surfaces d'estives collectives, de cueillette sauvage, de bois, de marais... ne sont pas prises en compte

### Indicateurs

Ce jeu de données nous permet de calculer les indicateurs suivants :

- Surface totale en bio ou conversion
- Nombre d'exploitations par produit et par statut (bio ou conversion)

## Cheptels

### Nomenclatures

Une nomenclature 16 postes:

1. VA : Vaches allaitantes
1. VL : Vaches laitières
1. PO : Poules pondeuses
1. PC : Poulets de chair
1. AUVOL : Autres volailles de chair
1. BL : Brebis lait
1. BV : Brebis viande
1. CH : Chèvres
1. CO : Porcs charcutiers mis en place dans l'année
1. TR : Truies reproductrices
1. AQ : Aquaculture
1. LAR : Lapines
1. LA : Lapins
1. AUPA : Autre production animale (cervidés, escargots…)
1. API : Apiculture : en nombre de Ruches
1. HCHEP : Hors cheptel, nombre d'animaux présents sur la ferme au moment du contrôle, à n'utiliser qu'en termes de présence/absence.

La nomenclature serait à affiner notamment pour voir comment la joindre avec les données SAA et RGA

### Indicateurs

Pour l'instant peu d'indicateurs sont calculés à partir de ces données...

## Opérateurs

### Nomenclatures

Nombre d'opérateurs par commune, ou à défaut par code postal. Tous les opérateurs sont localisés par leur code postal, la quasi totalité par la commune de leur siège social.

Une nomenclature assez simple est utilisée :
P : producteurs (yc les producteurs ayant une autre activité : transformation à la ferme, magasin de la ferme...)
T : transformateurs ou restaurants (yc les transformateurs ayant une autre activité : transformateurs-distributeurs ou transformateurs-importateurs)
D : distributeurs (yc les distributeurs ayant une activité d'importation : distributeurs-importateurs...)
I : importateurs

## Utilisations dans les modélisations BASIC

Les données Agence Bio sont utilisées dans les modélisations BASIC pour :

- PARCEL essentiellement pour les surfaces et les calculs de rendements
