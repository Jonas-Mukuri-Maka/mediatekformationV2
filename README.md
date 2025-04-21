# Mediatekformation
## Présentation de l'application origine
![link](https://github.com/CNED-SLAM/mediatekformation)
## Les différentes pages
Voici toutes les pages du back office
### Page Formations (Back Office)
Cette page présente les formations proposées en ligne (accessibles sur YouTube) pour le back office. Elle est accessible en cliquant sur le bouton “Formations” sur le menu de navigation du back office.<br>
La partie du haut contient une bannière (logo, nom du site et titre de la page) ainsi qu’un menu de navigation simplifié (seulement la page actuelle).<br>
Le centre de la page est structuré comme la page “Formations” du front office, avec un affichage en colonne des différentes formations disponibles. Deux boutons sont ajoutés au-dessus de chaque formation :<br>
• Le bouton “Éditer” permet de modifier les informations de la formation concernée (titre, description, vidéo, playlist et catégories).<br>
• Le bouton “Supprimer” permet de supprimer la formation concernée. Lors du clic, un message de confirmation s’affiche, la suppression n'est effective qu’après validation.<br>
Un bouton “Ajouter une nouvelle formation” est situé en haut de la colonne de gauche, et permet d’accéder à la page de création d’une nouvelle formation.<br>
![image](https://github.com/user-attachments/assets/4f133945-a5fc-426b-9a09-ba91b253067c)
## Page Ajout / Modification de Formation
Cette page est accessible depuis la page Admin Formations, soit en cliquant sur “Ajouter une nouvelle formation”, soit sur “Éditer” pour modifier une formation existante.<br>
Elle permet d’ajouter une nouvelle formation à la base de données ou de modifier une formation existante.<br>
La partie centrale est divisée en trois zones :<br>
• La partie gauche permet de saisir le titre de la formation, de sélectionner une playlist (une seule) ainsi que ses catégories (de 0 à plusieurs).<br>
• La partie droite permet de choisir la date de publication (impossible de choisir une date future) et de saisir l’URL de la vidéo.<br>
• La partie inférieure contient un champ de texte pour saisir la description complète de la formation.<br>
Un bouton “Enregistrer” est situé en bas de la page pour valider l’opération.<br>
Dans le cas d’une modification, les champs sont préremplis avec les données existantes de la formation, et le titre de la page passe de “Nouvelle Formation :” à “Modification de Formation :”.<br>
![image](https://github.com/user-attachments/assets/ab18bf42-7ace-4a4e-a666-d2de239a7cae)

### Page Playlists (Back Office)
Cette page permet la gestion des playlists, c’est-à-dire des regroupements de formations, depuis le back office. Elle est accessible via le menu de navigation du back office en cliquant sur “Playlists”.<br>
La bannière et le menu en haut de page sont similaires aux autres pages du back office. Le menu contient uniquement les pages réservées à l’administration.<br>
Un bouton “Ajouter une nouvelle playlist” est placé en haut de la colonne dédiée aux playlists, et permet de créer une nouvelle entrée en renseignant un nom et une description.<br>
La partie centrale reprend la présentation de la page Playlists du front office, à ceci près qu'elle inclut deux actions supplémentaires visibles au-dessus de chaque carte de playlist :<br>
• Le bouton “Éditer” permet de modifier les informations de la playlist (nom et description).<br>
• Le bouton “Supprimer” n’est disponible que pour les playlists ne contenant aucune formation. Lorsqu’il est visible et activé, un message de confirmation s’affiche avant suppression définitive.<br>
![image](https://github.com/user-attachments/assets/ffd6ead8-98d2-4534-8f2a-6fc1d557c694)
## Page de Modification d’une Playlist
Accessible en cliquant sur “Éditer” depuis la page des playlists, cette page permet de modifier les détails d’une playlist existante.<br>
La structure de la page est divisée en deux colonnes :<br>
• À gauche, l’utilisateur peut modifier le nom de la playlist ainsi que sa description.<br>
• À droite, la liste des formations associées à cette playlist est affichée, avec leurs titres respectifs à titre d’information (non modifiables depuis cette page).<br>
Un bouton “Enregistrer” est présent en bas de page pour valider les modifications et les enregistrer dans la base de données.<br>
![image](https://github.com/user-attachments/assets/af9473fa-921f-4515-819d-c99a2fe94930)
## Page d’Ajout d’une Playlist
Cette page s’ouvre en cliquant sur le bouton “Ajouter une nouvelle playlist” dans la section Playlists du back office.<br>
Elle permet la création d’une nouvelle playlist. L’utilisateur y saisit un nom ainsi qu’une description pour la playlist à créer.<br>
Un bouton “Enregistrer” situé en bas de la page permet de finaliser l’ajout et d’enregistrer la nouvelle playlist dans la base de données.<br>
![image](https://github.com/user-attachments/assets/4b0c7a7f-8bba-4347-b490-58c11b18de85)

### Page Catégories (Back Office)
Cette page permet de consulter et gérer les catégories de formations disponibles dans la base de données. Elle est accessible via le bouton “Catégories” dans le menu de navigation du back office.<br>
La partie centrale de la page affiche un tableau structuré en deux colonnes :<br>
• La colonne “Catégories” liste les noms de toutes les catégories existantes,<br>
• La colonne “Actions” permet la suppression d’une catégorie donnée, uniquement si celle-ci n’est associée à aucune formation.<br>
Au-dessus du tableau, une zone de saisie accompagnée d’un bouton “Ajouter” permet de créer une nouvelle catégorie. Le nom renseigné est enregistré dans la base de données, à condition qu’il ne soit pas déjà utilisé.<br>
![image](https://github.com/user-attachments/assets/f4c7a792-89dd-4be8-94f0-955d94183672)

### Page de Connexion (Back Office)
Cette page permet aux utilisateurs autorisés d'accéder à l'interface d’administration du site. Elle est automatiquement affichée lorsqu’un utilisateur tente d’accéder à une page du back office sans être connecté.<br>
La page est composée d’un formulaire de connexion simple situé au centre de l’écran, contenant les champs suivants :<br>
• Un champ “Nom d'utilisateur” pour saisir l’identifiant,<br>
• Un champ “Mot de passe” pour l’authentification sécurisée.<br>
Un bouton “Connexion” permet de valider les informations saisies. En cas d’erreur (identifiants incorrects), un message d’alerte s’affiche pour en informer l’utilisateur.<br>
Une fois la connexion réussie, l’utilisateur est redirigé automatiquement vers la page principale du back office (par défaut, la page Formations).<br>
![image](https://github.com/user-attachments/assets/eec3613b-093d-4b22-aa92-aa3801478400)


## La base de données
La base de données exploitée par le site est au format MySQL.
### Schéma conceptuel de données
Voici le schéma correspondant à la BDD.<br>
![HfvUBfhcN4](https://github.com/user-attachments/assets/2200ca4b-caf9-4f1a-920d-35abdd2e219d)
<br>video_id contient le code YouTube de la vidéo, qui permet ensuite de lancer la vidéo à l'adresse suivante :<br>
https://www.youtube.com/embed/<<<video_id>>>
### Relations issues du schéma
<code>
<strong>formation (id, published_at, title, video_id, description, playlist_id)</strong><br>
id : clé primaire<br>
playlist_id : clé étrangère en référence à id de playlist<br><br>
<strong>playlist (id, name, description)</strong><br>
id : clé primaire<br><br>
<strong>categorie (id, name)</strong><br>
id : clé primaire<br><br>
<strong>formation_categorie (formation_id, categorie_id)</strong><br>
formation_id, categorie_id : clé primaire<br>
formation_id : clé étrangère en référence à id de formation<br>
categorie_id : clé étrangère en référence à id de categorie<br><br>
<strong>user (id, username, roles, password)</strong><br>
id : clé primaire<br>
username : unique<br><br>
<strong>doctrine_migration_versions (version, executed_at, execution_time)</strong><br>
version : clé primaire<br><br>
<strong>messenger_messages (id, body, headers, queue_name, created_at, available_at, delivered_at)</strong><br>
id : clé primaire<br>
queue_name, available_at, delivered_at : indexés<br>
</code>
## Lien vers le site de MediatekFormation
https://mediatekformation86.worldlite.fr/
