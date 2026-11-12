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

## Lecture du rapport

Groupe 8 : Flavien, Leticia, Sarah, Marie, Arthur et Cheikh.

Ordre de lecture : [Health](health.ipynb), [Ecology](ecology.ipynb),
[Logistics](logistics.ipynb), [Public Records](public_records.ipynb), puis
[synthèse transversale](synthese_transversale.ipynb). Chaque domaine possède
ses propres préparations ; les rapprochements inter-domaines sont recalculés
depuis les CSV sources dans la synthèse. Le fichier Base reste un document
de travail et ne remplace pas les notebooks de domaine.

## Récit caché reconstitué

Les sources convergent vers le scénario suivant : **une population dissimulée
parmi les humains, désignée comme « Chamaeleonidian », est associée à des
identités publiques et à des réseaux durables. Une infrastructure écologique
et logistique organise des flux biologiques restreints autour de Meridian.
Les documents rapportent notamment une consommation de chauves-souris.
Une branche clinique Asterion fournit parallèlement des interventions
récurrentes à huit personnalités influentes. Les archives décrivent des
stratégies opposées concernant l'exploitation de l'environnement, le
réchauffement et la divulgation. Un transfert non terrestre est évoqué,
sans itinéraire matériellement reconstitué.**

Ce récit est entièrement fictif. La conclusion distingue les relations
calculées dans les tables, les affirmations des documents et les hypothèses.
Elle ne constitue pas un corrigé officiel ni une garantie d'avoir identifié
toutes les intentions de l'auteur. La consigne demande un narratif : nous
n'avons pas identifié de règle de décodage établissant une phrase chiffrée
unique à restituer mot pour mot.

### 1. Particularités physiologiques et identité publique

Trois dossiers constituent les principales pistes cliniques :

- **PAT-31065** : `CLN-510027` décrit deux sources contractiles spatialement
  distinctes et partiellement indépendantes. Les signaux apportent des
  discordances persistantes, sans établir à eux seuls deux cœurs anatomiques.
- **PAT-31115** : `CLN-510055` décrit des discordances de capture visuelle et
  thermique qui persistent partiellement avec un autre appareil. Un contrôle
  délibéré de l'apparence est envisagé, mais aucun mécanisme de transformation
  n'est démontré.
- **PAT-31012** : `CLN-510064` associe une démarche oscillante à un équilibre
  préservé et à des particularités oculaires et rythmiques répétées.

`PUB-510063` rapporte la classification restreinte « Chamaeleonidian » pour
une population clinique inhabituelle. Les mesures n'identifient pas seules
une espèce, son origine ou le nombre d'individus concernés.

`CLN-510025` rapproche PAT-31065 d'**Elias Voss**, président de Meridian
BioLogistics. Cette résolution est affirmée par la note, mais n'est pas
reproduite par une égalité des attributs administratifs : Health enregistre
**Corin Hallen, né en 1975**, contre **Elias Voss, né en 1961**, dans le
registre public. Corin Hallen ne doit pas non plus être confondu avec
**Dr Corin Hale**, le rédacteur des deux notes centrales de ce dossier.

Sources : [notes cliniques](data/health/clinical_notes.csv),
[patients](data/health/patient_administration.csv),
[déclarations de responsables](data/public_records/officer_filings.csv)
et [documents publics](data/public_records/public_and_investigative_documents.csv).

### 2. Continuités historiques : des pistes, pas des égalités d'identité

Les registres font apparaître deux successions chronologiques de fonctions :

| Parcours commercial et médical | Parcours naturaliste et écologique |
| --- | --- |
| Edward Vann : nomination en 1840 | J. Varlan : nomination en 1885 |
| Emil Warden : 1895 | Jonah Bell : 1924 |
| Adrian Vosmere : 1952 | Julien Marot : 1970 |
| Elias Voss : 1996 | Jacob Vale : 2008 |

`PUB-510043` et `PUB-510076` rapprochent des adresses, des associés et des
formulations historiques, avec une piste explicite entre Vosmere et Voss.
Ces récurrences soutiennent le thème de réseaux durables et d'identités
potentiellement renouvelées. Elles ne prouvent pas que chaque colonne du
tableau représente une seule personne. Les minutes de 1962 nomment même
Bell, Marot et Vale ensemble.

La licence d'Emil Warden, délivrée en 1895, apparaît dans 147 rencontres
Health jusqu'en 2025 et dans 35 actes jusqu'en 2024. J. Varlan et Jonah Bell
possèdent aussi des licences anciennes encore actives. Mais le registre
contient également une licence délivrée en 2026 associée à des actes
antérieurs : les erreurs de date ou la réutilisation d'identifiants doivent
être examinées avant de conclure à une longévité exceptionnelle.

Sources : [déclarations](data/public_records/officer_filings.csv),
[licences professionnelles](data/public_records/licensed_professionals.csv),
[rencontres](data/health/clinical_encounters.csv),
[actes](data/health/clinical_procedures.csv) et documents `PUB-510043`,
`PUB-510076`, `PUB-510033` et `PUB-510044`.

### 3. Approvisionnement biologique et cloisonnement des informations

Les identifiants d'organisations permettent de rapprocher les domaines :

| Organisation | Registre public | Partenaire ERP | Relation observée |
| --- | --- | --- | --- |
| Horizon Field Research Cooperative | REG-AVL-01013 | BP-30056 | Demande des accès et expédie le sous-ensemble écologique |
| Meridian BioLogistics | REG-VLN-01001 | BP-30078 | Reçoit ce sous-ensemble et expédie le sous-ensemble clinique |
| Asterion Clinical Institute | REG-VLN-01002 | BP-30021 | Reçoit le sous-ensemble clinique et exploite les deux établissements des actes répétés |

Le circuit comprend **18 expéditions environnementales et animalières**,
déclarées comme échantillons biologiques en lots scellés, et **26 livraisons
de programme clinique**, comprenant échantillons biologiques ou consommables
médicaux. Ces 44 expéditions sont déclarées à 2–8 °C ; leurs classes
d'autorisation ne sont pas toutes `restricted`. Le transporteur récurrent
est Northstar Cold Chain Services, distinct de Meridian.

À **KNT-KES**, le dossier `ACC-2024-0014` enregistre un accès Horizon du
21 mars 2024 à 18 h au 22 mars à 03 h. `SHP-2024-00007` part six heures
plus tard, du dépôt FCL-1030 vers l'installation d'agrégation biologique
Meridian FCL-1024. Il déclare **six lots scellés, pas six animaux**.

`EFR-510088` décrit des traces de manipulation et une baisse d'activité.
La baisse commence toutefois avant l'accès, n'est pas unique parmi les sites
et ne permet pas de compter des animaux prélevés. Le rapport comporte aussi
des discordances de dates et de disponibilité d'appareil détaillées dans
Ecology. `PUB-510079` apporte un témoignage explicite sur une consommation
de certaines Eonycteris spelaea collectées ; il ne fournit pas la liste
des consommateurs ni la destination de tous les lots.

`MEM-510100` décrit **CHAMELEO** comme une procédure de routage et de gestion
séparée des dossiers ordinaires et des annexes scellées. `MEM-510101` relie
**Unwabu** à l'autorité approuvant les exceptions et au bureau exécutif de
Meridian. Ce mécanisme éclaire le cloisonnement des informations. Il ne
permet pas d'établir qu'Unwabu est Elias Voss ou un autre individu précis.

Sources : [expéditions](data/logistics/shipments.csv),
[partenaires ERP](data/logistics/erp_business_partners.csv),
[entités enregistrées](data/public_records/registered_entities.csv),
[événements d'accès](data/public_records/site_access_case_events.csv),
[rapports écologiques](data/ecology/environmental_field_reports.csv) et
[mémos institutionnels](data/public_records/institutional_memos.csv).

### 4. Une branche clinique sélective, distincte des dossiers physiologiques

MRP-42 représente **50 actes chez 28 patients**. Vingt personnes ont un acte
unique de recherche ; huit bénéficiaires reçoivent les 30 actes répétés :

| Patient | Nom administratif | Actes MRP-42 |
| --- | --- | ---: |
| PAT-31221 | Leora Kassen | 5 |
| PAT-31044 | Tavian Serat | 4 |
| PAT-31174 | Mirek Talven | 4 |
| PAT-31119 | Celene Varro | 4 |
| PAT-31074 | Oskar Nivren | 4 |
| PAT-31183 | Adrienne Solva | 3 |
| PAT-31142 | Rayan Belen | 3 |
| PAT-31099 | Elira Vaun | 3 |

Les noms et années de naissance rapprochent ces bénéficiaires de responsables
politiques, économiques et institutionnels. Les actes répétés utilisent
LIC-VLN-MED-1002, la licence de Dr Naima Orrel, dans les deux établissements
Asterion FAC-VLN-101 et FAC-AVL-201. **Les trois patients physiologiquement
atypiques cités plus haut ne figurent pas parmi ces huit bénéficiaires.**

Les 26 livraisons cliniques précèdent 26 actes distincts dans le même
établissement, de **4,2 à 7,8 jours**. La comparaison par établissement et
année conserve 25 livraisons cliniques comparables à des témoins ; la
dernière reste sans témoin. Cette correspondance n'identifie pas le contenu
administré : aucune clé disponible ne relie directement un lot réceptionné
au matériel MRP-42 utilisé chez un patient.

L'écart moyen entre âge chronologique et BIOAGE estimé est de **11,32 ans**
chez les huit bénéficiaires répétés, contre environ un an dans les autres
groupes. Cela soutient l'existence d'un programme particulier dans le récit,
sans démontrer son mécanisme, son efficacité rajeunissante ou un échange
de bénéfices contre un soutien politique. Les trois actes d'Elira Vaun
précèdent le décès public de 2021 : ils ne prouvent pas une intervention
post mortem.

Sources : [procédures](data/health/clinical_procedures.csv),
[observations](data/health/clinical_observations.csv),
[nominations publiques](data/public_records/public_appointments.csv),
`PUB-510045` et [calculs de la synthèse transversale](synthese_transversale.ipynb).

### 5. Stratégies environnementales opposées et hypothèse de transfert extérieur

Les minutes de 1962 (`PUB-510033`) opposent Bell, favorable aux effets
attendus du réchauffement et des corridors floraux, Marot, qui veut intégrer
les accès aux grottes aux infrastructures, et Vale, qui critique une
stratégie dépendant de l'extraction et d'une hausse permanente de chaleur.
`PUB-510094` retrouve une tension entre continuité de programmes contrôlés
et transparence, protection des habitats et contrôle indépendant.

Le récit suggère donc des stratégies concurrentes autour d'intérêts de long
terme. Il ne démontre ni que ce réseau aurait provoqué le réchauffement
mondial, ni que tous les militants écologistes ou Jacob Vale appartiendraient
à la population décrite.

`PUB-510063` rapporte une expression de **« non-terrestrial transfer »**.
Le document précise lui-même que l'itinéraire, la destination, le contenu
et l'ampleur ne sont pas identifiés. Il ne permet pas de désigner une planète,
d'affirmer que les chauves-souris y sont expédiées ou de déterminer l'origine
de la population.

### 6. Vérifications qui empêchent de surinterpréter le récit

- **Dates des mémos et dates des transports.** `MEM-510100` date de 2023
  et cite SHP-2022-00011, partie le 9 février 2022. `MEM-510101` date de
  2025 et cite SHP-2023-00035, partie le 30 mai 2023. Les deux expéditions
  sont déclarées `ambient` et `ordinary`, respectivement comme équipements
  de protection et service juridique. Leur lien documentaire avec CHAMELEO
  ne suffit pas à les présenter comme deux cargaisons biologiques réfrigérées.
- **Volumes de transport.** Les comptes selon la date réelle de départ
  donnent 43 expéditions en 2021, 61 en 2022, 73 en 2023, 47 en 2024 et
  34 en 2025. Le maximum observé est 2023, pas 2021 ou 2024. Les transports
  de 2025 s'arrêtent au 15 juin : le total ne décrit pas une année complète.
- **Lieux et documents.** Valenne Central District est nommé dans 14 des
  40 documents publics. Cela ne signifie pas 14 enquêtes rédigées sur place.
  Les sept documents datés de 2025 sont de types différents ; un seul est
  une `investigative_note`.
- **Rôle d'AVL-301.** Le laboratoire regroupe les dix professionnels
  environnementaux et les neuf professionnels de recherche du registre,
  mais aucun des huit médecins n'y a son établissement principal enregistré.
  Cette concentration ne démontre ni une direction unique ni une complicité
  de tous les intervenants.
- **Indépendance des sources.** Mara Venn signe `PUB-510079` et `PUB-510063` ;
  Soren Kade signe les trois mémos centraux ; Jora Menne signe les pistes
  `PUB-510044` et `PUB-510076`. Ces textes ne sont pas autant de témoignages
  indépendants.
- **Contre-exemples.** `MEM-510089` emploie CHAMELEO pour un ancien logiciel ;
  `PUB-510070` présente Chamaeleonidian comme une métaphore ; `PUB-510127`
  cite Unwabu dans un contexte maritime ou folklorique ; `PUB-510121`
  emploie non-terrestrial pour des observations satellitaires. Les usages
  ordinaires ne doivent pas être fusionnés avec les indices du programme.

### Portée de la conclusion

Le noyau du récit est étayé par les textes et par une partie des relations
structurées. Restent non établis : les égalités exactes entre identités
historiques, l'identité physique d'Unwabu, le consommateur et le devenir de
chaque lot, le mécanisme de MRP-42, un éventuel échange politique et la
destination extérieure. Les affirmer comme des faits rendrait le récit plus
précis que les sources disponibles.

Le détail des préparations, contrôles et résultats négatifs reste dans les
notebooks de domaine. La [synthèse transversale](synthese_transversale.ipynb)
présente les rapprochements recalculés ; la
[synthèse rédigée](Synthese_croisee_narratif.md) en propose une autre lecture.

**Assistance IA.** Une assistance a été utilisée pour le recoupement des
données, la vérification du code et l'aide à la rédaction. Les sources,
calculs, contradictions et limites sont exposés pour permettre la discussion
et la vérification par le groupe.

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

/!\ Ces jeux de données sont entièrement synthétiques et ont été créé dans un but pédogagique.
Ils ne représentent pas des informations factuelles à propos de personnes réelles,
d’organisations réelles, de gouvernnements réels ou localisations réelles.
Toute ressemblance avec des personnes réelles, physiques ou morales, est totalement involontaire et fortuite. /!\ 
 
## Pour bien commencer

1. Faites un `fork` de ce repository vers un noveau repository pour votre groupe.
2. Clonez le repository de votre groupe sur votre machine.
3. Créez un environnement : `python -m venv .venv` (version testée : Python 3.14.7).
4. Activez-le puis installez les dépendances : `python -m pip install -r requirements.txt`.
5. Dans VS Code, sélectionnez son interpréteur et son noyau Python ; ou lancez `python -m notebook nom-du-notebook.ipynb`.
6. Travaillez en groupe et complétez le notebook

Les dépendances sont déclarées au format pip, et non sous forme d'un export
Conda spécifique à une machine. Sur Windows, l'interpréteur se trouve dans
`.venv\Scripts\python.exe`. Le dossier courant doit être celui qui contient
`data/`. Pour vérifier un notebook, redémarrez son noyau puis exécutez toutes
les cellules dans l'ordre. Les données brutes ne doivent pas être écrasées.

## Rendu

Le rendu pourra se faire via:

* une `pull-request`, 
* en m’envoyant une archive .zip contenant votre travail à `antoine.richard@chu-lyon.fr`.
