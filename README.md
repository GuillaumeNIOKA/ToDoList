To-DO List

Description de l'application :

L'application To-Do List permet aux utilisateurs de créer une tâche, de visualiser son statut et de la modifier. Plus tard, elle permettra de donner à chaque tâche une description et une date d'échéance. De plus, l'application proposera de rechercher et de filtrer les tâches.

Tâches à réaliser :

-Installer Symfony ; configurer le projet Symfony, configurer la connexion à SQL Server avec Doctrine
-Installer Angular ; Configurer les environnements pour communiquer avec le back-end Symfony


Développement du Back-end :

1 - Modéliser la base de données : Créer la table 'tasks' avec les colonnes id, title, description, due_date, status, created_at, updated_at.

2 - Création des entités et repositories : Créer l'entité task avec Doctrine, correspondant  à la table tasks. Générer les repositories nécessaires pourles opérations CRUD.

3 - Développement des Endpoints RESTful :
	-Récupérer la liste de toutes les tâches avec options de filtrage avec GET:api/tasks.
	-Récupérer les détails d'une tâche spécifique avec GET/api/tasks/{id}.
	-Créer une nouvelle tâche avec POST/api/tasks
	-Mettre à jour une tâche existante avec PUT/api/tasks/{id} ou PATCH
	- Supprimer une tache avec DELETE/api/tasks{id}

4 - Validation et sécurité : Implémenter de svalidations pour les champs obligatoires et les formats de données.


Développement du front-end avec Angular

1 - Structure de l'application :  configurer les routes principales (liste des tâches, création/édition de tâche, page 404), créer les composants nécessaires : TaskListComponent, TaskFormComponent, TaskDetailComponent, NavbarCoponent.

2 -  Servicdes et Communication avec l'API : Développze un service TaskService pour gérer les appels HTTP vers le back-end Symfony, implémenter les méthodes getTasks(), getTaskById(id), createTask(task), updateTask(id, task), deleteTask(id).

3 - Interface utilisateur. :Créer une inerface permettant de lister les tâches avec options de tri et filtreage, formulaires réactifs pour créer et éditer des tâches avec validations en temps réel et boutons d'action pour modifier, supprimer et marquer les tâches comme terminées.

Tests et validation :

1 - Tests back-end :  Ecrire des tests unitaires avec PHPUnit pour vérifier les fonctionnalités des endpoints et tester les validations et les réponses HTTP appropriées.

2 - Tests front-end : Écrire des tests unitaires pour les composants et services Angular et effectuer des tests end-to-end avec Cypress ou Protractor pour simuler les interactions utilisateur.

3 - Débogage et Optimisation : Identifier et corriger les bugs éventuels et optimiser l'application.
