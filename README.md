# TradEmploi / TradSNCF
TradEmploi / TradSNCF is a web application that allows people who do not speak the same languages to communicate. Everyone can speak and hear in their own language.

The application integrates, in a secure framework, language APIs provided by Google Cloud, Microsoft Azure, and DeepL.

Three types of services with different AI systems are used:
- The first one transcribes voice into text,
- The second translates the text,
- The third reads the translation aloud, all in 130 languages.

The data is processed anonymously and deleted after the exchanges.

The application was developed and deployed at France Travail in spring 2022 (TradEmploi), and at SNCF in 2024 to assist the 2 million foreign travelers (TradSNCF). It became available to the entire [inclusion network](https://inclusion.beta.gouv.fr/nos-services/inclusion-connect/) in 2024.

![image](https://github.com/user-attachments/assets/e5e72e04-6903-4b1d-8b10-490d165aa357)

![image](https://github.com/user-attachments/assets/9573197b-b666-44be-8836-b5bf4d31dc91)

# Prerequisites for using the application
- Internet: continuous connection via wired, WiFi, or 4G.
- Recommended devices: PC, tablet, smartphones (Android and iPhone).
- Recommended browsers: Google Chrome.
- User account: SSO France Travail, SNCF, [Inclusion Connect](https://inclusion.beta.gouv.fr/nos-services/inclusion-connect/), Firebase Auth (login/password or certificate).

# Choosing the language
The agent presents the screen to the user to choose a language. The choice is made based on:
- The language name (written in French and the target language),
- The name of the country where the language is most commonly spoken (written in French and the target language),
- The corresponding flag of the country.

A voice recording is used to confirm the user's correct language comprehension.

There are languages where voice output is not supported. In these cases, the user will not be able to hear the translations in their language and will need to read them on the screen. Voice support will be implemented for these languages when available from the translation providers.

<img width="770" alt="image" src="https://github.com/user-attachments/assets/70d19898-2a43-43a3-b9a0-59a8b3c63f87">

# Conversing
After choosing a language, you arrive on the conversation support page. A greeting message translated into the user's language provides instructions: "This is an automatic translator that will translate your language. For a better translation experience, use short and simple sentences and speak clearly." These instructions can be voiced in the user's language.

![image](https://github.com/user-attachments/assets/0349edd0-3b60-47fb-8370-eb456471ded2)

Important recommendations during conversations with non-native speakers:
- Speak clearly and close to the microphone,
- Use short sentences,
- Avoid acronyms. For example, instead of saying RIB, say "Relevé d’Identité Bancaire" as RIB may be mistranslated,
- After speaking, check the sentence written by TradEmploi before sending it:
    - Poor articulation or formulation can change the meaning of the sentence,
    - You can reformulate or modify it on the keyboard before sending it,
- Use hand signals to indicate whose turn it is to speak before clicking on the microphone.
- In public reception areas, avoid tablet conversations with crowds around to prevent disruptions (noise, sentences from nearby people).

# Evaluating the experience
At the end of the conversation, you can contribute to improving the tool by providing a quick and anonymous evaluation.
<img width="955" alt="image" src="https://github.com/user-attachments/assets/4719185a-dc6b-4d5a-b78b-52289ec26c01">


# Demonstration
Teaser video:

https://github.com/user-attachments/assets/ea8b524d-fc30-4b96-a896-92e98588ee74

Motion design video:

[![Watch the video](https://img.youtube.com/vi/aRF_eJWPfeY/default.jpg)](https://www.youtube.com/embed/aRF_eJWPfeY)

Media tests:
- [BFMTV video](https://www.bfmtv.com/paris/replay-emissions/bonjour-paris/sncf-une-appli-de-traduction-en-130-langues_VN-202404190143.html)
- [RTL Podcast](https://www.rtl.fr/actu/debats-societe/tradsncf-comment-fonctionne-l-appli-qui-devra-aider-les-touristes-etrangers-7900375831)

# Usage monitoring
Connections via Inclusion Connect button: https://stats.inclusion.beta.gouv.fr/public/dashboard/e9f7b6f2-e3af-45e9-84ef-0e91c2ba4c8c

# License
This project is distributed under the GNU Affero General Public License V3.0. Please read the LICENSE file.

# Modules and technical documentation
- Global technical documentation for the project, this page, [TradEmploi: main documentation](docs/documentation.md)
- Source code and technical documentation for the [TradEmploi-backend](https://github.com/OSS-Pole-Emploi/TradEmploi-BackEnd.git)
- Source code and technical documentation for the [TradEmploi-frontend](https://github.com/OSS-Pole-Emploi/TradEmploi-FrontEnd.git)
