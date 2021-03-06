
.. _l-projinfo2a:

2A - Projets informatiques - Data Scientist - Economiste
========================================================

.. contents::
    :local:

**Dates de rendu**

* dernier jour avant les vacances de Noël pour le rapport / notebook / programme
* premières semaines de janvier pour la soutenance

Data Scientist
++++++++++++++

Le projet informatique sera centré sur la résolution d'un problème de
machine learning à partir d'un jeu de données préparé à cet effet.
Le choix du sujet est libre et vous trouverez une liste de suggestions à
:ref:`l-datasources`.

Le site
`Kaggle <https://www.kaggle.com/competitions/search?SearchVisibility=AllCompetitions&ShowActive=true&ShowCompleted=true&ShowProspect=true&ShowOpenToAll=true&ShowPrivate=true&ShowLimited=true&DeadlineColumnSort=Descending>`_ `(2) <http://inclass.kaggle.com/>`_
référence de nombreuses compétitions intéressantes.
Toutefois, avant d'utiliser les données Kaggle, je vous encourage à lire les articles
`Date use for teaching after competition concludes <http://www.kaggle.com/c/decoding-the-human-brain/forums/t/8331/date-use-for-teaching-after-competition-concludes>`_
et `Using a Kaggle contest as a term project <http://www.kaggle.com/forums/t/2745/using-a-kaggle-contest-as-a-term-project>`_.
Les règles peuvent varier d'un projet à l'autre, prenez soin de les lire avant de choisir un projet
car on ne peut pas tout faire avec les données disponibles sur ce site.

Les publications scientifiques mettent parfois leurs données à dispositions :

* `Patient Risk Stratiﬁcation with Time-Varying Parameters: A Multitask Learning Approach <http://www.jmlr.org/papers/volume17/15-177/15-177.pdf>`_
* `Trend Filtering on Graphs <http://www.jmlr.org/papers/volume17/15-147/15-147.pdf>`_

Travail attendu
+++++++++++++++

On vous demande de vous poser une problématique et d'y répondre en utilisant des données.
Le projet est orienté plus machine learning pour les data scientist,
plus qualitatif et collecte de données pour les économistes.

* Rapport + code (PDF, Notebook, HTML)
  il peut être converti au format PDF ou HTML avec `nbconvert <https://nbconvert.readthedocs.io/en/latest/>`_ et Latex).
  Si le rapport n'est pas un notebook, il faudra indiquer la fonction à l'origine de chaque table ou graphique.
* Une introduction : quel est le problème à résoudre, les questions auxquelles on cherche à répondre, un aperçu des données.
* Une attention particulière sur la rigueur de la démarche (base d'apprentissage / test,
  overfitting, validation croisée, vérification sur quelques exemples,
  type de variable - continues, discrètes, catégorielles).
* On pourra également souligner le raisonnement ou l'intuition qui vous amène
  à essayer tel modèle, tel feature, telle méthode.
* La présence d'au moins un graphique.
* Une conclusion : le modèle, les résultats sont-ils exploitables ?
* Soutenance

**data scientist**

* La comparaison de deux modèles sur le même jeu de données (soit deux modèles différents,
  soit le même modèle avec des paramètres différents), on s'intéressera aux observations
  pour lesquelles les modèles sont en désaccords. On pourra également comparer
  les vitesse d'apprentissages et les performances.
* L'ajout d'une variable/feature non présente dans le jeu de données initial
  (cela peut être une combinaison des précédentes).
* Prolongements / perspectives : le problème à résoudre est souvent extrait de son contexte,
  il s'agit de le replacer dans un environnement industriel. Cela peut passer par
  une réflexion autour des questions suivantes (qui ne s'appliquent pas forcément à tous les jeux de données).

Les questions à se poser :

* Le modèle est-il exploitable avec ses performances ?
* Est-il exploitable seul ou associé à autre chose (est-il une feature d'un autre modèle) ?
* Quel est sa durée de vie ? Ses performances vont-elle se dégrader dans le temps ? Peut-on le détecter ?
* Le modèle peut-il passer à l'échelle et être entraîné sur des jeux 10, 100, 1000 fois plus grand ?
* Certaines variables/information sont coûteuses à obtenir,
  est-il envisageable de faire moins coûteux sans trop de perte de performances ?
* Doit-il être maintenu, rafraîchi, à quel coût ?
* Si le modèle doit être rafraîchi régulèrement, le modèle peut-il être utilisé
  voire réappris sans intervention humaine ?
* Si le modèle est rafraîchi régulièrement et automatique,
  serai-il facile de détecter qu'une mise à jour a échoué ?
* Lorsque l'apprentissage est long et coûteux, l'estimation d'un nouveau
  modèle pourrait-elle être faite à partir de la précédente ou non ?
  (nouvel apprentissage ou simple mise à jour)
* Si vous deviez vendre ce modèle de machine learning, quel modèle économique choisiez-vous ?
  (une application, une extension Excel, un service distant payé à chaque prédiction,
  une application smartphone, le modèle seulement...)
* Lorsque le modèle se trompe, se trompe-t-il de beaucoup ? Quel serait le coût de l'erreur ?
  Peut-on le réduire ?

**economiste**

Trois dimensions doivent être présentes dans le projet.
Pour chacune de ces parties, il est possible d'aller plus ou moins loin.
Il est recommandé d'aller loin sur au moins une des dimensions.

#. **La récupération de données :**
   Ces données peuvent être directement disponibles sous la forme de fichiers txt, csv ...
   ou provenir de sites internet (scrapping, API).  Plus le travail
   sur la récupération de données est important (par exemple scrapping sur plusieurs
   sites), plus la partie obtiendra de points. En partant des données de
   `IMBD sur les films <http://www.imdb.com/interfaces>`_.
   Vous pouvez récupérer des informations sur les films ressemblants grâce à
   l'API de `Tasktekid <https://www.tastekid.com/>`_ et répondre à la question de
   qu'est ce qui rend des films similaires (le casting, le thème, le réalisateur ...)
#. **Le traitement et l'analyse :**
   La présence de statistiques descriptives est indispensable dans le projet.
   De la description de la base aux premières grandes tendances des données,
   cette partie permet d'avoir une vision globale des données : le lien avec
   la problématique, comment elle permet d'y répondre, quels sont les premiers éléments de réponse...
   Chaque résultat doit être interprété : pas la peine de faire un describe et de ne pas le commenter.
   Vient ensuite la phase de modélisation : un modèle peut être le bienvenu quand des
   statistiques descriptives ne suffisent pas à apporter une solution complète à
   votre problématique. Le modèle importe peu (régression linéaire, random forest ou autre) :
   il doit être approprié et justifié.
#. **La représentation / application :** Là encore, plusieurs niveaux sont envisageables.
   Vous pouvez simplement représenter vos données en utilisant
   :epkg:`matplotlib`, aller plus loin avec :epkg:`seaborn` ou :epkg:`scikit-plot`,
   (voire `D3.js <https://en.wikipedia.org/wiki/D3.js>`_ pour les plus motivés)
   ou encore réaliser une application en :epkg:`Flask`.
   La base d'une bonne visualisation est de trouver le type de graphique adéquat
   pour ce que vous voulez montrer (faut-il un scatter ou un line pour
   représenter une évolution ?) et de le rendre visible : une légende
   qui a du sens, des axes avec des noms etc.

Barème approximatif
+++++++++++++++++++

* rapport : 6 points
* graphiques : 3 points
* prolongements : 3 points
* démarche scientifique : 4 points
* soutenance : 4 points

Le projet doit être réalisé seul ou par groupe de deux, voire trois.
Un des modèles utilisés n'est pas linéaire et n'est pas un arbre de décision.
Chaque membre d'un groupe doit mentionner une contribution personnelle au projet.
La note globale peut être interprétée comme suit :

* *8* : le projet est mauvais,
* *12* : le projet s'est arrête à la comparaison de modèles de
  machine learning,
* *16* : le projet contient une idée originale,
  une analyse intéressantes des résultats,
* *20* : les auteurs ont construit un raisonnement
  qui a abouti à un fait intéressant sur le jeu de données
  de départ.

Liens
+++++

- :ref:`Bien démarrer un projet de machine learning <l-debutermlprojet>`
- `Quelques astuces pour faire du machine learning <http://www.xavierdupre.fr/blog/2014-03-28_nojs.html>`_
- `Using Python to Dive into Signalling Data with CellNOpt and BioServices <http://arxiv.org/abs/1412.6386>`_
- `SPySort: Neuronal Spike Sorting with Python <http://arxiv.org/abs/1412.6383>`_
- `Machine learning isn't Kaggle competitions <http://jvns.ca/blog/2014/06/19/machine-learning-isnt-kaggle-competitions/>`_.
- :ref:`gitnotebookrst`

.. _l-question-projet-2A-ml:

Questions
+++++++++

* :ref:`question_2014_projet_1_2A`
* :ref:`question_2014_projet_2_2A`
* :ref:`question_2014_projet_3_2A`
* :ref:`question_2014_projet_4_2A`
* :ref:`question_2014_projet_5_2A`
* :ref:`question_2014_projet_6_2A`
* :ref:`question_2015_projet_2_2A`
* :ref:`question_projet_2016`

Retours des projets des années précédentes
++++++++++++++++++++++++++++++++++++++++++

* :ref:`l-remarque-2A-2017-2018`
