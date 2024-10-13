# JEE DOCUMENTATION

## Qu'est ce que JEE ?

Jakarta EE est une plateforme qui fournit un ensemble d'outils et de spécifications pour le développement d'applications web robustes et évolutives destinées aux entreprises.


## Qu'est ce que c'est le mot Spécification ?

Le mot spécification désigne un ensemble de règles, normes et définitions qui décrivent comment un certain composant ou service doit fonctionner

### Spécification vs Implémentation :

#### Spécification : 
C'est une description abstraite de ce qu'un système, une classe, ou une méthode doit faire. Par exemple, une interface ou une classe abstraite fournit une spécification.

#### Implémentation : 
C'est la réalisation concrète de cette spécification. L'implémentation transforme cette description abstraite en code qui exécute une logique métier ou des opérations spécifiques.


## Qu'est ce que c'est le mot Servlet ?

Une Servlet est un composant Java côté serveur qui permet de traiter les requêtes et réponses HTTP dans une application web.

### Cycle de vie d'une Servlet 

![image](https://github.com/user-attachments/assets/52e322ba-2132-4f66-b79b-5dfec620d273)

#### 1) Chargement et Instanciation:
Le conteneur de servlets charge la classe de la servlet en mémoir et Il crée une instance de cette servlet.

#### 2) Initialisation :
La méthode init() est appelée une fois et une seule pour initialiser la servlet. C'est le moment d'effectuer des tâches de configuration, comme charger des fichiers de propriétés ou établir des connexions à des bases de données.

#### 3) Service :
Pour chaque requête HTTP, le conteneur appelle la méthode service(). Cette méthode est au cœur du traitement de la requête. Elle détermine le type de requête (GET, POST, etc.) et appelle la méthode appropriée (doGet(), doPost(), etc.).  
Les méthodes doGet() et doPost() sont les plus couramment utilisées pour traiter respectivement les requêtes GET et POST.

#### 4) Destruction :
Lorsque le conteneur décide de détruire la servlet (par exemple, au redémarrage du serveur ou lors d'un arrêt explicite), la méthode destroy() est appelée. C'est l'occasion de libérer les ressources utilisées par la servlet, comme les connexions à la base de données.

