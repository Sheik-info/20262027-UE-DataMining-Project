# Projet Data Mining — M2IA / M2DS (2026–2027)

**Groupe 8 :** Flavien, Leticia, Sarah, Maria, Arthur et Cheikh.  
**UE :** Data Mining  
**Nature du document :** rapport d'analyse et guide de lecture des notebooks.

> **Avertissement :** tous les jeux de données et le récit étudié sont fictifs, créés à des fins pédagogiques. Ils ne décrivent aucune personne, organisation ou situation réelle.

## Sommaire

1. [Contexte et objectifs](#1-contexte-et-objectifs)
2. [Jeux de données](#2-jeux-de-données)
3. [Organisation du rapport et notebooks](#3-organisation-du-rapport-et-notebooks)
4. [Démarche méthodologique](#4-démarche-méthodologique)
5. [Résultats et récit caché reconstitué](#5-résultats-et-récit-caché-reconstitué)
6. [Contrôles, contradictions et limites](#6-contrôles-contradictions-et-limites)
7. [Conclusion et portée des résultats](#7-conclusion-et-portée-des-résultats)
8. [Reproduction des analyses](#8-reproduction-des-analyses)
9. [Assistance IA](#9-assistance-ia)

## 1. Contexte et objectifs

Ce projet de groupe de l'UE Data Mining vise à **mettre en évidence un narratif caché** à partir de données synthétiques réparties en quatre domaines : santé, écologie, logistique et archives publiques.

Notre démarche consiste à explorer les données de chaque domaine, à relever les anomalies et régularités, puis à confronter les informations entre domaines. Le but est de proposer une reconstruction argumentée du récit, en explicitant les preuves, les calculs, les contradictions et les incertitudes.

**Principe de lecture :** les correspondances mesurées dans les tables, les affirmations contenues dans les documents et les hypothèses interprétatives sont distinguées tout au long du rapport.

## 2. Jeux de données

| Domaine | Dossier source | Nature des informations |
| --- | --- | --- |
| Santé (Health) | `data/health/` | Données médicales issues de cliniques et d'hôpitaux |
| Écologie (Ecology) | `data/ecology/` | Recherches environnementales et observations de terrain |
| Logistique (Logistics) | `data/logistics/` | Données d'entreprises, de stocks et de transport |
| Archives publiques (Public Records) | `data/public_records/` | Registres et documents administratifs |

Le dictionnaire `data/data_dictionary.csv` décrit les variables présentes dans les différents jeux de données.

## 3. Organisation du rapport et notebooks

Le **présent README contient le rapport narratif détaillé** : résultats, éléments de preuve, rapprochements et limites. Les notebooks fournissent les analyses reproductibles, les préparations de données et les calculs sur lesquels repose ce rapport.

| Ordre | Notebook | Contenu |
| --- | --- | --- |
| 1 | [Health](health.ipynb) | Sept tables : profils cliniques, signaux, notes et interventions répétées ; contributions de Leticia et Flavien réunies |
| 2 | [Ecology](ecology.ipynb) | Six fichiers : conditions de collecte, profils de sites, variations mensuelles et rapports de terrain |
| 3 | [Logistics](logistics.ipynb) | Sept fichiers : stocks, commandes, réceptions et circuits de transport |
| 4 | [Public Records](public_records.ipynb) | Neuf fichiers : registres, documents, références et parcours administratifs |
| 5 | [Synthèse transversale](synthese_transversale.ipynb) | Recoupements recalculés entre les quatre domaines, textes sources, contradictions et conclusion |

Chaque notebook de domaine prépare et analyse ses tables. La synthèse transversale **recalcule les rapprochements depuis les CSV sources**, afin de rendre vérifiables les correspondances présentées ci-dessous. `Base_notebook_to_complete.ipynb` est le modèle initial et ne fait pas partie du rapport final. Les contributions antérieures restent consultables dans l'historique Git.

## 4. Démarche méthodologique

Notre analyse s'articule autour des étapes suivantes :

1. **Exploration par domaine :** examiner les fichiers et leurs variables, en s'appuyant sur le dictionnaire de données.
2. **Préparation et vérifications :** contrôler la cohérence des identifiants, des dates et des informations utiles aux rapprochements.
3. **Recherche de régularités et d'anomalies :** étudier les dossiers cliniques, les événements écologiques, les flux logistiques et les archives administratives dans leurs notebooks respectifs.
4. **Recoupements transversaux :** rapprocher organisations, lieux, événements, identifiants et chronologies entre les quatre domaines ; les calculs correspondants sont regroupés dans la synthèse transversale.
5. **Confrontation des hypothèses :** examiner les documents textuels, les contre-exemples et les incohérences avant de formuler une interprétation.

**Niveau de preuve utilisé dans ce rapport :**

- **Observation calculée :** résultat obtenu à partir des tables et vérifiable dans les notebooks.
- **Affirmation documentaire :** information mentionnée dans une note, un rapport ou un mémo, qui ne constitue pas nécessairement une preuve indépendante.
- **Hypothèse :** interprétation proposée pour relier les indices ; elle reste signalée comme telle lorsqu'aucune vérification directe n'est possible.

Les sections suivantes exposent l'ensemble des résultats détaillés, en conservant les identifiants des dossiers et les références aux fichiers sources.

## 5. Résultats et récit caché reconstitué

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

### 5.1. Particularités physiologiques et identité publique

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

### 5.2. Continuités historiques : des pistes, pas des égalités d'identité

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

### 5.3. Approvisionnement biologique et cloisonnement des informations

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

### 5.4. Une branche clinique sélective, distincte des dossiers physiologiques

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

### 5.5. Stratégies environnementales opposées et hypothèse de transfert extérieur

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

## 6. Contrôles, contradictions et limites

### 6.1. Vérifications qui empêchent de surinterpréter le récit

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

## 7. Conclusion et portée des résultats

### 7.1. Portée de la conclusion

Le noyau du récit est étayé par les textes et par une partie des relations
structurées. Restent non établis : les égalités exactes entre identités
historiques, l'identité physique d'Unwabu, le consommateur et le devenir de
chaque lot, le mécanisme de MRP-42, un éventuel échange politique et la
destination extérieure. Les affirmer comme des faits rendrait le récit plus
précis que les sources disponibles.

Le détail des préparations, contrôles et résultats négatifs reste dans les
notebooks de domaine. La [synthèse transversale](synthese_transversale.ipynb)
présente les rapprochements recalculés et les textes sources.

## 8. Reproduction des analyses

**Prérequis :** Python 3.14.7 (version indiquée comme testée), Jupyter Notebook et les dépendances de `requirements.txt`.

Depuis la racine du dépôt (contenant `data/`) :

```bash
python -m venv .venv
python -m pip install -r requirements.txt
python -m notebook
```

Activez l'environnement virtuel avant d'installer les dépendances et de lancer Jupyter : sous Windows, `.venv\Scripts\activate` ; sous macOS/Linux, `source .venv/bin/activate`.

Ouvrez les notebooks dans l'ordre de lecture indiqué en section 3. Pour vérifier leur reproductibilité, redémarrez le noyau et exécutez toutes les cellules dans l'ordre. Ne modifiez pas les données brutes. Les dépendances sont déclarées au format pip, et non dans un export Conda propre à une machine. Dans VS Code, sélectionnez l'interpréteur de l'environnement virtuel et le noyau correspondant.

## 9. Assistance IA

Une assistance IA a été utilisée pour le recoupement des données, la vérification du code et l'aide à la rédaction. Les sources, calculs, contradictions et limites sont exposés pour permettre leur discussion et leur vérification par le groupe.

