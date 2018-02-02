# TodoMVC
Exercice basé sur le site todomvc.com

## User stories
Définition des actions de l'utilisateur :
- [ ] User peut ajouter une tâche
- [ ] User peut valider une tâche
- [ ] User peut supprimer une tâche
- [ ] user peut afficher les tâches réalisées
- [ ] User peux afficher les tâches à réaliser
- [ ] User peux supprimer toutes les tâches réalisées

## Mise en place du projet
Etapes à suivre pour préparer PMDtodo :
- [ ] Initier un serveur NodeJS
- [ ] Configurer la BDD MongoDB
- [ ] Créer une route `Front` pour afficher un fichier `Index` dans le dossier `www`
- [ ] Créer une route `API` qui renvoie en `json` l'objet `{ msg: 'Hello API' }`

## Configurer la base de données
Le but est de définir le/les modèle(s) de données à utiliser pour l'application.
- 1. Combien d'informations faut-il enregistrer pour une tâche ?
- 2. Comment une tâche est validée ?
- 3. Comment une tâche est supprimée ?
- 4. Comment les tâches sont filtrées ?

### 1. Combien d'informations faut-il enregistrer pour tâche ?
Il faut deux informations :
- _id : string
- state : boolean
- content : string

### 2. Comment une tâche est validée ?
Quand le `state` est égal à `true`.

### 3. Comment une tâche est supprimée ?
Si l'état est égal à `true` : supprimer l'objet de la BDD.
- Connaître le `_id` de l'objet
- Créer une route `API` pour supprimer l'objet de la BDD

### 4. Comment les tâches sont filtées ?
Je dois sélectionner tous les objets et n'afficher que ceux dont le `state` vaut `true` ou `false`.
- Créer une route `API` pour sélectionner les tâches
