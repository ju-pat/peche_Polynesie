# peche_Polynesie
Le code de notre projet de M2-MSV concernant des données de captures de pêche en Polynésie française.

Ces codes utilisent des bases de données transformées : Data_R_total.csv

### Pour les modèles GLM : fichier *GLM.Rmd*
Il contient :
- différents GLM entraînés, leurs performances, avec la possibilité de choisir la variable réponse et des changer les variables explicatives
- des visualisations descriptives du jeu de données

### Pour les RF : fichier *RandomForest.ipynb*
Il contient :
- une phase de preprocessing avec la possibilité de choisir la variable réponse et des changer les variables explicatives (cf rapport, possible de modéliser une espèce par les autres)
- une pipeline complète d'entraînement de 3 RF différents
- des visualisations des variables importantes et d'arbres simples de décision
- une méthode de fine-tuning avec optuna et de cross-validation

