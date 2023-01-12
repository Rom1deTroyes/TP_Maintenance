# But de l'exécutable
Cette fonction a pour but d'évaluer les prédictions faites par un modèle de classification binaire sur un des jeux de données fournies. Il ne fonctionne que sur Windows ; si vous utilisez un autre système d'exploitation, vous devrez m'envoyer vos fichiers csv de prédictions pour que je vous donne les scores obtenus. 

# Instructions d'usage
Dans un fichier de commande, entrez les instructions :
```> evaluate_score.exe chemin_vers_le_fichier_csv_de_predictions nom_du_dataset```
avec :
- ```chemin_vers_le_fichier_csv_de_predictions``` : chemin vers un fichier csv contenant toutes les prédictions, au format suivant :
image_name,label
0.jpg,Cat
1.jpg,Cat
2.jpg,Dog
etc.
- ```nom_du_dataset : nom du dataset concerné```, c'est à dire "dataset1", "dataset2", "dataset3", ou "dataset4"

# Format de sortie
Les scores sont écrits dans un fichier csv, placé dans le même dossier que ```chemin_vers_le_fichier_csv_de_predictions```, et nommé ```Ymd_HMS_scores.csv``` (avec ```Y``` l'année, ```m``` le mois, ```d``` le jour, ```H``` l'heure, ```M``` les minutes et ```S``` les secondes courants à l'exécution de la fonction).