# Besoins en surfaces agricoles pour nourrir les touristes

**Indicateurs :**
- Nombre de touristes en équivalent personnes annuelles par territoire et nombre de repas
- Besoins en surfaces agricoles pour nourrir les touristes

## Bases de données
- [Nombre de nuitées par an en hôtel et en camping par département (Insee)](https://outil-sources-interne.basic.coop/#/publication/367/insee-tourisme)
- Nombre de places en hôtel et camping par commune (Insee)
- Part des résidences secondaires par commune (Insee)
- Besoin en surfaces agricoles par personne (Parcel)


## Calcul
**Nombre de résident.es secondaires en équivalent personnes annuelles** = population du territoire (Insee) * % de résidence secondaires / (1 - % de résidences secondaires) * taux d'occupation des résidences secondaires (12%)

**Nombre de touristes en équivalent personnes annuelles** = Nombre de nuitées par département * Nombre de places en hotel et camping du territoire / Nombre de places en hotel et camping du département / 365 jours

**Besoins en surfaces agricoles pour nourrir les touristes** = Besoin en surfaces agricoles par personne * ( Nombre de touristes + Nombre de résidents secondaires ) * 365



## Limites
- L’ensemble de ces données ne permet pas de prendre en compte les touristes hébergés chez des particuliers (Airbnb notamment). 


## Implémentation

https://github.com/lebasic/outil-analyse-durabilite/tree/master/modele_tat/CONSOMMATION