# User stories – API Users

## User Story 1
En tant qu'utilisateur d'une application consommatrice d'API, je veux récupérer la liste des utilisateurs afin d'afficher un annuaire.

### Critères d'acceptation
- la requête `GET /users` retourne un code 200,
- la réponse est au format JSON,
- la réponse contient une liste d'utilisateurs,
- chaque utilisateur possède au minimum les champs `id`, `name`, `username`, `email`.

## User Story 2
En tant qu'utilisateur, je veux récupérer le détail d'un utilisateur à partir de son identifiant afin d'afficher sa fiche.

### Critères d'acceptation
- la requête `GET /users/1` retourne un code 200,
- la réponse contient l'utilisateur demandé,
- l'objet retourné contient les champs clés attendus.

## User Story 3
En tant que consommateur d'API, je veux connaître le comportement du service lorsqu'un identifiant inexistant est demandé afin de gérer correctement les cas d'erreur.

### Critères d'acceptation
- le comportement doit être explicite et documenté,
- le résultat doit permettre au client de distinguer une ressource trouvée d'une ressource absente.

## User Story 4
En tant que consommateur d'API, je veux créer un utilisateur afin de vérifier le fonctionnement nominal d'un endpoint de création.

### Critères d'acceptation
- la requête `POST /users` accepte un payload JSON,
- la réponse confirme la création simulée,
- les champs envoyés sont présents dans la réponse.
