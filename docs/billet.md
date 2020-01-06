# Titre

## Cartouche d'identification

 - Manifestation : CodeursEnSeine 2019
 - Lieu : Kindarena
 - Conférence : Montée de version sans interruption
 - Horaire de la conférence : 14h30
 - Durée de la conférence : 50 minutes
 - Conférencier(s) :
   - Nelson Dionisi, Lead Developer chez Mirakl (https://github.com/ndionisi, https://www.linkedin.com/in/nelson-dionisi-84a00472/)
 - Audience : ~100 personnes
 - Auteur du billet : Thibaut EMION
 - Mots-clés : SaaS, Continuous Delivery, Migrations

## Support
 - Lien vers le support (diapos) présenté en conférence
 - Nombre de diapos du support :
 - Plan du support :

## Résumé

Cette conférence avait pour but de présenter les enjeux et le fonctionnement d'une montée de version d'application sans interruption.
En effet, les montées de version interrompant le service ont un large impact sur l'application. Elles peuvent par exemple engendrer des pertes de chiffre d'affaires dûes à l'absence de services, ou encore des pertes de client dûes à une mauvaise expérience utilisateur. Enfin, le modèle de release conséquentes à des intervalles de temps relativement longs est source de problèmes, résultant en de nombreux hotfix. La montée de version sans interruption, qui se base sur de plus petites et fréquentes releases, permet donc de fiabiliser le service.

Une montée de version sans interruption se base sur un principe de rétro-compatibilité entre les versions. On peut parler de 4 versions intermédiaires de l'application avant d'obtenir la réelle version finale :

 - La version originale à partir de laquelle on souhaite travailler (Serveur v1, Base v1).
	
 - Une nouvelle version de base, qui reste compatible avec l'applicatif du serveur (Serveur v1, Base v2).
	
 - Une nouvelle version d'applicatif sur le serveur, qui prend en compte les modifications au sein de la base (Serveur v1, Serveur v2, Base v2).
	
 - Une redirection du trafic vers le serveur v2 (Serveur v2, Base v2).
	 
## Architecture et facteur qualité
