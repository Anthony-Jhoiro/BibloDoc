# Biblo Doc'


![image](https://images.adagio.com/images2/custom_blends/117606.jpg)

Date : 5 octobre 2020 

Auteurs : Kilian Debraux et Anthony Quéré 

Nom du groupe : Golden Cookie Corp 

Confidentialité : ###



## objectifs  
L’idée du logiciel est née du besoin de plusieurs bibliothèques de numériser leur contenu. D’après la demande client, l’application  doit pouvoir centraliser les oeuvres de toutes bibliothèques, ainsi que de sécuriser les oeuvres sous licences (pas de vol physique) pour pouvoir mettre en commun la liste des oeuvres qu'ils possèdent.

## description (solution) :
Notre solution : un logiciel permettant de partager les oeuvres de l'association en fonction de son droit (domaine publique ou sous brevet) aux membres des différentes bibliothèques et aussi à ces membres de proposer différentes oeuvres pour enrichir la base d'oeuvres. Le logiciel prendre en compte les domaines des oeuvres (privé/public), la sécurité (chiffrage des oeuvres protégées), ainsi que la vérification des oeuvres proposées par les membres

## contexte : 



## Glossaire
- bibliothèque numérique = application disponible au public (ex: site web)
- gestion decentralisée 
- membre = prévoir une authentification et une gestion de compte
    - chaque membre a une clef de chiffrement
- numériser
- empreint
- œuvres de domaine public
    - Il peut y avoir autant de copi que de membre
- œuvres du domaine privé
    - maximum 3 fois plus de copies que de licence d'exploitation
    - chaque œuvre est chiffrée par une clef différente avec une date de validité
    - fin de validité = suppression automtique de la copie
- œuvre = 1 fichier contenant l'œuvre et 1 fichier JSON
- index des œouvre mis à jour en temps réel
- 4 rubriques / répertoires
    - fond commun
    - emprunts = œuvres sous droit empruntées par un membre et chiffré avec sa clef
    - séquestre = ??
    - à modérer = œuvres proposées par les membres et non validées
- bibliothécaires
    - controllent les œuvres dites "à modérer"
    - complètent des données :
        - auteurs
        - éditeurs
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
Œuvres privées : une clef de chiffrement par œuvre ou par copie ?
Location : payante ou non ?
Qu'est-ce qu'une licence d'exploitation ?
