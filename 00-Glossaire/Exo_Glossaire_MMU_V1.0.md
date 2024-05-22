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
1.	Quel est l’environnement à installer pour exécuter un script PHP ? Citer 2 exemples de logiciels permettant ce contexte
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
12.	Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP
13.	Quelle est la différence entre les instructions « require » et « include » en PHP
14.	Comment effectuer une redirection en PHP ?
                - header()

15.	Définir la partie « front-end » et « back-end » d’une application
16.	Définir le contrôle de version ? Qu’est-ce que Git ?
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
21.	Définir JSON. Dans quel contexte ce format est-il utilisé ? 
22.	Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?
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
                On peut exécuter en l’affectant à une variable, en l’auto-invoquant ou en l’utilisant dans un évènement.

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
40.	Qu’est-ce qu’une grille de mise en page ?
41.	Qu’est-ce que la notion d’affordance en UX Design ?
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

50.	Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple
    - Étendre une classe consiste à créer une classe mère qui regroupe des classes enfants. Cela permet aux classe enfant d’hériter des attributs de la classe mère.
    Ex : On crée une classe mère “Personne” et deux classes enfant “Acteur” et “Réalisateur”, on a plus qu’à déclarer les attributs 
        (nom, prenom, sexe, age) une seule fois dans la classe “Personne” et les deux classes enfant hériteront de ses attributs.

51.	Définir l’opérateur de résolution de portée
52.	Définir une méthode / propriété statique
53.	Définir le polymorphisme en POO

54.	Définir une méthode / classe abstraite ?
    - Une méthode abstraite peut seulement être déclaré par son nom ou ses paramêtres (signature).
    - Une classe abstraite est une classe qui ne peut être instanciée. 
    Si une classe contient une méthode abstraite, elle doit elle aussi devenir une classe abstraite

55.	Définir le chaînage de méthodes

56.	Qu’est-ce que la méthode __toString() ? Existe-t-il d’autres méthodes « magiques »
    - La méthode magique **toString permet de passer en chaîne de caractères différents attributs de la classe, elle peut être appelée en utilisant $this. 
    Il existe d’autres méthodes magiques (**construct, **destruct, __call et plein d’autres).

57.	Qu’est-ce qu’un « autoload » ?
    - Un autoload est un auto-chargement de classe, il permet de charger plusieurs classes d’un programme au sein d’un seul et même fichier.

58.	Comment appelle-t-on en français les « getters » et les « setters » ?
    - es getters sont des accesseurs et les setters sont des mutateurs.

59.	Qu’est-ce que la sérialisation en PHP ? 
    - La sérialisation est une technique qui à pour but de transferer des valeurs entre scripts sans qu'elles perdent leurs structure ou type.

## Architecture 
60.	Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur. Définir l’acronyme de ce type de requête. Si on ajoute un « S » à cet acronyme, expliquer la différence
61.	Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern
62.	Qu’est-ce que l’architecture MVC ?
63.	Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?
64.	Quels sont les avantages de l’architecture MVC ?
65.	Existe-t-il des variantes à l’architecture MVC ?
66.	Qu’est-ce qu’une API ? Définir l’architecture REST

## Modélisation - Base de données
67.	Qu’est-ce que la modélisation de données ? Définir la méthode Merise

68.	Quelles sont les 3 étapes principales de la méthode Merise ? 
    a.	Analyse, conception et réalisation
    b.	Planification, exécution et contrôle
    c.	Création, modification et suppression

69.	Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?
    - Le MCD repose sur les notions d'entité et d'association et sur les notions de relations. 
    Le modèle conceptuel des données s'intéresse à décrire la sémantique du domaine (entity/relationship en anglais).

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
95.	Qu’est-ce que la faille XSS ? Comment s’en prémunir ?
96.	Qu’est-ce que la faille CSRF ? Comment s’en prémunir ?
97.	Définir l’attaque par force brute et l’attaque par dictionnaire
98.	Existe-t-il d’autres failles de sécurité ? Citer celles-ci et expliquer simplement leur comportement
99.	A quoi servent l’authentification et l’autorisation dans un contexte d’application web ?
100. Définir la notion de hachage d’un mot de passe et citer des algorithmes de hachage
101. Qu’est-ce qu’une politique de mots de passe forts ?
102. Qu’est-ce que l’hameçonnage ?
103. Définir la « validation des entrées »

## RGPD
104. Qu’est-ce que le RGPD ?
105. Quel est son objectif principal ?
106. Quelle est la date d’entrée en vigueur du RGPD ?
107. Quelles sont les sanctions possibles en cas de non-respect du RGPD ?
108. En France, quel est l’autorité administrative qui s’occupe de faire appliquer le RGPD ?
109. Quel est le consentement valide selon le RPGD ?
110. Qu’est-ce qu’une politique de confidentialité ?
111. Quelle est la durée de conservation maximale des données personnelles selon le RGPD ?
112. Quels sont les droits des utilisateurs selon le RGPD ?
113. Qu’est-ce que le principe de minimisation des données selon le RGPD ?

## SEO
114. Qu’est-ce que le SEO ? 
115. Quel est l’objectif principal du SEO ?
116. Existe-t-il plusieurs types de référencement ? Lesquels ?
117. Qu’est-ce que la densité de mots-clés en SEO ?
118. Qu’est-ce qu’une balise « alt » ?
119. Qu’est-ce que la balise « meta description » ?
120. Qu’est-ce que le « nofollow » en SEO ?
121. Quelle est l'importance du contenu de qualité pour le référencement d'un site web ?
122. Pourquoi est-il important d'utiliser des balises de titre (h1, h2, h3, etc.) de manière structurée ?
123. Quelle est la recommandation pour les URL d'un site web bien référencé ?
124. Qu'est-ce que le maillage interne et pourquoi est-il important pour le référencement ?
125. Qu'est-ce que l'optimisation des images pour le référencement ?
126. Qu'est-ce qu'un plan de site (sitemap) et pourquoi est-il important pour le référencement ?

## Gestion de projets - DevOps
127. Qu’est-ce que la gestion de projet ?	
128. Qu’est-ce qu’une méthode Agile de gestion de projet ? 
129. Expliquer la méthode MoSCoW en quelques lignes et citer ses avantages
130. A quoi sert la méthodologie MVP ? Citer les caractéristiques clés
131. Qu’est-ce que la planification itérative ?
132. Citer 3 méthodes Agiles dans le cadre d’un projet informatique
133. Qu’est-ce qu’une réunion de revue de projet ?
134. Qu’est-ce qu’un livrable dans un projet ? 
135. Quels sont les 3 piliers SCRUM ? Définir chacun d’entre eux
136. Qu’est-ce que le DevOps et quel est son objectif principal ?
137. Qu’est-ce que l’intégration continue ? 
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
    a.	Add interactive behavior and dynamic content
    b.	Define the layout and design of web pages
    c.	Handle server-side operations
2)	Which programming language is primarily used for server-side web development ?
    a.	PHP
    b.	JavaScript
    c.	HTML
3)	What is the purpose of a web browser ?
    a.	To render and display web pages
    b.	To execute serve-side code
    c.	To manage databases
4)	What is the difference between GET and POST methods in HTTP ?
    a.	GET retrieves data from a server, while POST submits data to a server
    b.	GET submits data to a server, while POST retrieves data from a server
    c.	GET and POST methods are interchangeable
5)	What is the purpose of version control systems (e.g., Git) in web development ?
    a.	To track changes and manage collaborative development
    b.	To optimize website loading speed
    c.	To handle server-side scripting
6)	What is the purpose of a framework in web development ?
    a.	To provide a structured environment for building web applications
    b.	To handle network protocols and data transfer
    c.	To create visual designs and layouts for websites
7)	What does NoSQL stand for ?
    a.	Not Only SQL
    b.	Non-Structured Query Language
    c.	New Object-Oriented Language
8)	Which of the following is a characteristic of NoSQL databases ?
    a.	Strict schema enforcement
    b.	Support for complex transactions
    c.	Scalability and flexible data models