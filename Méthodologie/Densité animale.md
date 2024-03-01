# Densité animale (herbivores)


### Bases de données :
Les données utilisées pour déterminer le taux de densité d'herbivores (similaire au taux de chargement) sont issues des bases de données suivantes :
- [Recensement Général Agricole (2020)](../Bases%20de%20données/Recensement%20Général%20Agricole.md)
- [Registre Parcellaire Graphique (2020)](../Bases%20de%20données/Recensement%20Parcellaire%20Graphique.md)

### Calcul
La densité animale est le ratio des indicateurs suivants :

**Les UGBAG (Unité Gros Bétail Alimentation Grossière)** qui permettent de comparer et additionner les animaux selon leur consommation en herbe et fourrages (ne concerne que les herbivores) et qui représentent la ration alimentaire d'une vache laitière pendant 1 an  (la durée peut varier pour certains calculs de chargement instantannées ou saisonniers). Cet indicateur se calcule en convertissant chaque animal du cheptel avec les coefficients ci-dessous et en faisant la somme de tous les animaux.

|Espèce|Âge|UGB|
|---|---|---|
|Bovins|Vache laitière|1|
|Bovins|Vaches allaitantes|0,850|
|Ovins|Brebis|0,15|
|Caprins|Chèvres|0,17|
|Equins|Juments|0,8|

Plus d'info sur wikipédia https://fr.wikipedia.org/wiki/Unité_de_gros_bétail

**La Surface Fourragère Principale (SFP)** du RPG qui regroupe les prairies et surfaces fourragères (les surfaces de maïs fourrages sont donc inclues mais pas les surfaces de concentrés telles que les surfaces en céréales, oléagineux et protéagineux)

Ainsi l'indicateur permet d'estimer la pression sur les services ecosystémiques du sol exercée par le cheptel (pollution de l'eau par excrément et lessivage des engrais, appauvrissement du sol par culture intensive de fourrages).

### Limites
- Comme indiqué ci-dessus, l'indicateur ne prend pas en compte les aliments concentrés (blé, mais grain, soja etc.)

- Du fait de la division de deux bases de données indépendantes, on ne fait pas le lien entre chaque cheptel et l'endroit ou il pâture ou bien la localisation des champs de fourrages. Les fourrages peuvent être importés de loin et donner une impression de densité animale plus élevée ou plus faible que si l'on demandait à l'exploitant.e de calculer son taux de chargement (indicateur similaire utilisé à l'échelle d'une exploitation)

- Le taux de chargement qui est similaire est souvent calculé à l'échelle d'une exploitation ou d'un champ, et pas forcément sur une année complète. On le calcule parfois sur la saison de pâturage et il a alors une valeur plus élevée que sur l'année.