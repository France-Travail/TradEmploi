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
- Appareils recommandés : PC, tablette, téléphones.
- Navigateurs recommandés: Google Chrome.               
- Compte utilisateur : SSO France Travail, SNCF, [Inculusion Connect](https://inclusion.beta.gouv.fr/nos-services/inclusion-connect/), Firebase Auth (login/mot de passe ou certificat)

# Choisir la langue 

# 

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
