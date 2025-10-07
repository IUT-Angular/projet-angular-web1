# projet-angular-web1

## Consignes générales

L'application devra être ergonomique et intuitive.

La bibliothèque MatAngular devra être utilisée pour la mise en place des composants standards.

## Description fonctionnelle de l'application

Bienvenue dans "My Video jet", une application vous permettant de gérer votre cinémathèque.

## Spécifications techniques

Vous allez devoir gérer les entités suivantes :
- User, composé d'un id numérique, d'un login et d'un mot de passe, tous les 2 de type string
- Category, composé d'un id numérique et d'un libellé en chaine de caractères
- Actor, composé d'un id numérique et d'un nom en chaine de caractères
- Movies, composé d'un id numérique, d'un titre en chaine de caractères, d'une catégorie (identifiant de la Category) et une liste d'acteur (identifiants des Actor)
- Rates, composé de l'identifiant du film, de l'identifiant de l'utilisateur et de la note (allant de 0 à 5)

## Description fonctionnelle des pages

### Page de connexion

- La page de connexion est composé d'un champ 'login' ainsi que d'un champ 'mot de passe'.
- Les 2 champs sont obligatoires et tant qu'ils ne sont pas renseigné le bouton de validation du formulaire doit être non cliquable.
- Pour valider la connexion d'un utilisateur, le login et le mot de passe doivent être identiques.
- Une fois connecté, l'utilisateur devra être stocké en LocalStorage afin de connecter automatiquement l'utilisateur à la prochaine utilisation de l'application
- L'accès à toutes les pages devra être soumise à la vérification d'une connexion active

### Template des pages

- Après connexion, sur chaque page vous devez être en capacité de naviguer, via un menu, sur les pages suivantes :
    - page d'accueil
    - ajout d'un film
    - déconnexion 

### Page d'accueil

- La page d'accueil affichera le nom de l'ensemble des films présents à cette adresse : https://68dd25eb7cd1948060ac9cad.mockapi.io/movies
- Au clic sur un film, vous accèderez au détail du film
- Sur chaque film, vous afficherez un bouton "Vu" qui basculera la couleur du titre entre noir et vert à chaque clic
- Sur la page d'accueil vous aurez la possibilité de filtrer les films selon les critères suivants : nom (champ texte), catégorie (liste déroulante), vu (checkbox)
- le titre principal de la page devra être initialisé ainsi : "Bonjour {login}"

### Détail d'un film

- Le détail d'un film vous permettra d'afficher le nom du film, la catégorie du film ainsi que la liste des acteurs
- Vous devrez récupérer la note de l'utilisateur pour le film et lafficher sous forme d'étoile
- L'utilisateur a la possibilité de modifier la note si elle existe ou d'en ajouter une nouvelle

## Ajout d'un film

- Le formulaire d'ajout d'un film doit vous permettre d'ajouter un film en saisissant son nom (donnée obligatoire), une liste d'acteur (donnée facultative) et la catégorie du film (donnée obligatoire)

## Déconnexion

- Au clic sur le bouton de déconnexion, la connexion active de l'utilisateur devra être vidée

## API

- Actor : https://68dd25eb7cd1948060ac9cad.mockapi.io/actors
- Category : https://68dd25eb7cd1948060ac9cad.mockapi.io/categories
- Movie : https://68dd25eb7cd1948060ac9cad.mockapi.io/movies
- Rate : https://68dd25eb7cd1948060ac9cad.mockapi.io/rates

## Consignes

- La partie 1 est à rendre le mercredi 01/10/2025 à 19h30.