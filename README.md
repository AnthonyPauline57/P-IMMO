"# P-IMMO" 

		Découpage 1

En tant que visiteur, je veux visualiser les derniers biens en vente afin de découvrir les nouveautés de l'agence

--> Visualiser les derniers biens en vente
	--> nom des biens, superficie des biens, date de mise en vente des biens, lieu des biens, visualisation des biens, description des biens, prix des biens
°° Création de la Base De Données
°° Création de la Table "bien"
°° Création de la Vue "bien"
°° Création du Controller "bien"
°° Filtre date pour trier les biens


En tant que visiteur, je veux visualiser les détails d'un bien afin de le découvrir

--> Visualiser les details d'un bien
	--> adresse, photos (max6), description, données quantitatives (tailles m², nombre de pièces, nombre de chambres, nombre de salles de bain), liste d'éléments important du bine, avis du conseiller
	--> prix du bien
°° Création de la Table "detailBien"
°° Création de la Vue "detailBien"
°° Création du Controller "detailBien"
°° Utilisation de l'API Google Map pour visualiser le lieu du bien
°° Déploiement

		Découpage 2 

En tant que conseiller, je veux pouvoir me connecter à mon espace sécurisé

--> Se connecter à son espace personnel
	--> mail, mot de passe, nom, prénom
°° Création de la Table "Users"
°° Création de la Vue "inscription"
°° Création de la Vue "connexion"
°° Création du Controller "inscription"
°° Création du Controller "connexion"
°° Crypter le mot de passe
°° Création des différents rôle pour les différents utilisateurs


En tant que conseiller, je veux visualiser mes derniers biens en vente afin de pouvoir travailler dessus

--> Avoir une vue d'ensemble sur les derniers biens en vente
	--> visualisation des biens, visualisation de chaque détail de chaque bien
°° Modification de bien
°° Suppression de bien
°° Création d'une Vue "catalogue"
°° Création d'un Controller "catalogue"
°° Création d'un système de recherche
 

En tant que conseiller, je veux créer un nouveau bien afin d'améliorer sa visibilité

--> Création de nouveaux biens pour améliorer la visibilité
	--> visualisation des biens, visualisation de chaque détail de chaque bien
°° Gérer la visibilité de chaque bien

		Découpage 3

En tant que visiteur, je veux contacter le conseiller en charge d'un bien afin de lui demander des précisions

--> Contacter le conseiller
	--> conseiller du bien, detail du bien, mail du visiteur, mail du conseiller, objet du mail, description du ail, pièce jointe
°° Création d'une Vue "contact"
°° Création d'un Controller "contact"


En tant que conseiller, je veux visualiser les messages envoyés par les acheteurs afin de répondre à leurs questions

--> Visualisation des messages envoyés
	--> nom de l'acheteur, prénom de l'acheteur, titre du bien, lieu du bien
°° Création d'un historique de messages envoyés
°° Création d'un système "question / réponse"


En tant que visiteur, je veux faire une proposition afin d'acheter un bien

--> Proposition d'achat 
	--> moyen de paiement, TVA, prix de la proposition
°° Création de la table "achat"
°° Création de la Vue "achat"
°° Création d'un backend
°° Création du Controller "achat"
	°° Génération des données de paiement
	°° Utilisation de Stripe pour les virements
	°° Affichage des données de paiement


En tant que vendeur, je veux consulter les propositions reçus pour mon bien afin de les étudier

--> Consultation des propositions reçus des acheteurs pour le bien du vendeur
	--> prix proposé de l'acheteur, moyen de paiement, TVA
°° Création d'un système à choix multiple
	°° Acceptation de la proposition
	°° Refus de la proposition
	°° Proposition du vendeur

		Découpage 4 

En tant que vendeur, je veux accéder à mon espace personnel afin de suivre l'avancement de mon dossier

--> Accès à l'epace personnel du vendeur
	--> lien unique, avancement du dossier, nombre de visite, nombre de proposition
°° Création d'un espace personnel
°° Création d'un suivi de dossier


En tant que vendeur, je veux visualiser l'état d'avancement de ma vente afin de contrôler le travail de mon conseiller

--> Visualisation de l'avancement de la vente 
	--> avancement de la vente, nom du conseiller, prénom du conseiller, nombre de visite, nombre de proposition
°° Création d'un système de contact entre vendeur et conseiller


En tant que conseiller, je veux renseigner les visites programmées pour un bien afin de tenir le vendeur au courant

--> Renseigner les visites programmées
	--> date de la visite, heure de la visite, nom du potentiel acheteur, prénom du potentiel acheteur, notification
°° Création d'un système de notification pour que le conseiller alerte le vendeur d'une visite
°° Création d'une Table "planning"
°° Création d'une Vue "planning"
°° Création d'un Controller "planning"

		Découpage 5 

En tant qu'administrateur je veux créer de nouveaux utilisateurs

--> Création de nouveaux utilisateurs 
	--> mail de l'administrateur, mot de passe de l'administrateur, mail du nouvel utilisateur, mot de passe du nouvel utilisateur, rôle
°° Création d'une Table "ajout"
°° Création d'une Vue "ajout"
°° Création d'un Controller "ajout"


En tant qu'administrateur, je veux attribuer un rôle à un utilisateur

--> Attribution d'un rôle à un utilisateur 
	--> nom de l'utilisateur, prénom de l'utilisateur, mail de l'utilisateur, mot de passe de l'utilisateur, rôle de l'utilisateur
°° Création d'un rôle


En tant que vendeur, je veux choisir un mot de passe afin d'accéder à mon espace personnel

--> Attribution d'un mot de passe pour accéder à l'espace personnel du vendeur
	--> mail, mot de passe, envoi de mail qui contiens le mot de passe, nom, prénom
°° Création d'une Table "envoiMail"
°° Création d'une Vue "envoiMail"
°° Création d'un Controller "envoiMail"