# Biblo Doc'


![image](https://images.adagio.com/images2/custom_blends/117606.jpg)

Date : 5 octobre 2020 

Auteurs : Kilian Debraux et Anthony Quéré 

Nom du groupe : Golden Cookie Corp 

Confidentialité : ###



## objectifs  
L’idée du logiciel est née du besoin de plusieurs bibliothèques de numériser leur contenu. D’après la demande client, l’application  doit pouvoir centraliser les oeuvres de toutes bibliothèques, ainsi que de sécuriser les oeuvres sous licences (pas de vol physique) pour pouvoir mettre en commun la liste des oeuvres qu'ils possèdent.  

## description (solution) :
Notre solution : un logiciel permettant de partager les oeuvres de l'association en fonction de son droit (domaine publique ou sous brevet) aux membres des différentes bibliothèques et aussi à ces membres de proposer différentes oeuvres pour enrichir la base d'oeuvres.  
Le logiciel prendre en compte les domaines des oeuvres (privé/public), la sécurité (chiffrage des oeuvres protégées), ainsi que la vérification des oeuvres proposées par les membres  

## contexte : 
Ce logiciel sert à centraliser la gestion des oeuvres de plusieurs bibliothèques, ce qui permet de faire des économies car il représente un seul service pour plusieurs bibliothèques.  
De plus, une nouvelle bibliothèque pourra se greffer au logiciel sans aucun problème.  


## Glossaire
- bibliothèque numérique = application disponible au public (ex: site web)
- gestion decentralisée = une application pour plusieurs bibliothèques
- membre = prévoir une authentification et une gestion de compte
- numériser = le membre fournis lui même les fichiers des œuvres
- empreint = ???
- location = paiement en ligne ?
- œuvres de domaine public
    - Copies non chiffrés
    - Accessible pour tout le monde
    - Il peut y avoir autant de copi que de membre
- œuvres du domaine privé
    - maximum 3 fois plus de copies que de licence d'exploitation
    - notions de droit d'accessibilité
    - chaque œuvre est chiffrée par une clef différente avec une date de validité
    - fin de validité = suppression automtique de la copie
- œuvre = 1 fichier contenant l'œuvre et 1 fichier JSON avec les détails
- index des œouvre mis à jour en temps réel
- 4 rubriques / répertoires ~= page web
    - fond commun = tout ce qui est libre de droit
    - emprunts = œuvres sous droit empruntées par le membre actif et chiffré avec sa clef
    - séquestre = œuvres sous droit
    - à modérer = œuvres proposées par les membres et non validées
- bibliothécaires = authentification et administration des comptes de bibliothécaires
    - controllent les œuvres dites "à modérer"
    - complètent des données :
        - auteurs = il peut y avoir plusieurs auteurs
        - éditeurs = il peut y avoir plusieurs éditeurs
        - langue
        - pays d'origine
        - date de publication
        - droits
        - catégorie de l'œuvre
        - format du support
        - status de l'œuvre (domaine public ou non) qui place l'œuvre dans la bonne rubrique et gère les droits d'accès

type = format du support
sous type = catégorie de l'œuvre
formats et catégories :
    - Livre
        - BD
        - Enfants
        - Romans
        - Education
        - Loisir
        - Culture
        - Sante
        - ...
    - Musique
        - Classique
        - Jazz/Funk/Saoul
        - Pop
        - Metal
        - ...
    - Vidéos
        - SF
        - Histoire
        - Série
        - Documentaire
        - ...
    
## Questions
Œuvres privées : une clef de chiffrement par œuvre, par copie ou pas user ?  
Plus de détails sur les droits d'accessilité ?
Pourquoi utiliser un fichier JSON et non pas une base de donnée ?
Comment sont gérées les dates de validité ?
Pourquoi les repertoires "fond_commun" et "séquestre" ne contiennent qu'une partie des œuvres ?
Location : Si il y a des paiments comment sont ils gérés
Qu'est-ce qu'une licence d'exploitation ?
