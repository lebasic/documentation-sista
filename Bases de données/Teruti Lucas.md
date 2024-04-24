# Teruti Lucas

**Indicateur :** Surface en hectares, détaillée par type d'occupation du sol et par département.

## Méthode de collecte des données

**Avant 2017** : Des enquêteurices vont voir en personne sur une grille de points dans tout le territoire français ce qu'il y a dessus

**À partir de 2020** : 96% des données proviennent de fichiers administratifs : fichiers fonciers, RPG, IGN = plus précis

La méthode est bien détaillée dans cette page : https://artificialisation.developpement-durable.gouv.fr/bases-donnees/teruti-lucas


## Nomenclature


| Code | Type d'occupation du sol |
| --- | --- |
| 001 | Céréales (y compris semences)|
| 002 | Oléagineux (y compris semences)|
| 003 | Protéagineux (y compris semences)|
| 004 | Betteraves industrielles (non compris semences)|
| 005 | Canne à sucre (DOM)|
| 006 | Plantes à fibres (y compris semences)|
| 007 | Cultures industrielles diverses (non compris semences)|
| 008 | Plantes aromatiques, médicinales et à parfum (non compris semences)|
| 009 | Pommes de terre (y compris plants)|
| 010 | "Tubercules, racines et bulbes d'origine tropicale (DOM)"|
| 011 | Légumes frais (non compris semences)|
| 012 | Légumes secs|
| 014 | Fleurs et plantes ornementales|
| 015 | Semences et plants divers|
| 016 | Choux, racines et tubercules fourragers|
| 017 | Fourrages annuels|
| 018 | Prairies artificielles et temporaires|
| 019 | Jardins et vergers familiaux des exploitants|
| 020 | Jachères|
| 022 | Cultures fruitières (y compris châtaigneraies, oliveraies, noyeraies)|
| 023 | Vignes|
| 024 | Pépinières ligneuses|
| 025 | Cultures permanentes autres (oseraies, canne de Provence)|
| 027 | Surfaces toujours en herbe des exploitations|
| 029 | Jardins et vergers familiaux des non exploitants|
| 030 | Surfaces toujours en herbe (S. T. H.) hors exploitations (collectifs et hors champ)|
| 034 | "Surfaces boisées et peupleraies en plein (yc haies et alignements d'arbres"|
| 035 | Landes (non productives, non pacagées), friches, maquis, garrigues|
| 036 | Sols artificialisés|
| 037 | Autres (plages, rochers, eaux intérieures...)|



## Limites
- Cette indicateur est aussi bon que les données sur lesquelles ils se base : si le RPG, l'IGN ou les fichiers fonciers contiennent des erreurs, alors Teruti aussi.
- C'est en 2024 la meilleure source de données à l'échelle départementale pour caractériser l'occupation du sol, mais l'analyse d'image satellitaires OCS GE devrait bientot la dépasser en précision, notamment pour mesurer l'artificialisation.


## Utilisations dans les modélisations BASIC
- Parcel à l'échelle départementale, régionale et France.