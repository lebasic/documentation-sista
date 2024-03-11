# Infrastructures agro-écologiques

On veut représenter sur une carte la part cumulée de plusieurs éléments paysagers favorables à la biodiversité, rapportés à la surface agricole utile de la commune. On regarde ici les infrastructures agroécologiques (IAE) permanentes et non directement agricoles, dont l'effet est plus important à moyen et long termes (la quantification des IAE non permanentes et agricoles - prairies, jachères, estives... - est disponible dans l'onglet "Climat", partie "Surfaces en herbe").  Les différents éléments pris en compte sont donc :

- Les surfaces de haies, calculées à partir des mètres linéaires et multipliées par une largeur règlementaire de 10m (PAC)

- Les zones humides intérieures de Corine Land Cover

- Les bandes tampons de RPG

## Bases de données
- Surfaces du Registre Parcellaire Graphique (RPG)
- Surfaces de Corine Land Cover
- Linéaire de haies de la BD TOPO de l'IGN

## Calcul
Surface d'infrastructure agro-écologique = Surface en bande tampon (RPG) + Longueur de haie (IGN BD Topo) * 10 mètres de largeur (Hypothèse) + Surface en zones humides intérieures (Corine Land Cover)

## Limites
- La largeur de haie de 10 m n'est pas représentative de la réalité. Elle correspond à la largeur règlementaire de la PAC pour obtenir des bonus biodiversité.

- Les zones humides intérieures de Corine Land Cover ne sont pas nécessairement reliées à des surfaces agricoles.


## Implémentation

https://github.com/lebasic/outil-analyse-durabilite/blob/master/modele_tat/DURABILITE/Biodiversité%20habitat%20(2)%20-%20infrastructures%20agro-ecologiques.sql

