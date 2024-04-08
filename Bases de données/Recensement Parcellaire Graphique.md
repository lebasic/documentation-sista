# Recensement Parcellaire Graphique

- **Indicateur** : surface agricole par type de culture (bio et non bio)
- **Échelle géographique** : parcelle agricole (agrégées en communes)
- **Fréquence d'actualisation** : annuelle
- [**Lien Data Gouv**](https://www.data.gouv.fr/fr/datasets/registre-parcellaire-graphique-rpg-contours-des-parcelles-et-ilots-culturaux-et-leur-groupe-de-cultures-majoritaire/)

## Jeux de données

2 jeux de données sont disponibles pour le RPG, l'ensemble des cultures et les cultures bio. Nous avons dans OAD toutes les données du RPG depuis 2010 alors que les données RPG Bio existent depuis 2019.

## Méthode de collecte des données

Chaque exploitant.e déclare chaque année quelle culture est effectuée sur ses parcelles, dans le but d'obtenir les subventions de la PAC. L'IGN effectue un pré-remplissage des formulaires de déclaration à l'aide d'image satellites.

## Nomenclatures

Le RPG donne la nature des cultures par parcelles dans deux nomenclatures :

- De 2010 à 2014 dans une [nomenclature à 28 postes](https://outil-sources-interne.basic.coop/#/table/filieres.rpg_bichiffre)
- À partir de 2015 dans une nomenclature beaucoup plus détaillée de [300 et quelques postes](https://outil-sources-interne.basic.coop/#/table/filieres.rpg_trilettre)

Au BASIC et notamment dans Sista on utilise plusieurs regroupements de ces surfaces :

- Une nomenclature [en 12 postes](https://outil-sources-interne.basic.coop/#/table/filieres.basic_agricole_2)

  1. Légumes
  2. Fruits
  3. Céréales
  4. Oléoagineux
  5. Protéagineux, légumineuses
  6. Pomme de terre
  7. Cultures fourragères
  8. Estives et landes
  9. Prairies
  10. Vignes
  11. Cultures industrielles
  12. Jachères & Gel
  13. Autres espaces agricoles

- [En 5 postes](https://outil-sources-interne.basic.coop/#/table/filieres.basic_agricole_1)
  1. Fruits & Légumes
  2. Cultures annuelles
  3. Prairies, estives, landes
  4. Vignes
  5. Jachères & autres espaces agricoles

Ces regroupements permettent de représenter de la même manière plusieurs sources de données sur les surfaces (Teruti) et des modélisation BASIC (Parcel)

### Surfaces peu productives

On peut vouloir exclure de la surface agricole totale certaines surfaces jugées peu productives :

- Jachère de 6 ans ou plus déclarée comme SIE
- Jachère noire
- Surface pastorale - herbe prédominante et ressources fourragères ligneuses présentes
- Surface pastorale - ressources fourragères ligneuses prédominantes
- Bois pâturé (prairie herbacée sous couvert d'arbres)
- Jachère de 5 ans ou moins
- Jachère de 6 ans ou plus
  Cette classification est reprise de l'outil Crater.

## Limites

- Les surfaces des exploitations non déclarées à la PAC ne sont pas prises en compte : des cas typiques de sous estimation de la SAU par le RPG sont pour les régions viticoles du sud de la France.
- Les chiffres d'évolution de la surface agricole du RPG ne sont pas très fiables à priori du fait de

  - changements de nomenclatures pour certaines années
  - de la variabilité des surfaces déclarées chaque année
  - de l'assolement (rotation des cultures)

- Noter aussi que les Estives et landes sont beaucoup déclarées à la PAC et se retrouvent dans le RPG, mais ce sont des surfaces qui sont peu productives et qu'on peut vouloir exclure de la SAU totale (comme dans la méthodologie Crater par exemple (voir correspondances.rpg_trilettre\_\_crater)

Plus d'info sur outil source : https://outil-sources-interne.basic.coop/#/publication/1/ign-registre-parcellaire-graphique-rpg

## Utilisations dans les modélisations BASIC

Le RPG est un ingrédient de base dans les modélisations BASIC:

- Parcel (potentiel nourricier)
- Flux
- Productions agricoles en volumes
