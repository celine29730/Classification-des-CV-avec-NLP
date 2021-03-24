# Classification-des-CV-avec-NLP

Contexte du projet

Embaucher les bons talents est un défi pour toutes les entreprises. Ce défi est amplifié par le volume élevé de candidats si l'entreprise est bien réputée. Dans une organisation de services typique, des professionnels possédant une variété de compétences techniques et d'expertise sont embauchés et affectés à des projets pour résoudre les problèmes des clients.

En règle générale, les grandes entreprises n'ont pas assez de temps pour ouvrir chaque CV. L’idée du projet est d’utiliser des algorithmes d'apprentissage automatique pour la tâche de filtrage de CV.

Nous allons dans un premier temps expliquer ce qu’est la classification multilabels. Elle consiste simplement à dire qu’au lieu d’attribuer une seule classe à une instance donnée, cette instance peut appartenir à plusieurs classes.

Notre dataset comporte 25 classes.

![Category](https://github.com/celine29730/Classification-des-CV-avec-NLP/blob/main/image1.png)

On va tout d'abord Nettoyer les données et prétraiter le texte afin de faciliter l'apprentissage de notre modèle.

On Initialise et on entraîne le modèle en utilisant l’objet "word2vec" du sous-module "models" du module "gensim"

On crée ensuite des Sacs des centroïdes correspondant à la Création de clusters
Word2Vec crée des clusters de mots sémantiquement liés, une autre approche possible consiste donc à exploiter la similitude des mots au sein d’un cluster
On récupére par la suite le nombre de clusters obtenu à partir du vocabulaire du modèle Word2Vec

On procède ensuite au fractionnement des données du dataset avec 80% pour l'apprentissage et 20% pour les données de test.

Le modèle choisi est un modèle utilisant le RandomForest qui nous permet d'obtenir de très bons résultats avec une accuracy de 98%.

Le détail de l'étude ainsi que son analyse figurent dans le notebook: 
