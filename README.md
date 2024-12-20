
# Real Estate Market Analysis

## Introduction

Ce dépôt contient une analyse du marché immobilier (projet: Real Estate Market Analysis with Python Project), réalisée dans le cadre du projet du cours sur 365datascience.com. L'analyse vise à fournir des informations sur les tendances des biens immobiliers, la démographie des clients et la tarification à l'aide de diverses techniques de visualisation. Ce projet a été implémenté en Python à l'aide de bibliothèques de science des données populaires telles que Pandas, NumPy et Seaborn. Le projet a été initialement réalisé dans Google Colab, avec l'ensemble de données fourni par 365 Data Science, et un notebook Kaggle lié a également été publié pour l'engagement communautaire.

## Aperçu du Projet

Le projet comprend les étapes clés suivantes :

1. **Chargement des Bibliothèques et des Données** : Nous commençons par importer les bibliothèques Python nécessaires à l'analyse et à la visualisation des données, y compris Pandas, NumPy et Seaborn. Nous chargeons ensuite les ensembles de données des propriétés immobilières et des clients fournis par 365 Data Science.

2. **Nettoyage et Prétraitement des Données** : Nous nettoyons les ensembles de données en supprimant les colonnes inutiles et en gérant les valeurs manquantes. Le processus de nettoyage garantit que l'analyse est précise et exempte d'incohérences.

   - Par exemple, la colonne **'Unnamed: 0'** qui n'avait pas de valeur informative a été supprimée.
   - Les valeurs manquantes ont été traitées pour s'assurer que l'analyse future soit significative et exacte.

3. **Analyse Exploratoire des Données (EDA)** : L'étape de l'EDA consiste à analyser différents attributs des propriétés, tels que le prix, la localisation, et le type, ainsi que la démographie des clients. Pendant cette phase, plusieurs techniques de visualisation sont utilisées pour explorer les relations et les motifs au sein des données.

   - **Average Deal Satisfaction by Country** : Un histogramme a été utilisé pour représenter la distribution des prix. Cela nous a permis de visualiser la répartition des biens abordables par rapport aux biens haut de gamme. La plupart des biens se situent dans une gamme de prix moyenne, mais nous avons aussi observé quelques valeurs aberrantes très élevées.

     ![Average Deal Satisfaction by Country](images/Average_Deal_Satisfaction_by_Country.png)
     
     Cet histogramme montre que la majorité des propriétés se situent dans une fourchette de prix abordable, tandis que quelques-unes sont nettement plus chères, indiquant des biens haut de gamme.

   - **Revenue Distribution by State** : Nous avons utilisé des cartes de chaleur pour représenter les tendances par localisation. Cela nous a permis de voir les régions les plus attractives en termes de nombre de biens et de prix moyens. Les régions urbaines tendent à avoir des prix plus élevés par rapport aux régions rurales.

     ![Revenue Distribution by State](images/Revenue_Distribution_by_State.png)
     
     La carte de chaleur ci-dessus illustre les différences de prix moyens par région, avec des zones urbaines affichant des prix plus élevés, ce qui est cohérent avec la demande plus forte dans ces zones.

4. **Visualisation** : Différents types de graphiques, tels que les diagrammes à barres, les graphiques de dispersion et les cartes de chaleur, ont été utilisés pour comprendre les tendances du marché immobilier, les distributions de prix et les corrélations entre les différentes caractéristiques.

   - **Correlation Heatmap** : Une carte de chaleur de corrélation a été créée pour étudier la relation entre les variables du jeu de données. Par exemple, nous avons trouvé une forte corrélation positive entre la superficie et le prix des propriétés. Cela montre que plus une propriété est grande, plus son prix est élevé.

     ![Correlation Heatmap](images/Correlation_Heatmap.png)
     
     Cette carte de chaleur montre les relations entre différentes caractéristiques des propriétés. Par exemple, la corrélation élevée entre la superficie et le prix indique que la taille est un facteur déterminant du prix.

   - **Age Distribution of Customers** : Les diagrammes à barres ont été utilisés pour représenter la démographie des clients, telles que leur tranche d'âge et leur revenu moyen. Cela nous a permis d'identifier que la majorité des clients cherchant à acheter des propriétés appartiennent à la tranche d'âge 30-45 ans.

     ![Age Distribution of Customers](images/Age_Distribution_of_Customers.png)
     
     Le diagramme ci-dessus montre que la plupart des acheteurs de biens immobiliers sont des adultes entre 30 et 45 ans, ce qui est typique pour les personnes établissant une maison familiale.

   - **Revenue by Building Type Over Time** : Ce graphique de ligne montre les revenus par type de bâtiment au fil du temps. Chaque ligne représente un type de bâtiment et son évolution des ventes au cours des années. Cela nous permet d'identifier les tendances de revenus par type de bâtiment et de voir comment elles varient sur différentes périodes.

     ![Revenue by Building Type Over Time](images/Revenue_by_Building_Type_Over_Time.png)
     
     Le graphique ci-dessus montre que les revenus fluctuent de manière significative selon le type de bâtiment, certaines années affichant des pics marqués pour certains types de bâtiments. Cela peut indiquer des événements économiques spécifiques ou des variations dans la demande du marché.


## Vidéo Explicative

[![Voire le video](images/videoCover.png)](https://drive.google.com/file/d/1UEgGvjnuhrchRZpOys3xLW6dEipQznNW/view?usp=sharing)


## Notebook Kaggle

Le projet est également disponible sur Kaggle, où vous pouvez explorer le notebook et interagir avec les données. Le notebook Kaggle est accessible https://www.kaggle.com/code/nacernacer/real-estate-market-analysis-project 

## Comment Utiliser ce Dépôt

1. **Cloner le Dépôt** : Utilisez la commande suivante pour cloner le dépôt :
   ```
   git clone https://github.com/elbasri/REM_Analysis.git
   ```
2. **Installer les Dépendances** : Assurez-vous d'avoir Python 3.x installé, ainsi que Pandas, NumPy, Seaborn et Matplotlib. Ces bibliothèques peuvent être installées via pip :
   ```
   pip install pandas numpy seaborn matplotlib
   ```
3. **Exécuter le Notebook** : Vous pouvez ouvrir et exécuter le notebook Jupyter en utilisant n'importe quel environnement compatible avec Jupyter, tel que Jupyter Notebook, JupyterLab ou Google Colab. sinon vous pouvez utiliser le kaggle notebook pour creer votre (https://www.kaggle.com/code/nacernacer/real-estate-market-analysis-project)


## Références

- [365 Data Science Projects](https://learn.365datascience.com/projects/) : Ce projet a été créé dans le cadre de l'offre de cours de 365 Data Science, qui propose une variété de projets de science des données pour un apprentissage pratique.
- **Concepts de Visualisation des Données** : Les techniques de visualisation clés, telles que les diagrammes à barres, les graphiques de dispersion et les cartes de chaleur de corrélation, sont cruciales pour comprendre les relations entre les variables dans l'ensemble de données. Pour plus d'informations sur ces techniques, consultez la [documentation Seaborn](https://seaborn.pydata.org/) et la [documentation Matplotlib](https://matplotlib.org/).
