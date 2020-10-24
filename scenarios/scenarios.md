# Scénarios

## Contexte

Dans le cadre du développement de le logiciel BibloDoc, nous avons imaginé plusieurs scénarios pour nous guider dans la façon de concevoir le logiciel. Ici seront présents les scénarios imaginés, classés par ordre d'importance (le premier sera sûrement celui que l'on verra le plus, etc...)

## Scénarios

### 0) Connexion 

#### :mag: Description :
Ce scénario est le scénario de connexion. Il conte l'histoire de Jamy Gourmaud, récent YouTuber, qui recherche des musiques libres de droit, et qui doit donc se connecter.

#### :busts_in_silhouette: Acteurs :
Jamy Gourmaud, 56 ans, animateur de télévision et journaliste, récent YouTuber.

#### :wrench: Prérequis :
Aucun prérequis dans ce scénario

#### :file_folder: Données :
Jamy devra entrer son identifiant ou son adresse mail ainsi que le mot de passe qu'il a créé pour son compte.

#### :clipboard: Étapes du scénario:
1. Jamy charge la page d'accueil du site.  
2. Jamy clique sur le lien : "se connecter"
3. Jamy est redirigé vers la page de connexion
4. Jamy rentre son identifiant et son mot de passe.
5. Jamy clique sur le bouton "se connecter" pour valider le formulaire
6. Jamy est connecté
7. Jamy est content

#### :page_with_curl: Scénario abstrait :
(cf. diagramme de connexion)  
1. l'utilisateur charge la page d'accueil du site.  
2. l'utilisateur clique sur le lien : "se connecter"
3. l'utilisateur est redirigé vers la page de connexion
4. l'utilisateur rentre son identifiant et son mot de passe.
5. l'utilisateur clique sur le bouton "se connecter" pour valider le formulaire
6. **Si les données sont bonnes** l'utilisateur est connecté
6bis. **Si l'adresse mail ou l'identifiant ou le mot de passe n'est pas bon** l'utilisateur est averti de sa faute et est invité à entrer à nouveau ses coordonnées

### 1) Lire un livre libre de droit

(cf. diagramme getArtwork)

#### :mag: Description :
Ce scénario dépeint l'histoire de Jean-Michel, retraité passioné des romans de Jules Verne, et qui souhaite lire le tour du monde en 80 jours pour la 32ème fois. 

#### :busts_in_silhouette: Acteurs :
Jean-Michel : 90 ans, ancien bouilleur de cru dans la ville d'Orchie, passionné de romans et plus particulièrement de Jules Verne. Il se déplace en fauteuil roulant motorisé, il est très difficile pour lui de se rendre à la bibliothèque pour lire ce livre. Il est donc heureux d'y avoir accès depuis son ordinateur Packard Bell.

#### :wrench: Prérequis :
Dans ce scénario, Jean-Michel s'est déjà connecter à son compte utilisateur.

#### :file_folder: Données :
Jean-Michel devra entrer le titre, ou une partie du titre, d'une oeuvre, et ressortira le contenu et les informations de l'oeuvre.

#### :clipboard: Étapes du scénario:
1. Jean-Michel se dirige vers la page des oeuvres libres de droit. Il y trouve une liste gigantesque d'oeuvres et se demande comment peut il retrouver celle qu'il cherche. Heureusement, un petit champs lui demande quelle oeuvre souhaite t-il rechercher. Il rentre alors le titre de l'oeuvre, et au fur et à mesure qu'il tape les caractères, la liste des oeuvres se met à jour pour ne proposer que celle qui contiennent les caractères tapés dans leur titre, et se trie en fonction des ouvres les plus consomées. Il s'arrête donc sur "le tour du", puisqu'apparaît alors en 1ère position le livre qu'il recherche.  

2. Jean-Michel, heureux, clique alors sur son roman. La page charge, et le contenu arrive enfin. En en-tête, il voit les informations de l'oeuvre (auteur, date de parution...), puis il peut enfin savourer la lecture du livre en lisant les premières lignes : "En l'année 1872, la maison portant le numéro 7 de saville-row, Burlington Gardens, était habitée par Phileas Fogg..."  

#### :page_with_curl: Scénario abstrait :
1. l'utilisateur va à la page de recherche d'une oeuvre en libre service  
2. l'utilisateur rentre le titre de l'oeuvre dans la barre de recherche  
2bis. Ou bien l'utilisateur recherche l'oeuvre parmis celles en liste sur la page  
3. L'utilisateur clique sur l'oeuvre  
4. l'utilisateur va sur la page de consommation de l'oeuvre et peut la consommer

#### :x: Cas d'erreur :
Il faudra faire attention à ce que l'application soit la plus intuitive possible. En effet, Jean-Michel n'est pas un habitué de l'informatique (il a un ordinateur Packard Bell).

### 2) Lire une oeuvre protégée

#### :mag: Description :
Jordan est un petit jeune de 31 ans. Il est dans sa dernière étude de médecine pour devenir chirurgien urologue. Les années en médecine sont remplies et il n'a que l'été pour se détendre. L'été dernier, il a découvert cette application lui permettant d'écouter de la musique, il a créer un compte pour écouter ses morceaux préférés : "Bambino" de Dalida et "La Foule" d'Édith Piaf.  
Cette année, encore bien remplie, il a besoin de lire des livres sur l'urologie. Il se dit que se serait une bonne idée de les empruter via le logiciel, car il aura les livre directement dans son téléphone cellulaire portatif. Il part donc en quête d'un livre conseillé par sa professeur de pharmacologie : "Soigner là où ça fait mal", appartenant à la société Elsevier. 

#### :busts_in_silhouette: Acteur :
Jordan, 31 ans, en dernière années de médecine pour devenir chirurgien urologue, il s"interesse un peu à l'informatique mais aimerait que tout se fasse le plus vite possible pour qu'il perde le moins de temps dans les révisions.

#### :wrench: Prérequis :
Dans ce scénario, Jordan s'est connecté à son compte membre

#### :file_folder: Données :
Jordan devra entrer le titer de l'oeuvre qu'il recherche et ses coordonnées bancaires pour effectuer la transaction. Il aura alors accès aux informations et contenu de l'oeuvre.

#### :clipboard: Étapes du scénario concret :
1. Jordan s'est donc connecté sur son compte. Il va ensuite sur la page de location des oeuvres sous droit. Il voit qu'il y a beaucoup d'oeuvres disponible et décide rechercher grâce au formulaire le livre qu'il recherche. La liste des oeuvres se met à jour en fonction des caractères tapés par Jordan. Une fois tapé : "Soigner là o", il voit son livre recherché en 3ème position. Il clique alors dessus pour y avoir accès.  

2. Jordan est redirigé vers une page de paiement qui lui invite à entrer ses coordonnées bancaires. Il rentre donc le numéro de carte, la date de fin de validité, et le cryptogramme. Il doit ensuite rentrer un code envoyé par sa banque par sms. Une fois le code rentré, le site lui indique que le payement est bon, et il est directement redirigé vers le contenu de l'oeuvre qu'il peut enfin lire pour ses révisions.

#### :page_with_curl: Scénario abstrait :
1. l'utilisateur va à la page de recherche d'une oeuvre à louer
2. l'utilisateur rentre le titre de l'oeuvre dans la barre de recherche
2bis. Ou bien l'utilisateur recherche l'oeuvre parmis celles en liste sur la page
3. L'utilisateur clique sur l'oeuvre
4. L'utilisateur est redirigé vers la page d'achat de l'oeuvre
5. l'utilisateur rentre ses coordonnées bancaires
6. **Si les coordonnées bancaires sont bonnes** l'utilisateur revient automatiquement sur la page de consommation de l'oeuvre
6bis. **Si les coordonnées bancaires ne sont pas bonnes** l'utilisateur est redirigée vers la page de recherche d'ouvres avec un message d'erreur

#### :x: Cas d'erreurs :
1. Si Jordan tape le mauvais code bancaire, une réponse négative est renvoyée au logiciel. Le logiciel le redirige vers la page d'accueil.


