# Flux
À l'instar de Parcel, la modélisation des flux de matière alimentaire le long de la chaîne de valeur et à l'intérieur des territoires Français est un méga-modèle mobilisant de nombreuses bases de données et beaucoup d'hypothèses.

**Indicateurs :** tous en kilos équivalent matière première :
- Production
- Consommation
- Export/import

## Bases de données :

Production
- végétale : SAA et RPG
- animale : SAA et DDE
- produits transformés : Prodcom et DDE

Consommation
- humaine : Parcel et consommations à l'échelle nationale
- animale : echelle nationale, SAA et DDE

Import/export : Sitram et Comtrade


## Calcul
Le détail de la méthodologie de calcul est présenté à l'écrit dans [cette note méthodo](https://lebasic.sharepoint.com/:w:/r/sites/Basic_shared_files/Documents%20partages/3%20-%20R%26D/7%20-%20Projets%20de%20recherche/2020-PRA%20analyse%20CV%20territoriale/3-Traitement%20Donn%C3%A9es/Notes%20m%C3%A9thodo/Note%20m%C3%A9thodologique_territorialisation.docx) et de manière graphique [dans ce schéma](https://miro.com/app/board/o9J_l5JcW0o=/)

## Nomenclatures
La construction de ce modèle a occasionné la constitution d'une nomenclature de produits qui comporte les différentes étapes de transformation des produits alimentaires, et qui soit à un niveau d'agrégation qui permette de mettre en relation les différentes bases de données utilisées.
Pour consulter la table : https://outil-sources-interne.basic.coop/#/table/filieres.flux

À consulter également : [la note méthodo sur les correspondances de nomenclatures
](https://lebasic.sharepoint.com/:w:/r/sites/Basic_shared_files/Documents%20partages/3%20-%20R%26D/7%20-%20Projets%20de%20recherche/2020-PRA%20analyse%20CV%20territoriale/3-Traitement%20Donn%C3%A9es/Notes%20m%C3%A9thodo/Correspondances%20de%20nomenclature%20Projet%20de%20recherche%20action.docx?d=w473720e0f72149ecb1ac7e9b3be733c7&csf=1&web=1&e=FDQYFf)

## Limites
- Les imports exports sont calculés en utilisant Sitram, une source peu fiable basée sur un échantillonage de questionnaires à des camioneur.euses. La base n'est pas publique et potentiellement plus éditée depuis 2018.

- Les données à l'échelle de la commune ont peu de sens car souvent issues de totaux départementaux ou nationaux pro-ratisés par rapport à la population, à l'emploi ou la surface agricole.

- N'utiliser qu'un chiffre significatif pour les imports/exports (et encore), 2 pour la production consommation, et systématiquement vérifier avec de la biblio.

## Implémentation
https://github.com/lebasic/outil-analyse-durabilite/tree/master/modele_flux