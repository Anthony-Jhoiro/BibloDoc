# Scénarios

## Contexte

Dans le cadre du développement de le logiciel BibloDoc, nous avons imaginé plusieurs scénarios pour nous guider dans la façon de concevoir le logiciel. Ici seront présents les scénarios les plus importants, classés par ordre d'occurences (le premier sera sûrement celui que l'on verra le plus, etc...)

## Scénarios

### 0) Connexion

![](../out/scenarios/connexion/Connexion.png)

La connexion est un sous scénario qui revient plusieurs fois dans les autres scénarios. Elle est donc détaillée ici et ne sera qu'évoquer dans les autres scénarios.  
**Connexion :**  
(cf. diagramme de séquence partie connexion)  
Pour se connecter, l'utilisateur doit aller sur la page de connexion où lui seront demandés une adresse mail et un mot de passe.  
Il rentre ses coordonnées, puis le logiciel va rechercher dans la base de données si ces coordonnées sont associées à un compte. Bien entendu, le mot de passe est crypté avant d'être stocké en base de sonnées.  
Si les coordonnées sont bonnes, alors le logiciel atorise la connexion du membre et stocke un token de connexion avec les données du membre.  
Si les coordonnées ne sont pas bonnes (la base de données de trouve aucun compte avec ce mail, ou bien le compte associé au mail n'a pas le même mot de passe que celui rentré), le logiciel renvoie un message d'erreur de connexion, et l'utilisateur est invité à vérifier les informations qu'il a donné et à rentrer les bonnes.  

### 1) Lire un livre libre de droit

![](../out/scenarios/getArtworks/Get_Artworks.png)

(cf. diagramme de séquence partie get free artwork)

**Description :**
Ce scénario dépeint l'histoire de Jean-Michel, retraité passioné des romans de Jules Verne, et qui souhaite lire le tour du monde en 80 jours pour la 32ème fois. Se déplçant en fauteuil roulant motorisé, il est très difficile pour lui de se rendre à la bibliothèque pour lire ce livre. Il est donc heureux d'y avoir accès depuis son ordinateur Packard Bell.

**Acteurs :**
Jean-Michel : 90 ans, ancien bouilleur de cru dans la ville d'Orchie, passionné de romans et plus particulièrement de Jules Verne.

**Prérequis !**
Dans ce scénario, Jean-Michel s'est déjà connecter à son compte utilisateur.


**Étapes de l'oeuvre :**
**1)** Jean-Michel se dirige vers la page des oeuvres libres de droit. Il y trouve une liste gigantesque d'oeuvres et se demande comment peut il retrouver celle qu'il cherche. Heureusement, un petit champs lui demande quelle oeuvre souhaite t-il rechercher. Il rentre alors le titre de l'oeuvre, et au fur et à mesure qu'il tape les caractères, la liste des oeuvres se met à jour pour ne proposer que celle qui contiennent les caractères tapés dans leur titre, et se trie en fonction des ouvres les plus consomées. Il s'arrête donc sur "le tour du", puisqu'apparaît alors en 1ère position le livre qu'il recherche.  

**2)** Jean-Michel, heureux, clique alors sur son roman. La page charge, et le contenu arrive enfin. En en-tête, il voit les informations de l'oeuvre (auteur, date de parution...), puis il peut enfin savourer la lecture du livre en lisant les premières lignes : "En l'année 1872, la maison portant le numéro 7 de saville-row, Burlington Gardens, était habitée par Phileas Fogg..."

**cas d'erreur :**
Il faudra faire attantion à ce que l'application soit la plus intuitive possible. En effet, Jean-Michel n'est pas un habitué de l'informatique (il a un ordinateur Packard Bell).

### 2) Lire une oeuvre protégée
![Add artwork exemple](../out/scenarios/rentAnArtwork/Rent_An_Artwork.png)


**Description**
Jordan est un petit jeune de 31 ans. Il est dans sa dernière étude de médecine pour devenir chirurgien urologue. Les années en médecine sont remplies et il n'a que l'été pour se détendre. L'été dernier, il a découvert cette application lui permettant d'écouter de la musique, il a créer un compte pour écouter ses morceaux préférés : "Bambino" de Dalida et "La Foule" d'Édith Piaf.  
Cette année, encore bien remplie, il a besoin de lire des livres sur l'urologie. Il se dit que se serait une bonne idée de les empruter via le logiciel, car il aura les livre directement dans son téléphone cellulaire portatif. Il part donc en quête d'un livre conseillé par sa professeur de pharmacologie : "Soigner là où ça fait mal", appartenant à la société Elsevier. 

**Acteur :**
Jordan, 31 ans, en dernière années de médecine pour devenir chirurgien urologue, il s"interesse un peu à l'informatique mais aimerait que tout se fasse le plus vite possible pour qu'il perde le moins de temps dans les révisions.

**Prérequis :**
Dans ce scénario, Jordan s'est connecté à son compte membre

**Étapes du scénario :**
**1)** Jordan s'est donc connecté sur son compte. Il va ensuite sur la page de location des oeuvres sous droit. Il voit qu'il y a beaucoup d'oeuvres disponible et décide rechercher grâce au formulaire le livre qu'il recherche. La liste des oeuvres se met à jour en fonction des caractères tapés par Jordan. Une fois tapé : "Soigner là o", il voit son livre recherché en 3ème position. Il clique alors dessus pour y avoir accès.  
**2)** Jordan est redirigé vers une page de paiement qui lui invite à entrer ses coordonnées bancaires. Il rentre donc le numéro de carte, la date de fin de validité, et le cryptogramme. Il doit ensuite rentrer un code envoyé par sa banque par sms. Une fois le code rentré, le site lui indique que le payement est bon, et il est directement redirigé vers le contenu de l'oeuvre qu'il peut enfin lire pour ses révisions.

**Cas d'erreurs**
Pour jordan, la location des livres doit se faire rapidement pour que Jordan aie vite les livre pour réviser. Sinon, il risque de ne jamais relouer les livres sur le logiciel mais sur un concurent.


### 3) Add Artwork

![Add artwork exemple](../out/scenarios/addArtwork/Add_Artwork.png)

#### :page_with_curl: Description :
Anatolia veut mettre son livre en ligne. Elle se rend sur BiblioDoc, se connecte avec son compte. Puis clique sur ajouter une Œuvre, donne son document

#### :busts_in_silhouette: Acteurs :
Client : Anatolia (34 ans, écrivain) vient de terminer sont dernier livre et souhaite le rendre accessible sur la plateforme. Elle souhaite avoir le moins d'informations possible à remplir et avoir des informations simples en face d'elle car elle est peu à l'aise avec la technologie.

#### Prérequis :
Le client doit avoir un compte utilisateur et y être connecté.