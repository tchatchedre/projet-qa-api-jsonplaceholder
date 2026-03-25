# Stratégie de test – API Users (JSONPlaceholder)

## 1. Objectif
Valider le comportement principal du service `Users` exposé par l'API JSONPlaceholder, avec un focus sur la lecture de ressources, la création de données et la robustesse minimale des réponses.

## 2. Portée
### Inclus
- disponibilité des endpoints principaux,
- code de statut HTTP,
- structure générale de la réponse JSON,
- présence des champs majeurs,
- comportement sur identifiant inexistant,
- simulation de création d'un utilisateur.

### Exclu
- authentification,
- sécurité avancée,
- performance de charge,
- persistance réelle en base,
- gestion complète des validations métier.

## 3. Risques visés
- endpoint disponible mais structure de réponse incomplète,
- données obligatoires absentes,
- comportement ambigu sur ressource inexistante,
- acceptation de données incohérentes sans validation,
- confusion entre API de démonstration et API de production.

## 4. Approches utilisées
### 4.1 Test fonctionnel manuel
Construction de scénarios à partir du besoin attendu d'un service Users.

### 4.2 Test exploratoire ciblé
Ajout de vérifications autour des erreurs probables :
- utilisateur inexistant,
- payload partiel,
- valeurs manifestement invalides.

### 4.3 Contrôles automatisés légers
Utilisation de Postman pour automatiser des vérifications simples :
- statut HTTP,
- réponse JSON,
- présence des propriétés attendues.

## 5. Critères d'entrée
- API publique accessible,
- endpoints disponibles,
- environnement Postman prêt.

## 6. Critères de sortie
- cas de test rédigés,
- exécution principale réalisée,
- observations documentées,
- collection Postman exportée,
- dépôt GitHub mis à jour.

## 7. Priorités de test
### Priorité haute
- `GET /users`
- `GET /users/1`

### Priorité moyenne
- `POST /users`

### Priorité informative
- `GET /users/999`

## 8. Outils
- Postman
- Excel
- GitHub

## 9. Livrables
- stratégie de test,
- cas de test,
- rapport d'observations / anomalies,
- collection Postman,
- README de projet.
