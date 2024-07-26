# TradEmploi / TradSNCF
TradEmploi / TradSNCF est une application web qui permet à des personnes ne parlants pas les mêmes langues de communiquer. Chacun peut parler et entendre dans sa propre langue. 

L’application intègre, dans un cadre sécurisé, des APIs de langage fournis par Google Cloud, Microsoft Azure, et DeepL. 

Ce sont 3 types de services avec des natures d’IA différentes qui sont utilisées : 
- le 1er pour retranscrire la voix en texte, 
- le 2nd pour traduire le texte,
- le 3eme pour lire la traduction et tout cela en 130 langues.

Les données sont traitées de manière anonyme et sont supprimées à la fin des échanges.

L'application a été développée et déployée chez France Travail au printemps 2022 (TradEmploi), à la SNCF en 2024 pour l'accueil des 2 millions de voyageurs étrangers (TradSNCF) et rendu accessible à l'ensemble du [réseau de l'inclusion](https://inclusion.beta.gouv.fr/nos-services/inclusion-connect/) courant 2024.

![image](https://github.com/akourlaiev/TradEmploi/assets/20724274/e0719c08-607d-459b-8885-fdd6560d00de)

![image](https://github.com/user-attachments/assets/07e6680b-1af0-4dab-9af6-4d111e5cec2f)

# Prérequis à l'utilisation de l'application
- Internet : connexion permanente à internet filaire, WIFI ou 4G.
- Appareils recommandés : PC, tablette, téléphones (android et iPhone).
- Navigateurs recommandés: Google Chrome.               
- Compte utilisateur : SSO France Travail, SNCF, [Inclusion Connect](https://inclusion.beta.gouv.fr/nos-services/inclusion-connect/), Firebase Auth (login/mot de passe ou certificat).

# Choisir la langue 
L'agent présente l'écran à l'usager pour le choix de la langue. Le choix est fait en se basant sur : 
- le nom de la langue (écrit en français et dans la langue en question)
- le nom du pays où la langue en question est la plus répondu (écrit en français et dans la langue en question)
- le drapeau correspodant au pays

L'enregistrement sonore permet de valider la bonne comphéresion de la langue par l'usager.

Il existe des langues où la vocalisation n'est pas prise en charge. Pour ces cas, l'usager ne pourra pas entendre les traductions dans sa langue et devra les lire sur l'écran. La vocalisation sera mis en oeuvre pour ces lagues lorsqu'elle sera disponible chez les fournisseurs de traductions.

<img width="770" alt="image" src="https://github.com/user-attachments/assets/8dfc4b6b-a3d9-4afc-a669-6e5acd4b0272">
  
# Converser
Après avoir choisi une langue, vous arrivez sur la page support à l'entretien. Une phrase d'acceuil traduit dans la langue de l'usager donne quelques consignes d'utilisation : "Voici un traducteur automatique qui va traduire votre langue. Pour améliorer l'expérience de traduction, faites des phrases courtes et simples et parlez suffisamment fort.". Ces consignes peuvent être synthétisées vocalement dans la langue de l'usager.

![image](https://github.com/user-attachments/assets/0349edd0-3b60-47fb-8370-eb456471ded2)

Recommandations importantes lors des entretiens avec un usager allophone :
- Parlez distinctement, suffisamment proche du micro
- Faites des phrases courtes
- Evitez les acronymes. Exemple : à la place de RIB, dites Relevé d’Identité Bancaire, RIB est parfois traduit avec un contresens
- Après avoir parlé, vérifiez la phrase écrite par TradEmploi avant de cliquer sur envoi
    - Une mauvaise articulation, formulation peuvent changer le sens de la phrase
    - Vous pouvez reformuler ou modifier au clavier avant envoi
- Utilisez des signes de la main pour faire comprendre à l’usager que c’est à lui ou à vous de parler avant de cliquer sur le micro.
- En zone d’accueil public, évitez les échanges sur tablette avec du monde autour pour ne pas générer de perturbations (bruit, phrases d’une personne voisine)

# Evaluer l'expérience
A la fin de l'entretien, vous avez la possiblité de contribuer à l'amélioration de l'outil en effectuant une rapide évaluation de manière anonyme.
<img width="955" alt="image" src="https://github.com/user-attachments/assets/022b0a81-12f2-4ad4-8d19-4247cba31670">

# Démonstration
Vidéo teasing:

https://github.com/user-attachments/assets/ea8b524d-fc30-4b96-a896-92e98588ee74

Vidéo en motion design:

[![Watch the video](https://img.youtube.com/vi/aRF_eJWPfeY/default.jpg)](https://www.youtube.com/embed/aRF_eJWPfeY)

Tests par les médias : 
- [Vidéo BFMTV](https://www.bfmtv.com/paris/replay-emissions/bonjour-paris/sncf-une-appli-de-traduction-en-130-langues_VN-202404190143.html)
- [Podcast RTL](https://www.rtl.fr/actu/debats-societe/tradsncf-comment-fonctionne-l-appli-qui-devra-aider-les-touristes-etrangers-7900375831) 

# Suivi usage
Connexions via bouton Inclusion Connect : https://stats.inclusion.beta.gouv.fr/public/dashboard/e9f7b6f2-e3af-45e9-84ef-0e91c2ba4c8c

# Licence
Ce projet est distribué sous la licence GNU AFFERO GENERAL PUBLIC LICENSE V3.0. Merci lire le fichier LICENSE.

# Modules et documentation technique
- Documenation technique globale du projet : [TradEmploi: main documentation](docs/documentation.md)
- Code source et documentation technique du module [TradEmploi-backend](https://github.com/OSS-Pole-Emploi/TradEmploi-BackEnd.git)
- Code source et documentation technique du module [TradEmploi-frontend](https://github.com/OSS-Pole-Emploi/TradEmploi-FrontEnd.git)
