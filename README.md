# peche_Polynesie
Le code de notre projet de M2-MSV concernant des données de captures de pêche en Polynésie française.

Ces codes utilisent des fichiers et bases de données transformées.
### Pour les ACP : fichier *ACP github.Rmd*
Utilise : Data_R.csv
Il contient : 
- Une phase d'étude des corrélation
- Une phase d'étude de l'ACP
- Une phase de tentative de coloration de l'ACP par différentes grandeurs (présentées dans le rapport)
### Pour les modèles GLM : fichier *GLM.Rmd*
Utilise : Data_R_total.csv

Il contient :
- différents GLM entraînés, leurs performances, avec la possibilité de choisir la variable réponse et des changer les variables explicatives
- des visualisations descriptives du jeu de données

### Pour les RF : fichier *RandomForest.ipynb*
Utilise : Data_R_total.csv

Il contient :
- une phase de preprocessing avec la possibilité de choisir la variable réponse et des changer les variables explicatives (cf rapport, possible de modéliser une espèce par les autres)
- une pipeline complète d'entraînement de 3 RF différents
- des visualisations des variables importantes et d'arbres simples de décision
- une méthode de fine-tuning avec optuna et de cross-validation

### Pour la création d'une base de données compacte et les visualisations en clustermap : fichier *Etude_des_compositions.ipynb*
Utilise : Lev2-SortiesPeches, Lev3_CompoPrises, trackClassification_by_Coast.csv, trackClassification_by_habitat.csv, trackClassification_by_passToPass.csv, trackClassification_by_village.csv

Il contient :
- une phase de nettoyage des données et de reliage des bases de données sur les sorties et sur les captures
- création de la base de données compacte, avec notamment sélection d'une zone géographique par sortie pour chaque type de découpage géographique
Les autres parties contiennent certains résultats non concluants, mais les méthodes et outils restent intéressants et ont constitués une importante partie d'exploration des données
- différentes clustermap (plus ou moins concluantes, cf rapport)
- une étude descriptive plus spécifique aux nombres d'espèces pêchées par sortie en fonction de la technique et de l'habitat

### Pour les PLN : fichier *PLN github.Rmb*
Utilise : Data_R_total.csv
Il contient :
- une Phase de preprocessing des données 
- une Phase de création de fonctions utiles au plot des données
- les codes menant au plot du rapport 
