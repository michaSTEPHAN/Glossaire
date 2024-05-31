# GLOSSAIRE

- [Général](#général)
- [Front-end](#front-end)
- [UX / UI](#ux-ui)
- [Architecture](#architecture)
- [Modélisation / Base de données](#modélisation---base-de-données)
- [Symfony](#symfony)
- [Sécurité](#sécurité)
- [RGPD](#rgpd)
- [SEO](#seo)
- [Gestion de projets / DevOps](#gestion-de-projets---devops)
- [English](#english)

## Général
1.	Quel est l’environnement à installer pour exécuter un script PHP ? Citer 2 exemples de logiciels permettant ce contexte.
    - Laragon (Windows) et MAMP (MAC)

2.	Qu’est-ce qu’un algorithme ?  
    - Un algorithme est une méthode générale pour résoudre un type de problèmes.
    - C'est une suite finie et non ambiguë d'instructions et d’opérations permettant de résoudre une classe de problèmes.

3.	Qu’est-ce qu’une variable ? Par quel symbole est préfixée une variable en PHP ?
    - Une variable est un élément qui associe une valeur à un libellé.
    - En PHP une variable est préfixée par un $.

4.	Qu’est-ce que la portée d’une variable ?
    - Une variable a une certaine « portée ». Il s’agit de la zone de code dans laquelle elle peut être utilisée, dans laquelle elle est définie.

5.	Qu’est-ce qu’une constante ? Quelle est la différence avec une variable ?
    - Une constante garde toujours la même valeur alors qu'une variable peut prendre différentes valeur dans le programme.

6.	Qu’est-ce qu’une superglobale, combien en existent-ils et donner un exemple d’utilisation 
    - Afin d'accéder à toutes les informations pouvant être transmises par le client au serveur, PHP dispose de plusieurs variables dites "superglobales". Toutes les superglobales sont du type tableau, proposant ainsi une manière simple d'y regrouper plusieurs informations sous forme de paires "clé / valeur".
    - Il en existe 9 ($GLOBALS,$_SERVER,$_GET,$_POST,$_FILES,$_COOKIE,$_SESSION,$_REQUEST,$_ENV)
    - Exemple $_GET : Liée à la méthode HTTP GET, contient tous les paramètres ayant été transmis au serveur par l'intermédiaire de l'URL de la requête (Query String Parameters).

7.	Quels sont les différents types (primitifs) que l’on peut associer à une variable en PHP ? 
    Les citer et en donner des exemples (ne pas oublier le type d’une variable sans valeur)
    - Les différents types sont :
        -> char (caractère) : $nom = 'michael'
        -> int (entier) : $age = 49
        -> float (chiffre à virgule) : $montant = 100,15€
        -> double (chiffre à virgule dépassant les 15 chiffres) : π
        -> boolean (booléen) : $estjuste = true
        -> byte (octet)
        -> void : null

8.	Existe-t-il plusieurs types de tableaux en PHP, si oui lesquels ?
    - Il y a les tableaux indexés, les tableaux associatifs et les tableaux multidimensionnels.

9.	Quelles sont les différentes structures de contrôles qu’il existe en algorithmie ? Donner un exemple pour chacune d’entre elles.
    - Il existe 3 différentes structures de contrôle :
        -> La séquence : Consiste à exécuter les actions les unes à la suite des autres (Ex : un bloc de code)
        -> La répetition : La répétition consiste à évaluer une condition et d'effectuer une ou des actions tant que la condition est VRAI (Ex : for, while, foreach)                        
        -> La sélection : La séquence consiste à exécuter les actions les unes à la suite des autres (Ex : if/else)                        

10.	Quelle est la fonction PHP permettant de demander la longueur d’une chaîne de caractères ?
    - strlen()

11.	Qu’est-ce qu’une session ? Quelle fonction permet de démarrer une session en PHP ? Donner un exemple d’utilisation en PHP
    - Les sessions sont un moyen simple de stocker des données individuelles pour chaque utilisateur en utilisant un identifiant de session unique. Elles peuvent être utilisées pour faire persister des informations entre plusieurs pages.
    - Les sessions peuvent être démarrées manuellement en utilisant la fonction session_start().
    - Site necessitant une connexion avec login + password.

12.	Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP.
    - Un cookie, appelé aussi témoin de connexion ou témoin, est une petite quantité de données échangées entre un serveur HTTP et un client HTTP, et qui permet de créer une session avec état lors de la visite d'un site Web.
    - Les cookies peuvent être utilisés pour maintenir les données relatives à l'utilisateur durant sa navigation, mais aussi à travers plusieurs visites. Les cookies ont été introduits pour donner un moyen d'implémenter les paniers d'achat électronique, des dispositifs permettant à l'utilisateur d'accumuler les articles qu'il veut acheter durant sa navigation sur le site.

13.	Quelle est la différence entre les instructions "require" et "include" en PHP ?
    - La fonction include est utilisée pour inclure un fichier au sein du processus courant. Elle prend un argument en entrée : la chaîne de caractères qui correspond au chemin du fichier.
    - La fonction require agit de la même manière que sa "sœur" include à ceci près qu'elle génère une erreur si le fichier à inclure n'est pas trouvé. Comme son nom l'indique, le fichier est requis pour que l'application fonctionne.

14.	Comment effectuer une redirection en PHP ?
                - header()

15.	Définir la partie "front-end" et "back-end" d’une application.
    - On trouve un front end et un back end dans chaque logiciel, et, par conséquent, dans chaque site Web. Les deux termes décrivent simplement deux niveaux différents qui constituent les programmes et les sites. Ces deux niveaux se retrouvent quand on traduit la première syllabe dans les deux cas : "front" désigne le premier plan et "back" l’arrière-plan.
    - La grande différence entre le front end et le back end est donc la finalité des deux composants. Le front end côté client est la zone visible d’un logiciel et le point de contact direct pour tous les utilisateurs finaux. Le back end côté serveur n’est pas directement visible en tant que dispositif d’arrière-plan, et reste généralement invisible aux yeux des utilisateurs du programme.

16.	Définir le contrôle de version ? Qu’est-ce que Git ?
    - Le contrôle de version, également appelé contrôle de source, désigne la pratique consistant à suivre et à gérer les changements apportés au code d'un logiciel.
    - GIT : C'est un logiciel de gestion de versions décentralisé. C'est un logiciel libre et gratuit, créé en 2005 par Linus Torvalds, auteur du noyau Linux, et distribué selon les termes de la licence publique générale GNU version 2. Le principal contributeur actuel de Git, et ce depuis plus de 16 ans, est Junio C Hamano.
    Depuis les années 2010, il s’agit du logiciel de gestion de versions le plus populaire dans le développement logiciel et web, qui est utilisé par des dizaines de millions de personnes, sur tous les environnements (Windows, Mac, Linux)3. Git est aussi le système à la base du célèbre site web GitHub, le plus important hébergeur de code informatique.

17.	Qu’est-ce qu’un CMS ? Citer au moins 2 exemples
        Un CMS est un système de gestion de contenu (Content Management System en anglais).
        Avec un CMS, les utilisateurs peuvent créer des sites web de toute sorte — sites vitrine, sites d’e-commerce, blogs — et gérer leur contenu sans avoir à coder les éléments de leur site à partir de zéro.
        Exemple : WordPress / Joomla

## Front-end
18.	Définir HTML
        - HTML =  HyperText Markup Language
        C'est le langage de balisage conçu pour représenter les pages web.
        Il permet d’écrire de l’hypertexte de structurer sémantiquement une page web, de mettre en forme du contenu, de créer des formulaires de saisie ou encore d’inclure des ressources multimédias dont des images, des vidéos, et des programmes informatiques.

19.	Définir CSS
        - CSS (Cascading Style Sheets) permet de créer des pages web à l'apparence soignée.
        C'est un langage de mise en forme des documents.

20.	Définir Javascript
    - JavaScript est un langage de programmation qui permet d'implémenter des mécanismes complexes sur une page web. À chaque fois qu'une page web fait plus que simplement afficher du contenu statique — afficher du contenu mis à jour à des temps déterminés, des cartes interactives, des animations 2D/3D, des menus vidéo défilants, ou autre, JavaScript a de bonnes chances d'être impliqué. C'est la troisième couche des technologies standards du web, les deux premières (HTML et CSS) étant couvertes bien plus en détail dans d'autres tutoriels sur MDN.

21.	Définir JSON. Dans quel contexte ce format est-il utilisé ? 
    - JSON (JavaScript Objet Notation) est un langage léger d’échange de données textuelles. Pour les ordinateurs, ce format se génère et s’analyse facilement. Pour les humains, il est pratique à écrire et à lire grâce à une syntaxe simple et à une structure en arborescence. JSON permet de représenter des données structurées (comme XML par exemple).

22.	Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?
    - Oui il est possible d’interpreter du JavaScript côté serveur avec Node.js, il s’suffit d’écrire une ligne de commande “node example.js”.

23.	Qu’est-ce qu’un sélecteur CSS ?
    - Un sélecteur est une expression qui indique au navigateur à quelle entité HTML s'applique la règle CSS correspondante. 
    Le ou les éléments ciblés par le sélecteur sont le sujet de ce sélecteur.

24.	Quelle balise HTML permet de créer un lien hypertexte ?
    - C'est la balise href
    <a href="https://www.commentcoder.com">Texte d'ancre</a>

25.	Qu’est-ce qu’une requête AJAX ?
    - Une requête AJAX est une technique qui permet d’actualiser une page web sans la recharger totalement.

26.	Quel sélecteur CSS permet de sélectionner tous les éléments d’une classe spécifique ? D’un identifiant spécifique ?
    - Le sélecteur "." permet de sélectionner tous les éléments d’une classe 
    - Le sélecteur "#" permet de sélectionner tous les éléments d’un identifiant.

27.	Définir le responsive design.
    - Le responsive design est le fait de créer une application qui s’adapte à différentes tailles d’écran (mobile, tablette et desktop).

28.	Qu’est-ce que le templating ?
    - Le templating est le fait de regrouper plusieurs fichiers et leurs appliquer du HTML/CSS afin d’éviter les répétitions.

29.	Qu’est-ce qu’une fonction anonyme en Javascript ?
    - Une fonction anonyme est une fonction qui n’a pas de nom. 
    - On peut exécuter en l’affectant à une variable, en l’auto-invoquant ou en l’utilisant dans un évènement.

30.	Quelle méthode JavaScript est utilisée pour ajouter un élément à la fin d'un tableau ?
    - La méthode push().

31.	Qu’est-ce qu’un « media query » ?
    - Un media query est une requête CSS qui permet de modifier le visuel en fonction de la taille de l’écran utilisé.

32.	Qu’est-ce qu’un pseudo élément en CSS ?
    - Un pseudo-élément est un mot-clé ajouté en utilisant "::" qui permet de mettre en forme certaines parties de l’élément ciblé par la règle.

33.	Qu’est-ce que Bootstrap ? Donner d’autres exemples équivalent
    - Bootstrap est un framework front-end, il permet de créer le HTML et CSS bien plus rapidement en utilisant des templates.
    - Tailwind, Bulma ou Materialize.

34.	Quand un formulaire HTML est créé, quelles sont les 2 méthodes qui peuvent lui être associées ? Donner la différence entre ces 2 méthodes
    - La méthode GET récupère une page et affiche son contenu alors que la méthode POST récupère le contenu et l’envoie au serveur.

## UX UI
35.	Quelle est la différence entre UX Design et UI Design ?
    - UX design (User Experience) se focalise sur la facilité de prise en main et l'accessibilité de l'interface.
    - UI design (User Interface) se focalise sur les visuels et la visibilité de l'interface.

36.	Qu’est-ce qu’un wireframe ? 
    - Un wireframe est un schéma d'une page web, il est souvent fait de forme basiques et en nuances de gris. Un wireframe permet de pré-visualiser la structure d'un site.

37.	Qu’est-ce qu’un prototype ? 
    - Un prototype est une version détaillée du produit fini avec animations et transitions incluses

38.	Qu’est-ce que la hiérarchie visuelle en UI Design ?
    - La hiérarchie visuelle est le fait d'appliquer des propriétés à certains éléments afin de les faires ressortirs
    Ex : Contraste de couleur, texte gras, taille de la police...

39.	Qu’est-ce que l’accessibilité en UX Design ? 
    - Les produits doivent être utilisables par des personnes de tous les âges, capacités et handicaps, en suivant les directives d’accessibilité.

40.	Qu’est-ce qu’une grille de mise en page ?
    - La grille est un élément déterminant de la mise en page, permettant de structurer le format. Elle est incontournable pour les documents d’édition, numérique ou les formats de presse.
    - lle permet de découper le format dans sa largeur (et plus tard dans sa hauteur) en plusieurs parties égales, séparées par des espaces verticaux. L’usage des colonnes ainsi créées permet de travailler avec des « zones », proportionnelles entre elles, ce que l’œil du lecteur perçoit immédiatement.
    - Bien qu’elle ne soit pas la seule composante de la lisibilité, la grille, et donc l’agencement dans la page qu’elle sous-tend, contribue grandement à la lisibilité.

41.	Qu’est-ce que la notion d’affordance en UX Design ?
    - Simplifier le parcours de navigation de l’utilisateur en rendant le site ergonomique, simple et accessible. C’est ce qu’implique l’affordance en UX Design.
    - L’affordance est définie par la disposition d’un élément à connoter explicitement sa vocation. Disposée dans un environnement propice à sa compréhension, l’utilisation de l’objet est alors évidente et intuitive.

42.	Qu’est-ce qu’un « mobile first design » ?
    - Le mobile first design est le fait de créer un site avec une structure et un style adapté aux petits écrans, puis de l'ajuster pour les écrans plus larges.

## Programmation orientée objet (POO)
43.	Donner une définition de la programmation orientée objet
    - La POO consiste à définir et faire interagir entre eux des objets, compris ici comme tous types de structures issues d’un langage donné. Par convenance, les objets en POO désignent le plus souvent des variables complexes, elles-mêmes composées de variables ou de fonctions.

44.	Qu’est-ce qu’une classe ? Comment la déclare-t-on ?
    - Une classe est un élément qui créé contient des objets, on la déclare avec des attributs et des méthodes.

45.	Qu’est-ce qu’un objet ?
    - Un objet représente un concept, une idée ou toute entité du monde physique. Il possède une structure interne et un comportement et peut interagir avec ses pairs.

46.	Définir la notion de propriété / attribut / méthode
    - Les attributs (propriétés) représentent les caractéristiques de l’objet et les méthodes correspondent aux actions possibles avec l’objet.

47.	Qu’est-ce que la visibilité d’une propriété ou d’une méthode ? Citer les différents types de visibilité
    - La visibilité d’une propriété/méthode correspond à son rayon d’action.
        -> Publique : permet aux propriétés/méthodes d’être accessible depuis n’importe où dans le programme principal.
        -> Privée   : permet aux propriétés/méthodes de n’être accessible que depuis l’intérieur de la classe.
        -> Protégée : intermédiaire entre les deux autres, elle permet d’utiliser les propriétés/méthodes communs dans une classe parente et ses classes dérivées.

48.	Quelle est la méthode spécifique utilisée pour créer un nouvel objet à partir d’une classe ?
    - Le constructor est la méthode (magique) la plus utilisée pour créer un nouvel objet, elle permet de définir tous les attributs de l’objet en le créant.

49.	Qu’est-ce que l’encapsulation ?
    - L’encapsulation est un mécanisme consistant à rassembler les données et les méthodes au sein d’une structure en cachant l’implémentation de l’objet, c’est-à-dire en empêchant l’accès aux données par un autre moyen que les services proposés. 
    L’encapsulation permet donc de garantir l’intégrité des données contenues dans l’objet. Ainsi, si l’on veut protéger des informations contre une modification inattendue, on doit se référer au principe d’encapsulation.

50.	Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple
    - Étendre une classe consiste à créer une classe mère qui regroupe des classes enfants. Cela permet aux classe enfant d’hériter des attributs de la classe mère.
    Ex : On crée une classe mère “Personne” et deux classes enfant “Acteur” et “Réalisateur”, on a plus qu’à déclarer les attributs 
        (nom, prenom, sexe, age) une seule fois dans la classe “Personne” et les deux classes enfant hériteront de ses attributs.

51.	Définir l’opérateur de résolution de portée
    - L'opérateur de résolution de portée [symbole "double deux-points" (::)] fournit un moyen d'accéder aux membres "constante", "propriété statique", "méthode statique d'une classe" ou "une de ses classes parentes". 

52.	Définir une méthode / propriété statique
    - Une propriété ou une méthode statique est une propriété ou une méthode qui ne va pas appartenir à une instance de classe ou à un objet en particulier mais qui va plutôt appartenir à la classe dans laquelle elle a été définie.

53.	Définir le polymorphisme en POO
    - Le mot polymorphie vient du grec et signifie "qui peut prendre plusieurs formes". Dans la programmation orienté objet, le polymorphisme est utilisé en relation avec les fonctions, les méthodes et les opérateurs. Des fonctions et des méthodes de mêmes noms peuvent avoir des comportements différents ou effectuer des opérations sur des données de types différents. 
    On distingue 2 types de polymorphisme, la surcharge et la redéfinition.

54.	Définir une méthode / classe abstraite ?
    - Une méthode abstraite peut seulement être déclaré par son nom ou ses paramêtres (signature).
    - Une classe abstraite est une classe qui ne peut être instanciée. 
    Si une classe contient une méthode abstraite, elle doit elle aussi devenir une classe abstraite

55.	Définir le chaînage de méthodes
    -Chainer des méthodes nous permet d’exécuter plusieurs méthodes d’affilée de façon simple et plus rapide, en les écrivant à la suite les unes des autres, "en chaine".
    En pratique, il va suffire d’utiliser l’opérateur d’objet pour chainer différentes méthodes. On écrira quelque chose de la forme $objet->methode1()->methode2().

56.	Qu’est-ce que la méthode __toString() ? Existe-t-il d’autres méthodes « magiques »
    - La méthode magique **toString permet de passer en chaîne de caractères différents attributs de la classe, elle peut être appelée en utilisant $this. 
    Il existe d’autres méthodes magiques (__construct, __destruct, __call et plein d’autres).

57.	Qu’est-ce qu’un « autoload » ?
    - Un autoload est un auto-chargement de classe, il permet de charger plusieurs classes d’un programme au sein d’un seul et même fichier.

58.	Comment appelle-t-on en français les « getters » et les « setters » ?
    - es getters sont des accesseurs et les setters sont des mutateurs.

59.	Qu’est-ce que la sérialisation en PHP ? 
    - La sérialisation est une technique qui à pour but de transferer des valeurs entre scripts sans qu'elles perdent leurs structure ou type.

## Architecture 
60.	Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur. 
Définir l’acronyme de ce type de requête. 
Si on ajoute un "S" à cet acronyme, expliquer la différence.

61.	Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern
    - Les Design Patterns, ou modèles de conception, sont des solutions éprouvées à des problèmes récurrents de design ou de code. Utile au designer et au développeur, le design pattern améliore aussi l’utilisabilité du site ou de l’application. 
    Ces "patrons de conception", réutilisables, rendent l’interface plus intuitive pour l’utilisateur.
    - Modèle de référence qui sert de source d'inspiration lors de la conception de l'architecture d'un système ou d'un logiciel informatique en sous-éléments plus simples.
    - Ex :  
            -> Prototype: permet de créer de nouveaux objets en copiant des objets  existants.
            -> Flyweight: permet de réduire l'utilisation de la mémoire en partageant des objets similaires.
            -> Observer :  établit une relation un à plusieurs entre des objets, où lorsqu'un objet change, plusieurs autres objets sont avisés du changement

62.	Qu’est-ce que l’architecture MVC ?
    - MVC, ou modèle-vue-contrôleur (model-view-controller en anglais), est ce qu’on appelle un modèle d’architecture logicielle. Ce type d’architecture, aujourd’hui très répandu dans les projets d’applications web, doit son succès notamment à sa forte maintenabilité et à sa facilité à être utilisé en travail collaboratif.

63.	Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?
    - Model
        Il représente les données qui vont être utilisées dans l’application web. C’est ici que va être stockée la data, et tout ce qui permet de la modifier (getters, setters, etc.), que ça soit en local en en distant (base de données).
        Ce sont littéralement des modèles de données.

    - View
        C’est l’interface graphique de l’application. C’est via cet élément que vont se faire les interactions entre l’utilisateur et le code métier. Elle ne contient presque aucune logique (contrairement à l’architecture concurrente de MVC dont on parlera plus loin), son but est de construire, à partir de ce que renvoie le serveur, une interface et de l’afficher à l’utilisateur.

    - Controller    
        C'est l’élément qui contient la logique métier. C’est ici que sont la plupart des algorithmes, calculs, etc...
        C’est aussi l’intermédiaire principal entre la vue et le modèle. Par exemple, la vue soumet un formulaire au contrôleur, qui gère sa validation via du code métier, et demande au modèle de faire des modifications dans la base de données.


64.	Quels sont les avantages de l’architecture MVC ?
    - Facile à maintenir, de par sa séparation obligatoire en fichiers et logique.
    - Le développement peut se faire à plusieurs niveaux en parallèle (création des vues par un développeur freelance front pendant qu’un développeur back travailler sur les contrôleurs).
    - La décorrélation des vues et de la logique permet de tester le code de manière plus simple et efficace, du moins en théorie.

65.	Existe-t-il des variantes à l’architecture MVC ?
    - Oui il existe l'architecture Flux créée par Facebook.

66.	Qu’est-ce qu’une API ? Définir l’architecture REST
    - API
        Une API, ou interface de programmation, est un programme qui permet à deux applications distinctes de communiquer entre elles et d’échanger des données1. C’est un concept intangible qui fonctionne sur un accord d’entrées et de sorties2. Une API peut être utilisée pour ajouter des informations à une application sans avoir à la recréer ou la redévelopper entièrement1. Une application peut être un logiciel ou une application mobile2.
    - Architecture REST
        REST (Representational State Transfer) est un style d’architecture permettant de construire des applications (Web, Intranet, Web Service). 
        Il s’agit d’un ensemble de conventions et de bonnes pratiques à respecter et non d’une technologie à part entière. L’architecture REST utilise les spécifications originelles du protocole HTTP, plutôt que de réinventer une surcouche (comme le font SOAP ou XML-RPC par exemple).

## Modélisation - Base de données
67.	Qu’est-ce que la modélisation de données ? Définir la méthode Merise
    -> La modélisation des données est le processus de création d'une représentation visuelle de l'ensemble ou d'une partie d'un système d'information, afin de communiquer les connexions entre les points et les structures de données. L'objectif est d'illustrer les types de données utilisées et stockées dans le système, les relations entre ces types de données, les façons dont les données peuvent être regroupées et organisées, ainsi que leurs formats et attributs.

    -> MERISE est une méthode de conception, de développement et de réalisation de projets informatiques. Le but de cette méthode est d'arriver à concevoir un système d'information. La méthode MERISE est basée sur la séparation des données et des traitements à effectuer en plusieurs modèles conceptuels et physiques.

68.	Quelles sont les 3 étapes principales de la méthode Merise ? 
    a.	Analyse, conception et réalisation
    b.	Planification, exécution et contrôle
    c.	Création, modification et suppression

69.	Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?
    - Un MCD consiste à représenter de manière visuelle et simplifiée l’ensemble des données d’un système d’information.
    - Il repose sur les notions d'entité et d'association et sur les notions de relations. Il s'intéresse à décrire la sémantique du domaine (entity/relationship en anglais).

70.	Qu’est-ce qu’un modèle logique de données (MLD) en Merise ?
    - Le MLD, également appelée dérivation du MCD dans un formalisme adapté à une implémentation ultérieure, au niveau physique, sous forme de base de données relationnelle ou réseau, ou autres (ex : simples fichiers).

71.	Donner la définition des mots suivants :
    a.	Entité
        -> L'entité est définie comme un objet de gestion considéré d'intérêt pour représenter l'activité à modéliser 
        (exemple : entité pays)
    b.	Relation
        -> Une relation est un lien sémantique entre entités.
    c.	Cardinalité
        -> La cardinalité, celle-ci indique le nombre minimum (0 ou 1) et maximum (1 ou n) de fois où une occurrence quelconque d'une entité peut participer à une relation.
    d.	Clé primaire / clé étrangère
        -> Dans une base de données relationnelle, une clé primaire est la donnée qui permet d'identifier de manière unique un enregistrement dans une table.
        -> Une clef étrangère est une contrainte qui consiste à avoir, dans une table, une colonne dont la valeur est indexée sur le champ d'une autre table.

72.	Que devient une relation de type « Many To Many » dans le modèle logique de données ?
    - Une entité.

73.	Qu’est-ce qu’une base de données ?
    - Une base de données permet de stocker et de retrouver des données structurées, semi-structurées ou des données brutes ou de l'information, souvent en rapport avec un thème ou une activité ; celles-ci peuvent être de natures différentes et plus ou moins reliées entre elles.
    - Une base de données est un "conteneur" stockant des données telles que des chiffres, des dates ou des mots, pouvant être retraités par des moyens informatiques pour produire une information. 

74.	Définir les notions suivantes : 
    a.	SQL
        - SQL (Structured Query Language, "langage de requêtes structurées") est un langage informatique normalisé servant à exploiter des bases de données relationnelles. 
        La partie langage de manipulation des données de SQL permet de rechercher, d'ajouter, de modifier ou de supprimer des données dans les bases de données relationnelles.
    b.	MySQL
        -  MySQL est le système de gestion de base de données relationnelle le plus populaire.
    c.	SGBD (donner 2 exemples de SGBD)
        - Système de Gestion de Bases de Données
        Ex : Oracle/MySQL/SQLServer

75.	Dans une base de données, les données sont stockées dans des ___. 
Celles-ci sont constituées de lignes appelées ___ et de colonnes appelées ___
    - TABLES / ENREGISTREMENTS / ATTRIBUTS ou CHAMPS

76.	Quelle est la différence entre une base de données relationnelle et non relationnelle ?
    - Une base de données relationnelle est une base de données où l'information est organisée dans des tableaux à deux dimensions appelés des relations ou tables. Une base de données relationnelle consiste en une ou plusieurs relations. Les lignes de ces relations sont appelées des enregistrements. Les colonnes sont appelées des attributs.
    - Une base de données non relationnelle est une base de données qui n’utilise pas le schéma tabulaire sous forme de lignes et de colonnes présent dans la plupart des systèmes de base de données plus traditionnels. Au lieu de cela, les bases de données non relationnelles utilisent un modèle de stockage qui est optimisé pour les exigences spécifiques du type des données stockées. Par exemple, les données peuvent être stockées sous forme de paires clé/valeur simples, de documents JSON ou de graphe comprenant des arêtes et des sommets.

77.	Qu’est-ce qu’une jointure dans une base de données ? En existe-t-il plusieurs ? Si oui lesquelles ?
    - La jointure est une opération essentielle en SQL, permettant de combiner les enregistrements de deux ou plusieurs tables basées sur des colonnes communes. Plus précisément, une jointure est l'union de « n » tables contenant des valeurs identiques dans « m » de leurs colonnes. Les jointures sont utilisées pour retrouver des données dispersées sur plusieurs tables en une seule requête.
        - INNER JOIN
        - LEFT OUTER JOIN
        - RIGHT OUTER JOIN
        - FULL OUTER JOIN
        - CROSS JOIN

78.	A quoi sert une vue dans une base de données ?
    - Une vue dans une base de données est une synthèse d'une requête d'interrogation de la base. On peut la voir comme une table virtuelle, définie par une requête.
    - Les avantages des vues sont :
        -> Eviter de taper une requête très longue : la vue sert à donner un nom à la requête pour l'utiliser souvent,
        de masquer certaines données à certains utilisateurs. 

79.	Qu’est-ce que l’intégrité référentielle dans une base de données ?
    - En informatique, et plus particulièrement dans les bases de données relationnelles, l´intégrité référentielle est une situation dans laquelle pour chaque information d'une table A qui fait référence à une information d'une table B, l'information référencée existe dans la table B. L'intégrité référentielle est un gage de cohérence du contenu de la base de données.

80.	Quelles sont les fonctions d’agrégation en SQL ?
    - Les fonctions d’agrégation dans le langage SQL permettent d’effectuer des opérations statistiques sur un ensemble d’enregistrement.
        -> AVG() pour calculer la moyenne sur un ensemble d’enregistrement
        -> COUNT() pour compter le nombre d’enregistrement sur une table ou une colonne distincte
        -> MAX() pour récupérer la valeur maximum d’une colonne sur un ensemble de ligne. 
           Cela s’applique à la fois pour des données numériques ou alphanumérique
        -> MIN() pour récupérer la valeur minimum de la même manière que MAX()
        -> SUM() pour calculer la somme sur un ensemble d’enregistrement

81.	Qu’est-ce qu’un CRUD dans le contexte d’une base de données ?
    - L'acronyme informatique anglais CRUD (pour Create, Read, Update, Delete) (parfois appelé SCRUD avec un "S" pour Search) désigne les quatre opérations de base pour la persistance des données, en particulier le stockage d'informations en base de données.
    Soit :
        -> Create : créer
        -> Read : lire
        -> Update : mettre à jour
        -> Delete : supprimer
    Plus généralement, il désigne les opérations permettant la gestion d'une collection d'éléments.
    Ce terme est aussi un jeu de mots en anglais sur l'adjectif crude (en français brut ou rudimentaire).

2.	Quelles sont les clauses qui permettent de :
    a. Insérer un nouvel enregistrement dans une table
        -> INSERT INTO
    b. Modifier un enregistrement dans une table
        -> UPDATE
    c. Supprimer un enregistrement dans une table
        -> DELETE FROM
    d. Supprimer la base de données
        -> DROP
    e. Filtrer les résultats d’une requête SQL
        -> WHERE
    f. Trier les résultats d’une requête SELECT
        -> ORDER BY
    g. Regrouper les résultats d'une requête SELECT en fonction d'une colonne spécifique
        -> GROUP BY
    h. Concaténer 2 chaînes de caractères 
        -> CONCAT

83.	Comment se connecter à une base de données en PHP ? Quelle est la classe native utilisée ?

## Symfony
84.	Qu’est-ce que Symfony ?
85.	Sur quel langage de programmation et design pattern repose Symfony ? 
86.	Quelle est la dernière version en date de Symfony ?
87.	Qu’est-ce qu’un bundle ? 
88.	Quel est le moteur de template utilisé par défaut dans Symfony ?
89.	Qu’est-ce qu’un ORM ? Quel est son utilité et comment s’appelle-t-il au sein de Symfony ?
90.	Qu’est-ce que l’injection de dépendances ? Quel est l’outil utilisé dans ce contexte et quel fichier contient l’intégralité des dépendances du projet ?
91.	Que permet le bundle Maker au sein de Symfony ? 
92.	Quel est le langage de requêtage exploité au sein d’un projet Symfony ?
93.	Quel est le composant qui garantit l’authentification et l’autorisation des utilisateurs ?

## Sécurité
94.	Qu’est-ce que l’injection SQL ? Comment s’en prémunir ?
    - Une injection SQL, parfois abrégée en SQLi, est un type de vulnérabilité dans lequel un pirate utilise un morceau de code SQL (« Structured Query Language », langage de requête structuré) pour manipuler une base de données et accéder à des informations potentiellement importantes. C'est l'un des types d'attaques les plus répandus et menaçants, car il peut potentiellement être utilisé pour nuire à n'importe quelle application Web ou n'importe quel site Web qui utilise une base de données SQL (soit la plupart).
    - Pour les entreprises soucieuses de la prévention des injections SQL, les principes clés pour les aider à protéger les sites et les applications Web sont les suivants :
        -> Formation du personnel
        -> Contrôlez les saisies des utilisateurs
        -> Utilisez les dernières versions
        -> Analysez en permanence les applications Web
        -> Utiliser un pare-feu

95.	Qu’est-ce que la faille XSS ? Comment s’en prémunir ?
    - Le Cross-site Scripting (XSS) est une vulnérabilité particulièrement répandue dans les applications web.
    Les XSS font partie de la catégorie des vulnérabilités par injection de code au même titre que les injections SQL. Cependant pour découvrir et exploiter une faille XSS, il s’agit pour un attaquant d’injecter du code malveillant via les paramètres d’entrée côté client.
    - Pour prévenir les attaques XSS, il faut partir du principe que les données reçues par une application web ne peuvent pas être considérées comme « toujours » sûres.
    Il est donc important d’implémenter des mesures de protection pour traiter toutes les données venant de l’extérieur. Ainsi, tout contenu doit être filtré, validé et encodé avant d’être utilisé par l’application.

96.	Qu’est-ce que la faille CSRF ? Comment s’en prémunir ?
    - CSRF : le Cross Site Request Forgery (XSRF en français) est un mode d’escroquerie courant sur Internet. Les criminels prennent le contrôle d'une session autorisée par l’utilisateur (Session Riding) et peuvent ainsi exécuter des actions malveillantes. Celles-ci passent par le biais de requêtes HTTP.
    - On peut s'en premunir en :
        -> En ligne, en prenant des précautions et en faisant preuve de prudence.
        -> Contrôlant la présence de logiciels malveillants sur un terminal
        -> Protegeant contre les CSRF par les exploitants de sites
        -> En mettant en place la double authentification
        -> Se déconnectant après utilisation

97.	Définir l’attaque par force brute et l’attaque par dictionnaire
    - Une attaque par force brute est une méthode de piratage utilisant une tentative et une erreur pour déchiffrer les mots de passe, les identifiants de mot de passe et les clés de chiffrement. Il  s’agit d’une tactique simple mais fiable pour obtenir un accès non autorisé aux comptes individuels et aux systèmes et réseaux des organisations. Le hacker essaie plusieurs noms d’utilisateur et mots de passe, souvent à l’aide d’un ordinateur pour tester un large éventail de combinaisons, jusqu’à ce qu’il trouve les bonnes informations de connexion.
    Le nom "force brute" provient d’attaquants qui utilisent des tentatives excessivement puissantes pour accéder aux comptes d’utilisateurs. Bien qu’il s’agisse d’une ancienne méthode de cyberattaque, les attaques par force brute sont testées et restent une tactique populaire auprès des hackers.
    - Une attaque par dictionnaire est une attaque ciblant des mots de passe qui utilise des mots du dictionnaire ou des expressions courantes pour pirater les identifiants de connexion d'utilisateurs. Si vous utilisez des mots du dictionnaire ou des expressions courantes comme mots de passe, vous pouvez être vulnérable face à une attaque par dictionnaire.

98.	Existe-t-il d’autres failles de sécurité ? Citer celles-ci et expliquer simplement leur comportement.

99.	A quoi servent l’authentification et l’autorisation dans un contexte d’application web ?

100. Définir la notion de hachage d’un mot de passe et citer des algorithmes de hachage

101. Qu’est-ce qu’une politique de mots de passe forts ?

102. Qu’est-ce que l’hameçonnage ?

103. Définir la "validation des entrées"

## RGPD
104. Qu’est-ce que le RGPD ?
    - Règlement Général (européen) sur la Protection de Données.
        -> Concerne le traitement et la circulation des données à caractère personnel
        -> Fixe les conditions dans lesquelles les données peuvent être collectées, conservées et exploitées
        -> Doit aussi s’y conformer : 
            - tous les organismes qui se trouvent dans l’Union européenne
            - qui collectent et traitent des données des personnes situées sur le territoire de l’UE

105. Quel est son objectif principal ?
    -> Harmoniser la législation entre tous les pays européens
    -> Responsabiliser les acteurs
    -> Renforcer la confiance des citoyens européens qui confient leurs données en
      améliorant leur protection et leur confidentialité

106. Quelle est la date d’entrée en vigueur du RGPD ?
    -> Signé en avril 2016 et applicable depuis le 25 mai 2018

107. Quelles sont les sanctions possibles en cas de non-respect du RGPD ?
    -> Mise en demeure publique ou non (sur cnil.fr + legifrance.fr)
        - Amende administrative 
            20 millions € ou 4 % du CA mondial (maximum retenu)
        - Sanction
            Rappel à l’ordre par la présidente ou la formation restreinte
        - Injonction sous astreinte
            Ordre de satisfaire aux demandes d'exercice des droits des personnes, y compris sous astreinte
        - Sanction pénale
            300 000 € et 5 ans de prison pour les personnes physiques
            1 500 000 € pour les personnes morales

108. En France, quel est l’autorité administrative qui s’occupe de faire appliquer le RGPD ?
    - CNIL : Commission nationale de l’informatique et des libertés

109. Quel est le consentement valide selon le RPGD ?
110. Qu’est-ce qu’une politique de confidentialité ?
    - La politique de confidentialité est un document expliquant en détail les modalités de traitement des données personnelles dans le cadre d’une relation commerciale.
    Ainsi, cela concerne les opérations de traitement de données telles que :
        -> la collecte
        -> le classement
        -> le traitement
        -> la publication et la suppression des données
        
111. Quelle est la durée de conservation maximale des données personnelles selon le RGPD ?
112. Quels sont les droits des utilisateurs selon le RGPD ?
113. Qu’est-ce que le principe de minimisation des données selon le RGPD ?

## SEO
114. Qu’est-ce que le SEO ? 
    - SEO est l'acronyme de Search Engine Optimization et peut être défini comme l'art de positionner un site, une page web ou une application mobile dans les premiers résultats naturels des moteurs de recherche. En français, le SEO est désigné par le terme de référencement naturel.

115. Quel est l’objectif principal du SEO ?
    - Le principal objectif du SEO est d'accroître la visibilité d'un site web en obtenant un classement supérieur dans les résultats de recherche.

116. Existe-t-il plusieurs types de référencement ? Lesquels ?

117. Qu’est-ce que la densité de mots-clés en SEO ?
    - La densité de mots-clés est une mesure utilisée en SEO pour évaluer la fréquence d'apparition d'un mot-clé dans un texte en comparaison au nombre total de mots du texte. 
    Elle a  historiquement été utilisée pour déterminer la pertinence d'un contenu par rapport à une requête de recherche. Cependant, au fil du temps, les moteurs de recherche ont évolué et ne se basent plus uniquement sur la densité de mots-clés pour évaluer la pertinence d'un contenu.

118. Qu’est-ce qu’une balise « alt » ?
    - La balise ALT est un élément HTML qui permet de décrire une image et d'améliorer son référencement naturel. 

119. Qu’est-ce que la balise « meta description » ?
    - Une balise meta description est un élément HTML qui résume le contenu d’une page web. 
    Elle s’affiche sous le titre de la page dans les résultats des moteurs de recherche. 
    Elle permet aux internautes et aux moteurs de recherche de connaître la teneur et la qualité de la page. 
    Elle doit être concise et pertinente, et ne pas dépasser 160 à 240 caractères.

120. Qu’est-ce que le « nofollow » en SEO ?

121. Quelle est l'importance du contenu de qualité pour le référencement d'un site web ?

122. Pourquoi est-il important d'utiliser des balises de titre (h1, h2, h3, etc.) de manière structurée ?

123. Quelle est la recommandation pour les URL d'un site web bien référencé ?

124. Qu'est-ce que le maillage interne et pourquoi est-il important pour le référencement ?

125. Qu'est-ce que l'optimisation des images pour le référencement ?

126. Qu'est-ce qu'un plan de site (sitemap) et pourquoi est-il important pour le référencement ?

## Gestion de projets - DevOps
127. Qu’est-ce que la gestion de projet ?	
    - La gestion de projet consiste à planifier, organiser, et gérer les ressources pour atteindre des objectifs spécifiques dans un projet.
    - La gestion de projet1, est l'ensemble des activités visant à organiser le bon déroulement d’un projet et à en atteindre les objectifs en temps et en heures selon les objectifs visés. Elle consiste à appliquer les méthodes, techniques, et outils de gestion spécifiques aux différentes étapes du projet, de l'évaluation de l'opportunité jusqu'à l'achèvement du projet.

128. Qu’est-ce qu’une méthode Agile de gestion de projet ? 
    - La méthode agile est une méthodologie de gestion de projet ouverte au changement, dont l'objectif est de développer un produit de haute qualité de façon incrémentale.
    - Elle s'oppose aux méthodologies de gestion de projet traditionnelles qui s'organisent selon un mode de travail séquentiel.
    - La méthode agile est organisée en cycles de développements courts, appelés des sprints. Le produit final est développé au fur et à mesure de l'avancement des sprints.

129. Expliquer la méthode MoSCoW en quelques lignes et citer ses avantages.
    - La méthode MoSCoW est une technique visant à établir les priorités des besoins ou des exigences en matière d'assistance à maîtrise d'ouvrage et de développement logiciel. L'objectif est que le maître d'œuvre et le maître d'ouvrage s'accordent sur l'importance des tâches à réaliser par rapport aux délais prévus.

130. A quoi sert la méthodologie MVP ? Citer les caractéristiques clés
131. Qu’est-ce que la planification itérative ?
    - La planification itérative repose sur l’idée que les plans les mieux conçus nécessitent souvent des ajustements à mesure que les circonstances changent et que de nouvelles idées émergent. Cela implique un processus cyclique de planification, d’exécution, d’évaluation et de révision.

132. Citer 3 méthodes Agiles dans le cadre d’un projet informatique
        - La méthode Scrum
        - La méthode Kanban
        - La méthode Kanban

133. Qu’est-ce qu’une réunion de revue de projet ?
    - La revue de projet, aussi appelée réunion de revue, est une des réunions essentielles du projet.
    Elle a lieu à la fin de chaque phase majeure.
    Elle permet à la fois de valider que le travail accompli jusque-là est en ligne avec le plan détaillé et d’officialiser le passage à la phase suivante.
    Il y a donc plusieurs revues durant un projet.

134. Qu’est-ce qu’un livrable dans un projet ? 
    - Un livrable projet est le résultat attendu d'une tâche ou d'un projet, qui prend généralement la forme d'un produit physique, d'un logiciel, d'un service ou encore d'un document. Il s'agit d'un résultat spécifique, tangible et mesurable.

135. Quels sont les 3 piliers SCRUM ? Définir chacun d’entre eux.
    - Les trois piliers de Scrum  sont :
        -> La transparence : Tous les membres de l'équipe projet et les parties prenantes savent ce qu'il se passe.
        -> L'inspection    : Le travail est vérifié au fur et à mesure, afin d'éviter de devoir refaire deux fois la même chose. On le fait bien du premier coup.
        -> L'adaptation : L'équipe Scrum s'adapte continuellement au projet, à son contexte, et à ce qu'elle apprend en cours de route grâce à l'empirisme.

136. Qu’est-ce que le DevOps et quel est son objectif principal ?
    - Le terme “DevOps” est composé des termes “développement” et “opérations”. Il s’agit d’une pratique visant à fusionner le développement, l’assurance qualité, et les opérations à savoir le déploiement et l’intégration en un unique ensemble de processus continus.
    Cette méthodologie nouvelle est une extension naturelle des approches Agile et de livraisons continue (CI/CD).
    - avantage du DevOps est la vitesse. Cette méthode permet d’accélérer les lancements de produits et d’améliorer leur qualité. L’accélération est liée à la livraison continue, permettant de recevoir un feedback plus rapidement. Ainsi, les développeurs peuvent corriger les bugs de façon précoce. Les équipes peuvent donc se focaliser sur la qualité du produit et automatiser les processus.

137. Qu’est-ce que l’intégration continue ? 
    - 'intégration continue (de l'anglais : Continuous integration, CI), est un ensemble de pratiques utilisées en génie logiciel consistant à vérifier à chaque modification de code source que le résultat des modifications ne produit pas de régression dans l'application développée.

138. Qu’est-ce que Docker ? Et en quoi est-il utile dans le cadre du DevOps ?
        - Lorsque vous arrivez sur une nouvelle machine, plusieurs choses peuvent changer. 
        Par exemple les paramètres dans le PHP.ini ne seront pas forcément les mêmes, ou même les versions de PHP et MySQL ne seront pas les bonnes.
        - Docker va nous permettre de paramétrer un environnement et de pouvoir l’utiliser sur différentes machines (et sur différents systèmes d’exploitation).

139. Qu’est-ce qu’un test unitaire ?
        -  le test unitaire ("TU" ou "UT" en anglais) est une procédure permettant de vérifier le bon fonctionnement d'une partie précise d'un logiciel ou d'une portion d'un programme (appelée "unité" ou "module").

140. Quelle est l'unité de code testée lors d'un test unitaire ?
141. Quelles sont les caractéristiques d'un bon test unitaire ?
142. Qu'est-ce qu'une assertion dans un test unitaire ?
 
## English
1)	What does JavaScript enable you to do on a website ?
    a.	Add interactive behavior and dynamic content------------------------------------------ YES
    b.	Define the layout and design of web pages
    c.	Handle server-side operations
2)	Which programming language is primarily used for server-side web development ?
    a.	PHP----------------------------------------------------------------------------------- YES
    b.	JavaScript
    c.	HTML
3)	What is the purpose of a web browser ?
    a.	To render and display web pages------------------------------------------------------- YES 
    b.	To execute serve-side code
    c.	To manage databases
4)	What is the difference between GET and POST methods in HTTP ?
    a.	GET retrieves data from a server, while POST submits data to a server----------------- YES
    b.	GET submits data to a server, while POST retrieves data from a server
    c.	GET and POST methods are interchangeable
5)	What is the purpose of version control systems (e.g., Git) in web development ?
    a.	To track changes and manage collaborative development--------------------------------- YES
    b.	To optimize website loading speed
    c.	To handle server-side scripting
6)	What is the purpose of a framework in web development ?
    a.	To provide a structured environment for building web applications--------------------- YES
    b.	To handle network protocols and data transfer
    c.	To create visual designs and layouts for websites
7)	What does NoSQL stand for ?
    a.	Not Only SQL-------------------------------------------------------------------------- YES
    b.	Non-Structured Query Language
    c.	New Object-Oriented Language
8)	Which of the following is a characteristic of NoSQL databases ?
    a.	Strict schema enforcement
    b.	Support for complex transactions
    c.	Scalability and flexible data models------------------------------------------------- YES                    