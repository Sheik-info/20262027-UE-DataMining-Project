# Reconstitution du narratif fictif — synthèse croisée

Cette lecture rapproche Ecology, Logistics, Health et Public Records. Elle distingue les relations calculées dans les tables, les affirmations des documents et les hypothèses. Les données du projet sont entièrement synthétiques. Les calculs reproductibles et les textes sources sont présentés dans [synthese_transversale.ipynb](synthese_transversale.ipynb) ; les contrôles détaillés Ecology sont dans [ecology.ipynb](ecology.ipynb).

## 1. Un réseau d'organisations peut être reconstitué

Les correspondances reposent sur les numéros d'enregistrement, et non sur les seuls noms :

| Organisation | Registre public | Partenaire ERP | Relation observée |
| --- | --- | --- | --- |
| Horizon Field Research Cooperative | REG-AVL-01013 | BP-30056 | Demande des accès écologiques et expédie le sous-ensemble environnemental |
| Meridian BioLogistics | REG-VLN-01001 | BP-30078 | Reçoit ce sous-ensemble et expédie le sous-ensemble clinique |
| Asterion Clinical Institute | REG-VLN-01002 | BP-30021 | Reçoit le sous-ensemble clinique ; exploite les établissements du programme répété |

Les expéditions déclarées comprennent **18 transports de matériels environnementaux et animaliers** et **26 livraisons cliniques à température contrôlée**. Le transporteur récurrent est **Northstar Cold Chain Services**, BP-30047 : il ne faut pas le confondre avec Meridian, destinataire puis expéditeur.

Les licences Health FAC-VLN-101 et FAC-AVL-201 correspondent aux établissements ERP FCL-1010 et FCL-1007 par nom normalisé et organisation exploitante. Cela fournit un pont entre les référentiels, mais pas la preuve qu'un même contenu a circulé d'un site écologique jusqu'à un patient.

Sources : `registered_entities.csv`, `erp_business_partners.csv`, `erp_facilities.csv`, `licensed_facilities.csv`, `shipments.csv`.

## 2. KNT-KES est une piste croisée, pas une anomalie écologique unique

Les 64 sites sont suivis mensuellement pendant 78 mois, de janvier 2019 à juin 2025. Les observations sont rapportées aux heures d'effort ; les saisons et la qualité sont examinées avant d'interpréter une baisse.

À KNT-KES, l'indice observé vaut **45,9 % de sa référence calendaire en avril 2024** et **15,4 % en mai**, la référence étant la médiane du même mois en 2019–2023. Mai reste signalé lorsque l'on exige une disponibilité d'appareil d'au moins 90 %. Les mois analogues sélectionnés sur cinq conditions environnementales et de collecte ont des ratios plus élevés, mais ne constituent pas des témoins expérimentaux.

Cette baisse n'est pas unique : sur janvier 2024–juin 2025, TMB-PEL compte sept mois sous la moitié de sa référence, contre cinq pour KNT-KES. Les méthodes globales d'anomalies désignent surtout TMB-BRC, dont l'activité est élevée. La priorité donnée à KNT-KES vient donc de ses documents et de ses liens datés, pas d'un classement statistique qui l'isolerait sans ambiguïté.

Le dossier **ACC-2024-0014** enregistre un accès Horizon à KNT-KES du **21 mars 2024 à 18 h au 22 mars à 03 h**. L'expédition **SHP-2024-00007** part le **22 mars à 09 h**, soit six heures plus tard, de **FCL-1030** vers **FCL-1024**, l'installation d'agrégation biologique de Meridian. La déclaration porte sur **six lots scellés**, pas sur six animaux.

Le rapport **EFR-510088** décrit des traces de manipulation et une baisse d'activité, tout en laissant ouvertes des explications naturelles. Trois réserves sont importantes : la baisse commence déjà avant cet accès ; le rapport du 2 avril cite un relevé commençant le 5 avril ; sa disponibilité annoncée au-dessus de 90 % diffère du taux mensuel d'avril de 83,1 %. De plus, le dossier réglementaire **REG-2023-0008**, qui relie site et expédition, est daté de 2023 mais cite l'expédition de 2024. Ces discordances sont conservées.

Les vergers complètent le contexte écologique : leur activité de chauves-souris est associée à la nouaison et au rendement, mais les corrélations diminuent nettement après retrait des différences de site et du calendrier. Cela ne démontre ni un effet causal de pollinisation ni une manipulation climatique intentionnelle.

Sources : les six fichiers Ecology, `site_access_case_events.csv`, `regulatory_case_events.csv`, `shipments.csv`.

## 3. Les documents précisent gouvernance et usage allégué

**MEM-510100** décrit une procédure CHAMELEO de traitement séparé des dossiers et d'annexes scellées. **MEM-510101** relie explicitement la désignation **Unwabu** à l'autorité approuvant les exceptions CHAMELEO et au bureau exécutif de Meridian. Ce lien est plus précis qu'une recherche par mot-clé ; il n'établit pas qu'Unwabu est un individu nommé.

**PUB-510079** apporte un témoignage sur des **Eonycteris spelaea collectées**, des unités restreintes et un usage décrit comme de la **consommation**. Le témoin déclare ne pas connaître l'ensemble du réseau. Il s'agit d'un élément narratif explicite à confronter aux autres sources, non d'une utilisation finale démontrée par les comptages Ecology.

Les écarts de stock sont calculés en conservant catégorie et unité. **ADJ-2024-00117** est effectivement lié à SHP-2024-00007 et porte sur −3,02 lots scellés, avec un motif déclaré de correction de transfert. Il ne démontre pas une consommation. **MEM-510062**, daté d'avril 2024, évoque un déficit biologique mais cite **ADJ-2022-00088**, qui concerne des consommables médicaux en caisses en février 2022. Cette discordance empêche d'en faire une preuve directe du devenir des lots de mars 2024.

Contre-exemples : **MEM-510089** emploie CHAMELEO pour un ancien tableau de bord ; **PUB-510127** emploie Unwabu dans un contexte maritime ou folklorique ; **EFR-510082** décrit une collecte autorisée suivie de remise en liberté. Ces sens ne doivent pas être fusionnés.

## 4. Une branche clinique concerne huit bénéficiaires récurrents

MRP-42 représente **50 actes chez 28 patients**. Huit patients reçoivent **30 actes répétés**, de trois à cinq chacun, dans les deux établissements Asterion cités et avec la licence professionnelle **LIC-VLN-MED-1002**. Des noms et années de naissance correspondent à des responsables publics ou d'entreprise ; les rapprochements nominatifs sont des candidats à vérifier, pas des identités certifiées par le nom seul.

Le rapprochement des calendriers associe chacune des **26 livraisons cliniques** au premier acte MRP-42 ultérieur dans le même établissement, parmi les 30 actes répétés. Il retrouve **26 actes distincts chez les huit patients**, avec une arrivée **4,2 à 7,8 jours avant l'acte**. Quatre actes ne sont pas retenus par cette règle. Le calcul, détaillé dans la synthèse transversale, ne fixe pas de délai maximal et conserve les dates originales après conversion explicite. Cette proximité n'est pas un test de coïncidence ni une preuve d'administration : elle ne fournit aucune correspondance entre lot expédié et matériel utilisé.

Les patients répétés sont plus âgés : 71,3 ans en moyenne, contre environ 50 dans les autres groupes. L'écart moyen entre âge chronologique et BIOAGE estimé est de **11,32 ans**, contre **1,10 an** pour les vingt bénéficiaires d'un acte unique et **1,01 an** pour les 212 autres patients. Le calcul donne une valeur moyenne par patient, pour ne pas surpondérer ceux ayant plus de mesures.

Ce contraste soutient une piste de programme particulier dans le récit, **pas une efficacité thérapeutique démontrée**. Les groupes ne sont pas comparables expérimentalement et trois bénéficiaires répétés n'ont aucune mesure BIOAGE antérieure au premier acte. Aucun identifiant de matériel MRP-42 ne correspond directement à un identifiant de lot réceptionné dans le champ comparé. Les trois actes d'Elira Vaun précèdent le décès public de 2021 : ils n'étayent pas une intervention post mortem.

Sources : `clinical_procedures.csv`, `clinical_observations.csv`, `patient_administration.csv`, licences, nominations publiques et déclarations de dirigeants.

## 5. Le réseau s'inscrit dans un récit d'identités et de stratégies concurrentes

Les notes **CLN-510027**, **CLN-510055** et **CLN-510064** décrivent des particularités physiologiques ou de capture. Elles ne définissent pas à elles seules une espèce. **CLN-510025** affirme un lien entre PAT-31065 et **Elias Voss**. Le registre confirme qu'Elias Voss préside Meridian, mais la fiche Health affiche **Corin Hallen, né en 1975**, tandis que le dirigeant est enregistré avec une naissance en **1961** et une autre fonction. L'identité documentaire n'est donc pas reproduite par une égalité des attributs structurés.

Les sources **PUB-510043**, **PUB-510076** et **PUB-510044** suggèrent des continuités d'alias et d'associations historiques, notamment autour d'Adrian Vosmere, d'Elias Voss et de Jacob Vale. Cela reste une piste : noms, adresses de correspondance et formulations récurrentes ne prouvent pas une longévité exceptionnelle. **CLN-510126** fournit aussi un contre-exemple clinique où une hypothèse de double structure est rejetée après repositionnement.

Les minutes de 1962 (**PUB-510033**) et **PUB-510094** décrivent des stratégies opposées : aménagement de corridors et contrôle de programmes à long terme d'un côté ; opposition à l'extraction, au réchauffement et à la dissimulation de l'autre. Jacob Vale est associé à cette opposition, sans que son identité biologique soit déduite de ses positions.

Enfin, **PUB-510063** nomme une classification restreinte **« Chamaeleonidian »** et évoque un **transfert non terrestre**, avec un appui plus faible pour cette seconde affirmation. C'est un indice explicite du narratif fictif. L'absence d'une destination dans les registres terrestres fournis ne permet pas de démontrer indépendamment un itinéraire extraterrestre, une origine ou une ampleur.

## Conclusion graduée

Le narratif le mieux soutenu est celui d'un **réseau caché lié à des identités publiques et à des intérêts de long terme**, qui s'appuie sur des infrastructures écologiques, logistiques et cliniques. Le circuit Horizon–Meridian–Asterion est documenté ; les textes y ajoutent une gouvernance Unwabu–CHAMELEO, une consommation alléguée de chauves-souris, un programme clinique sélectif et une population dissimulée qualifiée de Chamaeleonidian. Ils suggèrent un conflit de stratégies sur l'environnement et la divulgation.

Nous nous rapprochons ainsi nettement du **narratif demandé par la consigne**. Nous n'avons pas identifié une phrase chiffrée à décoder. Restent non démontrés : la continuité matérielle d'un lot jusqu'à un patient, le mécanisme et l'efficacité de MRP-42, les égalités d'identités historiques, l'identification physique d'Unwabu, et la réalité précise du transfert extérieur.

Pour la discussion collective, les priorités sont de rechercher une table de correspondance entre lots et matériel clinique, de vérifier les dates contradictoires et les attributs d'identité, et de rechercher des sources indépendantes pour les allégations les plus fortes. Les documents narratifs ne sont pas automatiquement des observations indépendantes : ils peuvent partager les mêmes sources.

Assistance utilisée : proposition et correction de code, exploration des recoupements et rédaction assistées par IA. Les résultats calculés ont été réexécutés ; les incertitudes et les contre-exemples restent visibles.
