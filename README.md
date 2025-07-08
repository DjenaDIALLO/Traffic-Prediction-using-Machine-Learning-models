# Traffic-Prediction-using-Machine-Learning-models
Dans ce notebook, j'analyse et prédis la situation du trafic en utilisant différentes techniques de Machine Learning.

Base de données utilisée :

J'ai utilisé le jeu de données "Traffic Prediction Dataset" que j'ai trouvé sur Kaggle (https://www.kaggle.com/datasets/hasibullahaman/traffic-prediction-dataset). Ce dataset contient des informations sur le trafic, comme l'heure, la date, le jour de la semaine, le nombre de différents véhicules (voitures, motos, bus, camions) et la situation générale du trafic.

##Étapes:

Analyse Exploratoire des Données (EDA) : J'ai commencé par charger le jeu de données, vérifier s'il y avait des valeurs manquantes et visualiser comment la variable que je veux prédire ("Traffic Situation") est distribuée.
Prétraitement des Données : J'ai formaté les colonnes de temps et celles qui contiennent des catégories ('Time', 'Day of the week', 'Traffic Situation') pour les transformer en nombres, ce qui est nécessaire pour l'analyse.
Sélection des Caractéristiques : J'ai utilisé une matrice de corrélation pour voir les relations entre les différentes variables dans le dataset.
Standardisation des Données : J'ai appliqué une standardisation sur les colonnes numériques importantes ('Time', 'Date', 'CarCount', 'BikeCount', 'BusCount', 'TruckCount') pour que leurs valeurs soient sur la même échelle.
Division des Données : J'ai divisé le jeu de données en deux parties : une pour entraîner les modèles et une autre pour les tester.
Construction de Modèles de Machine Learning :
Modèles de Régression : J'ai construit et évalué des modèles comme la régression linéaire, Ridge, Lasso et Elastic Net pour voir s'ils pouvaient prédire une valeur continue.
Modèles de Classification : J'ai ensuite construit et évalué plusieurs modèles de classification pour prédire la catégorie de la situation du trafic (basse, normale, élevée, forte). J'ai testé la Régression Logistique, K-Nearest Neighbours, Bagging, Boosting, Support Vector Machine, Decision Tree Classifier et Random Forest Classifier.
Tuning des Modèles : J'ai affiné les paramètres de certains modèles de classification en utilisant GridSearchCV pour essayer d'améliorer leurs performances.
Analyse des Résultats : Enfin, j'ai comparé les performances (précision sur les données d'entraînement et de test) de tous les modèles dans un tableau et un graphique. Cela m'a permis de voir quels modèles étaient les meilleurs pour prédire la situation du trafic.
En conclusion, après avoir exploré et préparé les données, construit et évalué différents modèles, j'ai constaté que les modèles de classification, en particulier Boosting et Random Forest Classifier, sont ceux qui donnent les prédictions les plus précises pour ce problème de classification de la situation du trafic.
