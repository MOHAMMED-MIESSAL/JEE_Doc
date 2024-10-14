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


## Qu'est ce que c'est le mot RequestDispatcher ?
Le RequestDispatcher est un objet en Java utilisé pour transférer une requête HTTP d'un Servlet à une autre ressource (comme un autre Servlet, une page JSP, ou un fichier statique) sans que le client (le navigateur) n'en soit informé.

#### Il existe deux méthodes principales associées à un RequestDispatcher :

forward() : Redirige la requête vers une autre ressource pour qu'elle prenne en charge l'intégralité de la réponse.  

include() : Inclut le contenu d'une autre ressource dans la réponse actuelle, permettant à la ressource initiale de traiter une partie de la réponse, puis d'inclure le résultat d'une autre ressource.  



## Qu'est ce que c'est le mot JSP ?
JSP (JavaServer Pages) est une technologie Java utilisée pour créer des pages web dynamiques.

### Fonctionnement de JSP :
Lorsque vous créez une page JSP, vous pouvez inclure du code Java directement dans le fichier HTML à l'aide de balises spéciales. 
Lorsque cette page est appelée par le navigateur, le serveur web (comme Apache Tomcat) transforme la page JSP en un Servlet Java. 
Ce Servlet est ensuite exécuté, et le résultat est renvoyé sous forme de page HTML au client (le navigateur).


### Cycle de vie d'une page JSP :
#### 1) Traduction : 
La page JSP est convertie en Servlet Java.  
#### 2) Compilation :
Le Servlet est compilé en bytecode (fichier .class).  
#### 3) Exécution : 
Le Servlet est exécuté, générant une page HTML en réponse à la requête du client.  
#### 4) Renvoi de la réponse : 
Le contenu HTML généré est envoyé au navigateur.  



## Qu'est ce que c'est le mot JavaBean ?
Un JavaBean est une classe Java qui suit des conventions spécifiques (constructeur sans argument, méthodes getter et setter, sérialisation)
et qui est utilisée pour encapsuler des objets, facilitant ainsi la manipulation des données


## Différence entre Seveur Web & Serveur d'Application & Conteneur de Servlets  :

### 1. Serveur Web :
Un serveur web est un logiciel qui gère les requêtes HTTP des clients (généralement des navigateurs) et sert des pages web statiques ou dynamiques. 
Son rôle principal est de traiter les requêtes liées aux pages web et de les renvoyer au client sous forme de HTML.  

#### Exemples :  
Apache HTTP Server (ne supporte que les pages statiques)  
Nginx  
Apache Tomcat (spécifiquement conçu pour les servlets et JSP ) 



### 2. Serveur d'Application :
Un serveur d'application est un environnement plus complet qui, en plus de servir des pages web et des applications basées sur des servlets/JSP,
supporte l'exécution de toutes les spécifications Java EE (Jakarta EE). 


#### Exemples :  
Wildfly (JBoss)  
GlassFish



### 3. Conteneur de Servlets :  
Un serveur d'application est un environnement plus complet qui, en plus de servir des pages web et des applications basées sur des servlets/JSP,
supporte l'exécution de toutes les spécifications Java EE (Jakarta EE). 














