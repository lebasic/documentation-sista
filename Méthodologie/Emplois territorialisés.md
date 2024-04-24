# Emplois territorialisés

**Indicateur :** Emplois du territoire (Effectif au 31 décembre)

## Bases de données
- Démographie Des Entreprises (Insee)
- Sirene

## Calcul
Les bases de données que l'on a à disposition nous donnent le nombre d'établissements par commune (DDE, Sirene), sans préciser exactement combien de personnes sont employées mais en précisant la taille de l'établissement dans une fourchette d'emploi. L'effectif utilisé par l'Insee pour ranger les établissements dans des tranches est l'effectif au 31 décembre.


|Taille d'établissement| Effectif moyen modélisé|
|-----|-----|
|Etablissement non employeur|1|
|0 salarié|1|
|1 à 2 salariés|1.5|
|3 à 5 salariés|4|
|6 à 9 salariés|7.5|
|10 à 19 salariés|14.5|
|20 à 49 salariés|34.5|
|50 à 99 salariés|74.5|
|100 à 199 salariés|149.5|
|200 à 249 salariés|224.5|
|250 à 499 salariés|374.5|
|500 à 999 salariés|749.5|
|1 000 à 1 999 salariés|1499.5|
|2 000 à 4 999 salariés|3499.5|
|5 000 à 9 999 salariés|7499.5|
|10 000 salariés et plus|15000|

Pour calculer les emplois du territoire on effectue alors la somme, par taille d'établissement, du nombre d'établissements multiplié par l'effectif moyen de l'établissement.


## Limites
- Remplacer l'effectif réel par la médiane de la tranche est une grosse approximation ! La bonne nouvelle c'est que mathématiquement cette approximation est censée converger vers la vraie valeur quand le nombre d'établissement est élevé, mais peut se révéler très fausse quand on zoome sur un petit territoire et un secteur d'activité.
- Il s'agit d'un effectif au 31 décembre et non d'un effectif équivalent temps plein. Pour des secteurs qui comportent beaucoup de temps partiel, cela peut donner une fausse idée de l'emploi du territoire.


### Différences entre DDE et Sirene

> **Léonard :**
> 
> Salut Gaspard, j'ai retrouvé ce mail de l'INSEE dans mes spam (merci microsoft -_-).
> C'était suite à la question concernant la comparaison entre SIRENE et DDE, et ils répondent que dans DDE, sont comptées toutes les entreprises, même celles qui ont opté pour la "non-diffusion publique". Alors qu'on ne les a pas dans SIRENE. Cela explique pourquoi on a plus de résultats dans DDE que SIRENE du coup, si je me rappelle bien les résultats qu'on avait ^^.
> 
> De : CONTACT INSEE <contact@contact-insee.fr>
> Envoyé : jeudi 2 décembre 2021 11:28
> À : Léonard Michelet <leonard@lebasic.com>
> Objet : Insee : suite à votre demande d'information statistique : ticket numéro 1280075 [1281339-1638440922]
>
> Bonjour,
>
> Avec la base de données "démographie des entreprises", vous avez accès à toutes les unités présentes dans cette base et relevant du champ défini par cette même base.
> 
> En revanche, lorsque vous consultez le site www.sirene.fr,  vous avez UNIQUEMENT accès aux entreprises et établissements relevant de la diffusion publique.
> 
> Les sociétés et associations pouvant bénéficier de cette possibilité et les entrepreneurs individuels ayant opté pour la non-diffusion publique n'y sont donc pas répertoriés.
> 
> Vous ne pouvez pas donc pas comparer les chiffres issus de ces deux différentes sources.
>  
> 
> Nous vous rappelons ci-après, les textes régissant la diffusion publique.
> 
> Les articles R. 123-220 à R. 123-234 du code de commerce instituent un système national d'identification des entrepreneurs individuels ainsi que des personnes morales et de leurs établissements articulés autour du répertoire Sirene. La gestion de ce répertoire est confiée à l'Insee.
> 
> La responsabilité de l'Insee dans la gestion du répertoire, et notamment dans la diffusion de son contenu, se limite donc à la stricte application des lois en vigueur.
> 
> L'article R123-222 du code de commerce liste les éléments d'identification des entreprises qui sont portés au répertoire Sirene. L'article R123-232 du code de commerce précise également que l'Insee peut communiquer aux personnes ou organismes qui en font la demande les renseignements contenus dans le répertoire Sirene, à l'exception de ceux concernant la date et le lieu de naissance des personnes physiques.
> 
> La divulgation de ces données est une décision du législateur motivée par la nécessité pour les tiers de pouvoir accéder aux coordonnées d'une entreprise à partir de son numéro Siren, ainsi que par le besoin de la plupart des entreprises de pouvoir être facilement identifiées par leurs fournisseurs et clients.
> 
> Toutefois, pour les personnes physiques, aux termes de l'article A123-96 du code de commerce et conformément à l'article 21 du Règlement général de protection des données personnelles , pour ne plus figurer (ou figurer de nouveau) dans la base de données Sirene diffusion, (même pour une entreprise cessée), vous devez accéder à la téléprocédure par le portail FranceConnect.
> 
> Ainsi, seules les entreprises personnes physiques sont autorisées à modifier leur statut de diffusion. Pour les entreprises  personnes morales, la mise en diffusion est obligatoire à l’exception de quelques cas.
> 
> 
> 
> Nous sommes à votre disposition pour de plus amples informations.
> 
> Cordialement,
> Insee contact