# Les accidents de la circulation en France : modèle de prévision de la gravité des accidents corporels
Hélène / Orphée


![alt text](http://fastncurious.fr/wp-content/uploads/2017/12/Screenshot-2017-12-27-at-19.53.14.png)

Mini-projet Ironhack Data Analytics DAPT printemps 2021

Lors d'accidents de la route, peut-on prédire la gravité des blessures ?

En France (métropole et DOM-TOM), les forces de l'ordre relèvent des informations sur chaque accident de la circulation si :
- au moins 1 véhicule impliqué
- et au moins 1 victime ayant nécessité des soins. 
---> Bases de données Annuelles des Accidents corporels de la Circulation routière (BAAC), mises à disposition du public sur www.data.gouv.fr et libres d’utilisation. 

Notre étude : la BAAC de l’année 2019, un jeu de données de 132977 lignes / 54 colonnes, ramené après nettoyage à 130901 lignes.
Chaque ligne correspond à l'une des victimes des 58000 accidents de l'année 2019, et fournit des données sur les caractéristiques de l'accident, son lieu, le véhicule impliqué, la victime et la gravité de l'atteinte corporelle.

Cette gravité est codifiée comme suit :
- Indemne
- Blessé Léger (pas de nuit pasée à l'hôpital)
- Blessé Grave (plus de 24h d'hospitalisation)
- Décès sous 30 jours

On a testé 8 algorithmes de classification multi-classes : Random Forest, Logistic Regression, XG Boost, CatBoost, GradientBoosting, LightGBM, Extra-Trees, Perceptron
+ les 4 algorithmes du module Imbalanced-Learn.

Un classeur Tableau est consultable en ligne : https://public.tableau.com/app/profile/h.l.ne.hill/viz

Ce repository github inclut :
- un référentiel du projet et du jeu de données ("codebook")
- le code sous plusieurs notebooks Jupyter.
- le Pandas Profile Report du jeu de données.

Le jeu de données est téléchargeable sur data.gouv.fr : https://www.data.gouv.fr/fr/datasets/bases-de-donnees-annuelles-des-accidents-corporels-de-la-circulation-routiere-annees-de-2005-a-2019/
