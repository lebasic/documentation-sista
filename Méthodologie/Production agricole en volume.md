
# Production agricole en volume

### Bases de données :
- [Statistique Agricole Annuelle](../Bases%20de%20données/Statistique%20Agricole%20Annuelle.md)
- [Recensement Parcellaire Graphique](../Bases%20de%20données/Recensement%20Parcellaire%20Graphique.md)

### Calcul
Les volumes de production sont issus d'une modélisation à partir de deux sources de données : la Statistique Agricole Annuelle (SAA) et le Registre Parcellaire Graphique (RPG). La SAA fournit les productions en volumes a l'échelle du département, que l'on répartit ensuite au prorata des surfaces agricoles par commune, fournies par le RPG.

On peut consulter la table de correspondance entre les surfaces cultivées RPG et les production agricoles de la SAA ici : https://outil-sources-interne.basic.coop/#/table/correspondances.rpg_trilettre__statistique_agricole_annuelle

### Limites
Les volumes de betteraves industrielles et potagères sont répartis avec la donnée de surface de betterave totale (sucrières + potagères) du RPG (qui ne donne pas le détail de ces deux productions). Deux conséquences :
1. Il est possible qu'un territoire ne produise qu'une seule de ces betteraves mais les données ne nous permettent pas de l'identifier. On affecte la même proportion qu'à l'échelle départementale.
2. Comme ces deux productions ont des rendements très différents, on surestime un peu la production de betterave potagère et sous-estime un peu la betterave sucrière.