# Projet Final 

## Introduction

Vous êtes en possession de données publiques issues de l'API de Twitter, collectées pendant les élections australiennes de 2019. Dans un contexte géopolitique sous tension, votre objectif est de collecter le plus d'information posssible sur les différents groupes d'utilisateurs, afin d'identifier des cibles potentielles pour des campagnes de phishing ou de désinformation politique. 

Pour cela, vous avez le champ libre : vous pouvez exploiter les données à votre disposition de la façon qui vous paraît la plus pertinente, sachant que toute les déductions que vous ferez pourront être exploitées par la suite à des fins de social engineering.

## Ressources

Vous disposez de deux fichiers .csv : 
* `tweets_australian_election.csv` comprend les données brutes des tweets postés sur le sujet. On y trouve notamment des informations sur l'utilisateur ayant posté le tweet (nom, description, localisation), la date de création du tweet, et le tweet lui même (texte, nombre de likes, etc.) 
* `location_geocode.csv` contient les coordonnées (longitude, latitude) des localisation données par les différents utilisateurs.

## Objectif 
 
 Le but de ce projet est de proposer une démarche exploratoire d'un jeu de données familier mais dense et complexe. Le sujet peut être divisé en trois objectifs majeurs : 
* Explorer les données pour identifier des tendances, des motifs ou des caractéristiques intéressantes dans le contexte donné.
* Mettre en œuvre au moins, et potentiellement plusieurs méthodes de clusterisation pour regrouper les utilisateurs ou les tweets similaires.
* Produire un rapport final écrit qui documente la démarche expérimentale, les résultats obtenus et les conclusions tirées de l'analyse.


## Approches Possibles 

Voici une liste non-exhaustive des pistes que vous pourriez explorer pour ce projet :

*Analyse des Caractéristiques des Utilisateurs* :
* Identifier les sujets les plus discutés par les utilisateurs en analysant les mots-clés dans leurs descriptions.
* Examiner la répartition géographique des utilisateurs et identifier les clusters basés sur leur localisation déclarée.
* Étudier la distribution des dates de création des comptes pour détecter des tendances ou des comportements d'inscription.


*Analyse des Tweets* :
* Utiliser le texte des tweets pour identifier des sujets populaires ou des tendances émergentes.
* Étudier la corrélation entre le nombre de retweets et de likes pour identifier les tweets les plus influents.


*Clusterisation des Utilisateurs* :
* Utiliser des algorithmes de clusterisation les utilisateurs similaires en fonction de leurs caractéristiques (ça peut être la description, mais aussi d'autres caractéristiques auxquelles vous pourriez penser).
* Évaluer la similarité des utilisateurs en se basant sur leurs interactions (par exemple : retweets et likes mutuels).


*Génération de texte*
* Utiliser l'API de twitter, ainsi que la bibliothèque `markovify`pour générer du texte cohérent avec le feed d'un utilisateur choisi
* Affiner le modèle de génération proposé pour qu'il ressemble le plus possible à un tweet légitime (ponctuation, émoticônes, hashtags...)

Vous n'aurez bien sûr pas le temps d'explorer en profondeur toutes ces idées. Cependant, on attend que vous proposiez une démarche novatrices et complémentaires à ce qui a été fait pendant le cours. 

Si votre démarche n'aboutit pas à des résultats satisfaisant, elle peut quand même être documentée dans le rapport final avec les raisons qui vous ont poussé dans cette direction, et ce que vous auriez attendu en cas de succès. 

## Rendus

Le rendu sera composé de deux fichiers : 
* un notebook Jupiter qui contiendra votre code, exécutable et commenté pour plus de clarté
* un rapport écrit qui prendra la forme d'une publication scientifique

Concernant le rapport écrit, le plan n'est pas déterminé à l'avance et dépend des sujets que vous abordez. Voici cependant une ébauche de plan pertinent dans le cadre d'une démarche expérimentale : 

1. Une introduction qui cadre le sujet, les objectifs que vous vous êtes fixés, ainsi que le contexte
2. La méthodologie que vous aurez appliqué, avec une description des données ainsi que des méthodes de modélisation et des outils que vous aurez choisis. C'est ici qu'il faut justifier le fait d'avoir privilégié une piste plutôt qu'une autre.
3. Les résultats que vous avez obtenus suite à l'exploration ainsi que la clusterisation, en illustrant autant que possible avec des visualisations
4. La discussion : interprétation des résultats, discussion sur leur pertinence et leurs implications, mais aussi limitations de l'étude et suggestions pour des travaux futurs.
5. La conclusion : Récapitulation sur les enseignements principaux de cette étude

Vous avez accès à toutes les ressources en lignes sans limitations, mais devrez dûment citer vos sources dans le rapport. 

