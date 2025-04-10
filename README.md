# PyConso
Etude de la consommation d'électricité en France de 2013 à 2021

LE PROJET  PYCONSO chez Datascientest

Dans le cadre de notre projet fil rouge, PyConso, nous nous sommes fixés trois objectifs : 
Comparer la consommation d’énergie en France par rapport à sa production
Comparer les filières de production : nucléaire et renouvelables.
Construire un modèle de prédiction robuste de la consommation d’énergie régionale à différentes échelles de temps
Notre étude s’est basée sur l’analyse d’un jeu de données issues des enregistrements par le RTE, disponible en libre accès sur : https://opendata.reseaux-energies.fr/explore/dataset/eco2mix-national-cons-def/export/?disjunctive.nature. Les données ont été enregistrées de janvier 2013 à février 2022 pour toutes les régions métropolitaines. 
 Nous avons ajouté à ces données des données complémentaires issues de différentes sources, potentiellement explicatives de la consommation d’énergie afin de construire un modèle de ML robuste et performant pour la prédiction de cette variable cible.
Nous nous sommes donc posé la question suivante : de quelles variables dépend la consommation électrique en France ? 
Au niveau national mais également au niveau régional, on suppose qu’elle est d’abord logiquement fonction des caractéristiques saisonnières, avec une forte thermo sensibilité en hiver (en lien avec l’utilisation des chauffages) et dans une moindre mesure en été. On a donc sélectionné tout un panel de variables environnementales dont les fluctuations dépendent fortement des saisons ainsi que des variables indicatrices de l’utilisation d’électricité pour le chauffage ou le refroidissement. 
Au niveau local, on suppose que la consommation est également dépendante des cycles d’activités horo-hebdomadaires avec notamment une moindre demande la nuit et les week-ends. On a donc sélectionné des variables en lien avec la densité de population, les secteurs d’activité de la région et les besoins en électricité des transports. On a également intégré des variables en lien avec la baisse d’activité globale : vacances, jours fériés et périodes de confinement.
De plus, la production dépendant évidemment de la consommation, on s’est demandé de quelles filières dépendaient chaque région et on a souhaité comparer la production à la consommation régionale afin de mieux appréhender les problèmes qui risquent de se poser au niveau local.
Pour répondre à nos différents objectifs nous avons suivi les étapes suivantes :
Exploration des données : comprendre les observations et les variables
Preprocessing : préparer les données pour être exploitées
Data Visualisation 
Modélisation
