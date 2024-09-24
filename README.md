# Lab : Étude de l'Approximation Universelle dans les Réseaux de Neurones

## 🧠 Objectif   
L'objectif de ce laboratoire est d'étudier une propriété fondamentale des réseaux de neurones statiques (non récurrents) : **l'approximation universelle**. Cette propriété permet aux réseaux de neurones, même avec une seule couche cachée, d'approximer n'importe quelle fonction continue avec suffisamment de neurones.

Dans ce lab, nous entraînons un Multi-Layer Perceptron (MLP) avec une seule couche cachée sur une fonction définie par morceaux. Nous analysons ensuite comment le réseau approxime cette fonction.

## 📊 Étapes du Lab
### 1. Génération des Données

- La fonction f(x) est définie comme suit :
𝑓(𝑥)={
sin(𝜋𝑥) si 𝑥∈[−1,1[
0 si 𝑥∈[−2,−1]∪[1,2]
- Ajout d'un bruit normal N(0,0.2) aux données générées.   
- Génération de multiples échantillons d'entraînement et de test à partir de cette fonction.

### 2. Implémentation de MLP avec TensorFlow

- Utilisation d'un MLP simple avec une seule couche cachée pour approximer la fonction générée.
- Exploration de différentes architectures avec un nombre de neurones cachés variant (par exemple, 1, 3, 5, 7 neurones).
  
### 3. Recommandations

- Analyse des résultats : Démarrez avec un petit nombre de neurones et observez comment l'approximation de la fonction évolue.
- Variations : Testez différentes configurations de neurones dans la couche cachée pour observer comment l'approximation devient plus ou moins "sparse" en fonction de la capacité du modèle.
- Évaluation des performances : Testez la généralisation du modèle en évaluant ses performances sur un ensemble de test.

## 🛠️ Technologies Utilisées  
- `Python` : Langage de programmation principal pour l'implémentation.   
- `TensorFlow` : Framework pour la création et l'entraînement du réseau de neurones MLP.
- `NumPy` : Pour la génération et la manipulation des données.
- `Matplotlib` : Pour visualiser les approximations des fonctions.
