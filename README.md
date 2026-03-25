# Projet QA – API Testing avec JSONPlaceholder

## Contexte

Ce projet simule une mission QA autonome orientée **tests d'API** sur un service de gestion d'utilisateurs.
Le support de test utilisé est **JSONPlaceholder**, une API publique de démonstration conçue pour le test et le prototypage.

API cible : https://jsonplaceholder.typicode.com/users

## Objectif

Montrer une capacité à :
- analyser un besoin fonctionnel côté API,
- concevoir des cas de test manuels,
- exécuter des requêtes API via Postman,
- documenter les constats,
- structurer le travail sur GitHub comme dans une vraie mission QA.

## Méthodologies utilisées

Ce projet combine plusieurs approches QA :

### 1. Organisation de travail : approche Agile légère inspirée Kanban
Le travail est découpé par livrables :
- stratégie de test,
- cas de test,
- exécution API,
- constats / anomalies,
- publication GitHub.

### 2. Approche de test basée sur les risques
La priorité a été donnée aux points critiques :
- disponibilité des endpoints,
- structure des réponses JSON,
- cohérence des données obligatoires,
- comportement sur identifiant inexistant,
- comportement lors d'une création de ressource.

### 3. Test fonctionnel manuel d'API
Les scénarios ont été conçus à partir du comportement attendu d'un service "Users" :
- lecture de la liste des utilisateurs,
- lecture d'un utilisateur par identifiant,
- création d'un utilisateur,
- vérification des champs clés d'une réponse.

### 4. Vérifications automatisées légères
Une collection Postman est fournie avec des tests simples automatisés :
- vérification du code de statut,
- vérification du type de contenu JSON,
- vérification de la présence de champs attendus,
- contrôle basique de la taille de collection.

## Outils utilisés

- **Postman** : exécution des requêtes API et contrôles automatisés simples
- **Excel** : cas de test et journal de constats / anomalies
- **GitHub** : publication et présentation du projet
- **JSONPlaceholder** : API publique utilisée comme support de test

## Livrables du projet

- `README.md`
- `docs/Test_Strategy_API_JSONPlaceholder.md`
- `docs/User_Stories_API.md`
- `test-cases/Test_Cases_API_JSONPlaceholder.xlsx`
- `bug-reports/API_Findings_and_Bug_Report.xlsx`
- `postman/JSONPlaceholder_Users_Collection.json`

## Périmètre testé

### Endpoints couverts
- `GET /users`
- `GET /users/1`
- `GET /users/999`
- `POST /users`

## Résumé du travail réalisé

- conception d'une stratégie de test ciblée API,
- rédaction de cas de test couvrant cas nominaux, cas limites et erreurs,
- préparation d'une collection Postman,
- formalisation d'observations QA dans un rapport dédié.

## Important

Ce projet repose sur une **API réelle de démonstration**.
Certaines observations décrites dans le rapport doivent être lues comme des **écarts par rapport à une API de production** et non comme des défauts bloquants dans le contexte d'une API fake.

## Ce que ce projet permet de démontrer

- compréhension du test d'API,
- capacité à structurer un projet QA de manière autonome,
- aptitude à combiner plusieurs outils et approches dans un même projet,
- logique de documentation claire et exploitable.

---
Projet QA autonome – pratique du test logiciel côté API
