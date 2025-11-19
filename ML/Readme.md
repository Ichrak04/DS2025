
[pip install ucimlrepo from ucimlrepo import fetch_.md](https://github.com/user-attachments/files/23631819/pip.install.ucimlrepo.from.ucimlrepo.import.fetch_.md)
<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" style="height:64px;margin-right:32px"/>

# pip install ucimlrepo from ucimlrepo import fetch_ucirepo

# fetch dataset

wine_quality = fetch_ucirepo(id=186)

# data (as pandas dataframes)

X = wine_quality.data.features
y = wine_quality.data.targets

# metadata

print(wine_quality.metadata)

# variable information

print(wine_quality.variables)
donne moi un compte rendu  sous format markdown

Voici un compte rendu du dataset "Wine Quality" (ID 186) obtenu avec le package ucimlrepo, résumé sous format Markdown:[^1][^2][^3][^4]

***

# Compte Rendu : Wine Quality (UCI ID 186)

## Présentation du Dataset

Ce jeu de données regroupe les propriétés physico-chimiques de vins portugais "Vinho Verde" (rouge et blanc), collectées pour prédire la qualité du vin. Il est composé de deux fichiers (rouge et blanc) et inclut à la fois des données de laboratoire (caractéristiques du vin) et des données sensorielles (évaluation qualité par des experts).[^2][^4]

- **Source :** UCI Machine Learning Repository
- **Objectif :** Modélisation de la qualité basée sur les mesures physico-chimiques.[^2]
- **Type de tâche :** Classification ou régression (la variable cible est ordonnée mais déséquilibrée).[^4]
- **Instances représentées :** Échantillons de vin avec scores de qualité de 0 à 10.


## Variables du Dataset

Le dataset contient 12 variables principales (11 features et 1 cible):[^3][^4][^2]


| Nom de la Variable | Rôle | Type | Description |
| :-- | :-- | :-- | :-- |
| fixed_acidity | Feature | continue | Acidité fixée |
| volatile_acidity | Feature | continue | Acidité volatile |
| citric_acid | Feature | continue | Acide citrique |
| residual_sugar | Feature | continue | Sucres résiduels |
| chlorides | Feature | continue | Chlorures |
| free_sulfur_dioxide | Feature | continue | SO2 libre |
| total_sulfur_dioxide | Feature | continue | SO2 total |
| density | Feature | continue | Densité |
| pH | Feature | continue | Potentiel Hydrogène (pH) |
| sulphates | Feature | continue | Sulfates |
| alcohol | Feature | continue | Teneur en alcool |
| quality | Target | ordinal | Score qualité (0 à 10, mesuré par experts) |

*Pas de valeurs manquantes officielles, mais quelques valeurs supprimées ou modifiées lors du preprocessing*.[^4]

## Exemples de Manipulation avec ucimlrepo

- Installation : `pip install ucimlrepo`
- Chargement :

```python
from ucimlrepo import fetch_ucirepo
wine_quality = fetch_ucirepo(id=186)
X = wine_quality.data.features
y = wine_quality.data.targets
print(wine_quality.metadata)
print(wine_quality.variables)
```


## Points à explorer dans l'analyse

- **Répartition de la qualité** : La plupart des vins sont évalués entre 5 et 6, les rouges ayant une distribution plus étalée.[^5]
- **Corrélation des variables** : L'alcool et l'acidité volatile montrent une forte association avec la qualité mesurée.[^6]
- **Usage du dataset** : Convient à des méthodes de classification (qualité "bonne/mauvaise") ou de régression.[^7][^5]
- **Prétraitement** : Certains travaux appliquent des techniques d’équilibrage comme SMOTE pour améliorer la représentativité des classes minoritaires.[^5]


## Bibliographie

- Cortez et al., « Modeling wine preferences by data mining from physicochemical properties », Decision Support Systems, 2009.[^2][^4]
- UCI ML Repository : [Wine Quality Dataset](https://archive.ics.uci.edu/dataset/186/wine+quality).[^2]

***

Ce résumé combine les informations sur la structure, le contenu, les variables, et l'usage typique du jeu de données "Wine Quality" telles qu'utilisées dans les notebooks Python avec ucimlrepo.
<span style="display:none">[^10][^11][^12][^13][^14][^15][^16][^17][^18][^19][^20][^8][^9]</span>

<div align="center">⁂</div>

[^1]: ML.ipynb

[^2]: https://archive.ics.uci.edu/dataset/186/wine+quality

[^3]: https://codesignal.com/learn/courses/introduction-to-supervised-machine-learning/lessons/diving-into-the-wine-quality-dataset-an-in-depth-overview

[^4]: https://www.scribd.com/document/409574374/Data-Set-Information-WINE-QUALITY

[^5]: https://github.com/ujvarafetoshi/wine-quality-deep-learning

[^6]: https://joekusuma.com/wine-quality-dataset/

[^7]: https://www.kaggle.com/datasets/arnavs19/wine-quality-uci-machine-learning-repository

[^8]: https://archive.ics.uci.edu/dataset/109/wine

[^9]: https://www.kaggle.com/datasets/yasserh/wine-quality-dataset

[^10]: https://www.scribd.com/document/920823005/Wine-Quality-Dataset

[^11]: https://github.com/uci-ml-repo/ucimlrepo

[^12]: https://www.kaggle.com/code/taweilo/red-win-dataset-synthetic-process

[^13]: https://deepnote.com/app/maxbm19/Exploratory-Data-Analysis-Wine-Quality-4878db7d-bd7a-41eb-9630-753b4d93c2a4

[^14]: https://towardsdatascience.com/how-to-use-elastic-net-regression-85a6a393222b/

[^15]: https://www.geeksforgeeks.org/machine-learning/wine-quality-prediction-machine-learning/

[^16]: https://www.cliffsnotes.com/study-notes/16855661

[^17]: https://archive.ics.uci.edu

[^18]: https://pypi.org/project/serendipity-matrix/

[^19]: https://gitea1.its.isti.cnr.it/moreo/QuaPy/blame/commit/19524f9aa82a8cb70601009e19d53433cbf8b0e3/quapy/data/datasets.py

[^20]: https://www.kaggle.com/code/gengchensun/notebook33f08dc158

