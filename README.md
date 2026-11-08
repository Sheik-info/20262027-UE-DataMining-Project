# Année 2026-2027 - M2IA/M2DS - UE Data Mining - Projet

Sur ce repository, vous pourrez trouver l’ensemble des éléments
nécessaire au projet de groupe de l’UE Data Mining pour l’année 2026-2027.

Votre objectif est de mettre en évidence le narratif caché à l’intérieur
de ces données à l’aide des notions et méthodes vues au fur et
à mesure de l’UE Data Mining.

/!\ Ce narratif est entièrement fictif. Il a été créé dans un objectif pédagogique et ne reflète aucunement la réalité /!\

Pour ce faire, vous travaillerez en groupe en débattant et
en vous répartissant les tâches à faire.

Le rendu attendu est un rapport, sous la forme d’un notebook jupyter,
qui détaillera vos réflexions, les méthodes et vos conclusions.

Pour cela, le fichier `Base_notebook_to_complete.ipynb` est mis à votre disposition (vous pouvez changer le nom si vous le souhaitez).

Pensez à bien y préciser:

* Le nom de votre groupe
* La liste des membres

Vous serez avant tout évalué sur votre méthode, donc soyez précis, détaillé
et rigoureux dans vos descriptions.

/!\ L’usage de l’IA Générative est fortement déconseillé (ce sont vos cerveaux que l’on souhaite entrainer ici).
Si vous souhaitez tout de même l’utiliser, cela doit être justifié et documenté dans votre rapport /!\

## Jeux de données

Dans le dossier `data/`, vous trouverez les ensembles des jeux de données suivants:

- `data/public_records/` — jeux de données issus d’institutions administratives publiques,
- `data/health/` — jeux de données médicales issus de cliniques et d’hôpitaux,
- `data/ecology/` — jeux de données issus de recherches environnementales,
- `data/logistics/` — jeux de données issus de groupes et d’entreprises privées.

Le fichier `data/data_dictionary.csv` détaille les caractéristiques des variables présentes dans chaque jeu de données.

## Analyses Health du groupe

[health.ipynb](health.ipynb) réunit les contributions de Leticia et Flavien dans
une seule analyse : préparation des sept tables, profils administratifs et
cliniques, comparaisons par consultation et par acte, motifs et anomalies,
graphes et parcours, calendriers, signaux cardiaques et notes cliniques.

Les nettoyages communs ne sont pas exécutés deux fois. Les analyses à des
échelles différentes sont distinguées et leurs limites discutées ; elles ne
constituent pas des validations indépendantes. Le notebook s'exécute depuis
la racine du dépôt, sans commande Git ni écriture dans les CSV sources.
Les contributions antérieures restent accessibles dans l'historique Git.

## Ecology et synthèse transversale

- [ecology.ipynb](ecology.ipynb) : analyse des six fichiers Ecology, de la qualité
  des données aux profils de sites, séries mensuelles et rapports de terrain.
- [synthese_transversale.ipynb](synthese_transversale.ipynb) : recoupements
  reproductibles entre les quatre domaines, avec références et contre-exemples.
- [Synthese_croisee_narratif.md](Synthese_croisee_narratif.md) : lecture rédigée
  des résultats croisés et des hypothèses du narratif fictif.

La synthèse transversale est une proposition à discuter collectivement : elle
ne remplace pas la validation des analyses de chaque domaine et distingue les
jointures calculées, les affirmations documentaires et les hypothèses.

Les [messages Health](coordination/message_health.md) et
[Ecology](coordination/message_ecology.md) sont des documents de coordination,
séparés des notebooks de rendu. Les sauvegardes, fichiers temporaires, supports
de cours et fiches personnelles de révision ne font pas partie de cette publication.

/!\ Ces jeux de données sont entièrement synthétiques et ont été créé dans un but pédogagique.
Ils ne représentent pas des informations factuelles à propos de personnes réelles,
d’organisations réelles, de gouvernnements réels ou localisations réelles.
Toute ressemblance avec des personnes réelles, physiques ou morales, est totalement involontaire et fortuite. /!\ 
 
## Pour bien commencer

1. Faites un `fork` de ce repository vers un noveau repository pour votre groupe.
2. Clonez le repository de votre groupe sur votre machine.
3. (Installez conda si ce n’est pas déjà fait)
4. Installez les dépendances avec la commande: `conda create --name <envname> --file requirements.txt`
5. Lancez le notebook avec la commande: `jupyter notebook nom-du-notebook.ipynb`
6. Travaillez en groupe et complétez le notebook

## Rendu

Le rendu pourra se faire via:

* une `pull-request`, 
* en m’envoyant une archive .zip contenant votre travail à `antoine.richard@chu-lyon.fr`.
