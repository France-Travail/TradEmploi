# TradEmploi / TradSNCF
TradEmploi / TradSNCF est une application web qui permet à des personnes ne parlant pas les mêmes langues de communiquer. Chacun peut parler et entendre dans sa propre langue. 

L’application intègre, dans un cadre sécurisé, des APIs de langage fournis par Google Cloud, Microsoft Azure, et DeepL. 

Ce sont 3 types de services avec des natures d’IA différentes qui sont utilisées : 
- le 1er pour retranscrire la voix en texte, 
- le 2nd pour traduire le texte,
- le 3eme pour lire la traduction et tout cela en 130 langues.

L'application a été déployée chez France Travail au printemps 2022 (TradEmploi) et à la SNCF en 2024 pour l'accueil des 2 millions de voyageurs étrangers (TradSNCF).

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

L'enregistrement sonore permetant de valider la bonne comphéresion de la langue par l'usager.

Il existe des langues où la prise en charge la vocalisation dans la langue de l'usager allophone n'est pas prise en charge : "cas dégradés". Pour ces cas, l'usager ne pourra pas entendre les traductions dans sa langue et devra les lire sur l'écran. La vocalisation sera mis en oeuvre pour ces lagues lorsqu'elle sera disponible chez les fournisseurs de traductions.

<img width="770" alt="image" src="https://github.com/user-attachments/assets/8dfc4b6b-a3d9-4afc-a669-6e5acd4b0272">
  
# Converser
Une phrase d'acceuil traduit dans la langue de l'usager donne quelques consignes d'utilisation : "Voici un traducteur automatique qui va traduire votre langue. Pour améliorer l'expérience de traduction, faites des phrases courtes et simples et parlez suffisamment fort.". Ces consignes peuvent être synthétisées vocalement.
![image](https://github.com/user-attachments/assets/5a03ce01-7384-48af-9c60-eb9ad6211ca4)



# Licence
This project is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE V3.0. Please check the LICENSE file.

# Modules

- [TradEmploi: main documentation](docs/documentation.md)
- [TradEmploi-backend](https://github.com/OSS-Pole-Emploi/TradEmploi-BackEnd.git)
- [TradEmploi-frontend](https://github.com/OSS-Pole-Emploi/TradEmploi-FrontEnd.git)

# Installation

see TradEmploi-backend / TradEmploi-frontend:

1. backend: Create GCP Infrastructure with Terraform 
2. backend: Deploy backend services
3. frontend: Create the Firebase application
4. frontend: Deploy frontend application
5. frontend / backendConfigure security


```

TradEmploi: an instantaneous translation application between two people, one of whom is allophone

Copyright (C) <2022>  <Innovation Department, DSI France Travail>

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Affero General Public License for more details.
You should have received a copy of the GNU Affero General Public License along with this program.  If not, see https://www.gnu.org/licenses/.

```
