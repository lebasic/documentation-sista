# Potentiel nourricier

Question de recherche :

**Est-ce que le territoire étudié a suffisamment de surface agricole totale pour théoriquement nourrir sa population ?**

Question bonus : Est-ce que les productions actuelles sont suffisament diversifiées pour subvenir aux besoins des habitants ?

## Bases de données

- [Statistique Agricole Annuelle](../Bases%20de%20données/Statistique%20Agricole%20Annuelle.md)
- [Recensement Général Agricole](Bases%20de%20données/Recensement%20Général%20Agricole.md)
- Bilans d'approvisionnement
- Rica
- Agence Bio
- Comtrade
- [Recensement Parcellaire Graphique](../Bases%20de%20données/Recensement%20Parcellaire%20Graphique.md)
- Statistiques Insee de population
- Inca 3
- FOOD'GES
- Water Foot Print

Ainsi que de nombreux ratios et taux de conversion issus de bibliographie.


## Calcul
Lire la description de la méthode [dans ce document](https://bck.parcel-app.org/storage/app/uploads/public/633/407/dd3/633407dd356ea638253814.pdf)

Alternativement, consulter une représentation graphique du schéma de données de Parcel : https://miro.com/app/board/o9J_lzx3E0A=/

## Nomenclatures
La nomenclature de produits Parcel est construite de manière à pouvoir exprimer tous les produits alimentaires en équivalent matière première. Pour cette raison tous les produits laitiers sont regroupés en un seul produit car tous à base de lait.

[Consulter la table de nomenclature ici](https://outil-sources-interne.basic.coop/#/table/filieres.parcel)

## Limites
- Le potentiel nourricier est théorique : on imagine que les surfaces agricoles soient converties dans les cultures qui correspondent au besoin de la population
- Il ne prend pas en compte l'industrie de transformation nécessaire (voir Potentiel Agro-industriel)
- Les produits pris en compte ne sont que ceux qui peuvent pousser en France métropolitaine, avec des rendements régionalisés pour tenir compte des différentes conditions pédoclimatiques et pratiques d'élevage Françaises.
- Données essentiellement de 2017
- Les seules différences d'habitudes de consommation prises en compte sont celles dûes au sexe et à l'âge.
- Les calculs ne sont pas plus fiables que les données sur lesquels ils se basent (on pense notamment aux bilans d'approvisionnement)
  

## Implémentation

Documentation technique : https://doc.parcel-app.org