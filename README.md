# Naive-Bayes-classifier  vs  Tree-Augmented-Naive-Bayes-classifier

L’inférence probabiliste est devenue une technologie de base en IA, en grande partie grâce aux
développements des méthodes de la théorie des graphes pour la représentation et la
manipulation des distributions de probabilités complexes (Pearl, 1988)

## Les modèles graphiques probabilistes 

**1 Dirigé: Bayes Networks.   
 2 Non dirigé Markov random fields**
Permettre une séparation entre les aspects qualitatifs et
structurels et les aspects quantitatifs et paramétriques dans la
modélisation de l’incertitude.  
**1 Repréesentés via les patterns des arêtes dans le graphe 
  2 Repréesentés sous forme de valeurs numériques associées à  
des sous-ensembles de nœuds dans le graphe.**  

**Objectif: Naives Bayes Classifier Tree Augmented
Naive Bayes : Caractéristiques– Pouvoir prédictif**
PimaIndiansDiabetes : 768 observations de 9 variables –
Prédire la variable "outcome".   
iris : 150 observations de 5 variables – Prédire la variable  
"Species".
Algorithmes très populaires dans le domaine de la santé :
segmentation d’images et le diagnostic médical / Finance:
classification, détection de fraude.  

### Naives Bayes Classifier
Caractéeristique : très forte hypothèse d’indépendance.
**¤ Bayésien: utilise le théorème de Bayes pour calculer la
probabilité conditionnelle    
¤ Naive: il assume une indépendance entre les features
conditionnellement au label ce qui n’est pas forcement
établi.**

## TAN: Tree augmented Naif Bayes Classifier 
Une extension du classifier Naive Bayes en assouplissant
l’hypothèse de l’indépendance.
Prise en compte des corrélations entre les features
Maintenir la structure du graphe NB et l’augmente en
ajoutant des arêtes entre les variables
chaque variable peut avoir deux parents qui sont le nœud
de la classe et un autre nœud de variable, à l’exception de
la variable racine.  
L’information mutuelle : Pour construire l’arbre, il est
obligatoire de mesurer la corrélation entre chaque paire de
variables dans les données et ajouter des arêtes uniquement
entre les variables les plus corrélées. 
Concrètement: N variables ==> N nœuds ==> N-1 arêtes
à ajouter
La somme des poids de toutes ces arêtes = le poids
maximum parmi toutes ces structures.

