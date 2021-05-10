# Présentation
L'objectif du projet est de mettre en pratique tout ce que nous avons vu jusqu'ici concernant le développement REACT et l'usage d'EC2 sur AWS.
Vous allez donc devoir :
- Créer une application REACT et utiliser Bootstrap pour la mise en page
- Builder votre application et la déployer sur un serveur EC2

## Application REACT JS et Bootstrap
L'application à développer s'appelle Kapshare.
- C'est une application simple qui possède :
  - Une page de Login
  - Une Page d'accueil qui affiche 3 photos dans un **carrousel Bootstrap**

Image1  | Image2  | Image3
------------- | ------------- | -------------
<img src="https://github.com/jekobokidou/kapsiki-exo/blob/main/exo-001/DESSA10.jpg" alt="image1" width="200"/>  | <img src="https://github.com/jekobokidou/kapsiki-exo/blob/main/exo-001/DESSA11.jpg" alt="image1" width="200"/>  | <img src="https://github.com/jekobokidou/kapsiki-exo/blob/main/exo-001/DESSA12.jpg" alt="image1" width="200"/>

- L'application implémenter les mécanismes REACT :
  - **props** : 
    - *props* pour indiquer quelle image s'affiche en premier par défaut
    - *props* pour indiquer la largeur de l'image dans le carrousel
    - Les props doivent avoir des valeurs par défaut
    - Les props doivent être typées
  - **state** :
    - Conserver le nombre de click sur chaque image dans le state et l'afficher 
  - **Route et Link**
    -  Utiliser Route pour afficher les différents composants
    -  Utiliser link pour gérer les liens comme la connexion, la déconnexion
  - **sessionStorage**
    -  Utiliser sessionStorage pour gérer le statut de l'utilisateur connecté
  - **build**
    - Rechercher dans la documentation comment builder votre application afin qu'elle puisse être déployée sur un serveur Apache


## Déploiement sur Amazon EC2
Dans la console EC2
- Provisionnez 2 machines virtuelles **t2.micro** Amazon Linux contenant Apache Dans **User Data**
- Déployez votre application sur les 2 serveurs
- Mettez vos serveurs dans un **target group**
- Configurez un **Application Load Balancer** pour votre target group
- Testez votre application

