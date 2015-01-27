# Spécification fonctionnelle (SFD V.0.1)


## Introduction :book:





	* Ajouter des postes pour les élections. Par défaut, 4 postes sont déja crée :
		* :bust_in_silhouette: Président
		* :bust_in_silhouette: Vice-Président
		* :bust_in_silhouette: Secrétaire
		* :bust_in_silhouette: Trésorier
	* Valider ou invalider les membres.
	* Suppression et mise en forme des lois et leurs variations.




L'utilisateur entre, côté client une phrase secrétée qui génère une clé public, avec là qu'elle, il est identifié côté serveur. Le serveur n'a plus besoins de son mail et mot de pass, de se fait ça enlève le problème de sécurité côté serveur, il y a plus besoin de le pirater, car il ne garde plus aucune donnée sensible concernant le client.

Si l'utilisateur doit faire une modification exigent son authentification, un message est signé côté client, le serveur na plus qu'a vérifier la validité de la signature pour identifier que c'est bien l'utilisateur qui a fait la demande.

:arrow_right: Tout le compte est régénérer à partir de la phrase secrète à chaque utilisation et les données sont traitées en local avec JavaScript.

:arrow_right: Un nouveau code pin est demander a la connexion pour un cryptage symétrique de la phrase secrète pendant toute la durée de la session locale. le code pin n'est stocké nulle part.

:arrow_right: Tout le systeme cryptographique reste invisible pour le client final.

***


* :construction: Travail en cours




### :green_book: Application Client

> L'application client, affiche et accepter les inscriptions, authentification, vote, ajout de règles et leur révision.

* **Accueil**
	* **Intro :**
	* **Accès :**
	* **Maquette :**
	* **Informations :**
	* **Actions possibles :**
	* **Règles de gestion :**

### :closed_book: Application Admin

> L'application admin, contrôle et modifie toutes les données ajouter par les membres.

* **Accueil**
	* **Intro :**
	* **Accès :**
	* **Maquette :**
	* **Informations :**
	* **Actions possibles :**
	* **Règles de gestion :**

### :blue_book: Api serveur

> Api dédiée en PHP avec le protocole JSON RPC 2, permettant la démocratie en temps-réel.

* :construction: Travail en cours


# Q

:interrobang: Secrétaire = Admin ou élu ado ?

:interrobang: Rôle du président dans l'api ?

:interrobang: Informations fournies par les membres ? Ex : Nom, Prenom…

:date: *Lundi 26 Janvier 2015*