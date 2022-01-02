# Prédiction d'approbation de micro crédit



# Demo

[link](https://#)   [![Website perso.crans.org](https://img.shields.io/website-up-down-green-red/http/perso.crans.org.svg)](http://perso.crans.org/)

[App Micro Prêt] https://github.com/skyclanlourro/micro-pret.git

# Contenu

Une demande de prêt est utilisée par les emprunteurs pour demander un prêt. 
Grâce à la demande de prêt, les emprunteurs révèlent au prêteur des détails clés sur leurs finances. 
La demande de prêt est cruciale pour déterminer si le prêteur accordera la demande de fonds ou de crédit.

# Énoncé du problème

Le directeur de la banque SZE a identifié que parcourir les demandes de prêt pour filtrer les personnes qui peuvent obtenir
des prêts ou qui doivent être rejetées est un processus fastidieux et long. Il veut l'automatiser et augmenter l'efficacité de sa banque.
Le directeur de la banque LE-MAL a identifié que parcourir les demandes de prêt pour filtrer les personnes qui peuvent obtenir des prêts
ou qui doivent être rejetés est un processus fastidieux et long.
Après avoir discuté un peu, vos noms apparaîssent comme les rares scientifiques des données qui peuvent rendre cela possible dans un temps limité. 
Aiderez-vous alors le Directeur ?

# Objectif

L'idée derrière ce projet de ML est de créer un modèle de ML et une application Web que la banque pourra utiliser pour classer 
si un utilisateur peut obtenir un prêt ou non.

# Critère d'évaluation

Les soumissions sont évaluées à l'aide du F1 score.

# Données

## À propos des données
L'ensemble de données contient des informations sur les demandeurs de prêt. 
Il y a 12 colonnes indépendantes et 1 colonne dépendante. 
Cet ensemble de données comprend des attributs tels que l'ID de prêt, le sexe, si le demandeur de prêt est marié ou non, le niveau d'éducation, 
le revenu du demandeur, etc.

Pour charger les données d'entraînement dans votre notebook jupyter, utilisez la commande ci-dessous :
```
import pandas as pd
```
```
Loan_data = pd.read_csv("https://raw.githubusercontent.com/dphi-official/Datasets/master/Loan_Data/loan_train.csv" )
```

## Description des données

* Loan_ID : Un identifiant unique attribué à chaque demandeur de prêt
* Sexe: Sexe du demandeur (Homme, Femme)
* Marié : L'état matrimonial du demandeur (Oui, Non)
* Personnes à charge : Nombre de personnes à charge du demandeur (0,1,2,3+)
* Éducation: Niveau d'éducation du candidat (Diplômé, Non Diplômé)
* Self_Employed : Si le demandeur est travailleur indépendant (Oui, Non)
* Revenu du demandeur : le montant du revenu que le demandeur gagne
* Revenu du codemandeur : le montant du revenu que le codemandeur gagne
* LoanAmount : Le montant du prêt que le demandeur a demandé
* Loan_Amount_Term : nombre de jours pendant lesquels le prêt sera payé
* Credit_History : un enregistrement du remboursement responsable des dettes d'un emprunteur (1- toutes les dettes sont payées, 0- non payées)
* Property_Area : Le type d'emplacement où se trouve la propriété du demandeur (Rural, Semi-urbain, Urbain)

Cibler :

* Loan_Status : Prêt accordé ou non (Oui, Non)



## Tester l'ensemble de données

Chargez les données de test (nommez-les test_data). Vous pouvez charger les données en utilisant la commande ci-dessous.
```
test_data = pd.read_csv('https://raw.githubusercontent.com/dphi-official/Datasets/master/Loan_Data/loan_test.csv')
```
Ici, la colonne cible n'est délibérément pas là car vous devez la prédire.


# Auteur

[Nyam](https://github.com/skyclanlourro)
