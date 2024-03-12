# Besoins en surfaces agricoles pour la restauration collective

**Indicateurs :**
- Nombre de personnes et nombre de repas en restauration collective (scolaire et hospitalière)
- Besoins en matière première agricole pour la restauration collective
- Besoins en surfaces agricoles associées

## Bases de données
- Besoins en matière première et surfaces agricoles par personne (Parcel)
- [Effectifs des établissements scolaires](https://outil-sources-interne.basic.coop/#/publication/414/ministere-de-leducation-nationale-effectifs-des-etablissements-scolaires)
- [Effectifs étudiants](https://outil-sources-interne.basic.coop/#/publication/417/ministere-de-lenseignement-superieur-de-la-recherche-et-de-linnovation-effectifs-detudiants-dans-le-superieur)
- Proportion d'élèves en demi pension (Basic)
- [Places en EHPAD (Finess)](https://outil-sources-interne.basic.coop/#/publication/416/ministere-des-solidarites-et-de-la-sante-nombre-de-places-dans-les-etablissements-dhebergement-pour-personnes-agees-finess)


## Calcul
1. Le nombre de personnes est simplement la somme des bases de données d'effectifs scolaires, étudiants, Ehpad, hôpitaux.
2. Le nombre de repas à servir résulte de la multiplication avec un nombre de repas par jour qui dépend du type d'établissement :
   - Scolaires : 1 repas par jour multiplié par la proportion de demi pensionnaires
   - Ehpad : 3 repas par jour
   - Hôpitaux : le nombre de repas est imputé de la base Finess qui fourni le nombre de nuit d'hébergement (minoré à 0.5 quand il vaut zéro, on considère qu'il y a quand même demi-pension)
3. Besoin pour la restauration collective du territoire en matière première agricole = Repas par jour calculés précédemment * Nombre de jour par an par institution * Besoin en matière première agricole par personne par jour (Parcel)

    |Établissement|Jours d'ouverture par an|
    |-------|-------|
    |Maternelle (déjeuner)  |180|
    |Primaire (déjeuner)  |180|
    |Collège (déjeuner) |180|
    |Lycée (déjeuner) |170|
    |Université (déjeuner)  |170|
    |Maison de retraite (tous repas)  |365|
    |Hôpitaux (tous repas)  |365|

4. Besoin en surfaces agricoles = Besoin du territoire en surfaces agricole (Parcel) * Besoin pour la restauration collective en matière première agricole / Besoin du territoire en matière première agricole


## Limites
- Ces estimations de conso sont faites à partir de ratios d'autres estimations non spécifiques à la restauration collective (et pas non plus spécifiques à la restauration)
- Du plus fiable au moins fiable :
  - **Nombre de convives en restauration scolaire :** fiable, proche des données brutes
  - **Nombre de repas par jour :** dépend d'une hypothèse échelle nationale sur la proportion de demi-pensionnaires ainsi que du nombre de repas par jour en hôpitaux
  - **Besoin en matière première agricole pour la restauration collective du territoire :** en plus des hypothèses ci-dessus, ce besoin est issu de la modélisation Parcel qui estime les besoins alimentaires à partir des bilans d'approvisionnement échelle France. Cette moyenne Française peut s'éloigner des habitudes alimentaires et du niveau de gaspillage local, même si on prend en compte l'âge des convives qui est la principale variable expliquant les besoins alimentaires.
  - **Besoins en surfaces :** à peu près aussi fiable que ci-dessus. Garder en tête que seuls les produits Parcel sont pris en compte (donc excluant tous les produits tropicaux, l'huile d'olive l'alcool)

## Implémentation

https://github.com/lebasic/outil-analyse-durabilite/tree/master/modele_tat/CONSOMMATION