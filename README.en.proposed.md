# Proposed English README copy-edit for TradOpen: TradEmploi / TradSNCF

This file proposes a natural-English revision of `README.md`.

# TradOpen: TradEmploi / TradSNCF

TradEmploi / TradSNCF is a web application that enables people who speak different languages to communicate. Each person can speak and listen in their own language.

The application uses language APIs from Google Cloud, Microsoft Azure, and DeepL within a secure framework.

Three AI-powered services are combined:
- speech-to-text transcription
- text translation
- text-to-speech playback

Together, these services support up to 130 languages.

Data is processed anonymously and deleted after each exchange.

The application was developed and deployed at France Travail in spring 2022 (TradEmploi), and at SNCF in 2024 to assist 2 million international travellers (TradSNCF). It was made available across the entire [inclusion network](https://inclusion.gouv.fr) in 2024 and through [Pro Connect](https://www.proconnect.gouv.fr) in 2025.

![image](https://github.com/user-attachments/assets/e5e72e04-6903-4b1d-8b10-490d165aa357)

![image](https://github.com/user-attachments/assets/9573197b-b666-44be-8836-b5bf4d31dc91)

# Prerequisites for using the application
- A continuous internet connection: wired, Wi-Fi, or 4G.
- Recommended devices: PC, tablet, or smartphone (Android or iPhone).
- Recommended browser: Google Chrome.
- User account: France Travail SSO, SNCF, [Pro Connect](https://www.proconnect.gouv.fr), or Firebase Auth (login/password or certificate).

# Choosing the language
The first screen allows the user to choose a language. The choice is based on:
- the language name, written in French and in the target language
- the name of the country where the language is most commonly spoken, written in French and in the target language
- the corresponding national flag

A voice sample is then used to confirm that the correct language has been selected.

Speech output is not available for all languages. When speech output is unavailable, users can still read the translation on screen. Voice support will be added for these languages when it becomes available from the providers.

<img width="770" alt="image" src="https://github.com/user-attachments/assets/70d19898-2a43-43a3-b9a0-59a8b3c63f87">

# Conversing
After selecting a language, the user reaches the conversation page. A welcome message, translated into the user's language, provides the following guidance: "This is an automatic translator. For better results, use short, simple sentences and speak clearly." This guidance can also be played aloud in the user's language.

![image](https://github.com/user-attachments/assets/0349edd0-3b60-47fb-8370-eb456471ded2)

Important recommendations during conversations with non-native speakers:
- Speak clearly and stay close to the microphone.
- Use short sentences.
- Avoid acronyms. For example, instead of saying RIB, say "Relevé d’Identité Bancaire", as RIB may be mistranslated.
- After speaking, check the sentence transcribed by TradEmploi before sending it:
  - unclear speech or wording can change the meaning
  - you can edit or reformulate the sentence before sending it
- Use hand signals to indicate whose turn it is to speak before clicking the microphone.
- In public reception areas, avoid using a tablet in noisy or crowded surroundings, as background speech may interfere with the conversation.

# Evaluating the experience
At the end of the conversation, you can help improve the tool by submitting a quick and anonymous evaluation.
<img width="955" alt="image" src="https://github.com/user-attachments/assets/4719185a-dc6b-4d5a-b78b-52289ec26c01">

# Demonstration
Teaser video:

https://github.com/user-attachments/assets/ea8b524d-fc30-4b96-a896-92e98588ee74

Motion design video:

[![Watch the video](https://img.youtube.com/vi/aRF_eJWPfeY/default.jpg)](https://www.youtube.com/embed/aRF_eJWPfeY)

Media coverage:
- [BFMTV video](https://www.bfmtv.com/paris/replay-emissions/bonjour-paris/sncf-une-appli-de-traduction-en-130-langues_VN-202404190143.html)
- [RTL Podcast](https://www.rtl.fr/actu/debats-societe/tradsncf-comment-fonctionne-l-appli-qui-devra-aider-les-touristes-etrangers-7900375831)

# Usage monitoring
Metabase statistics: https://metabase.beta.francetravail.fr/public/dashboard/8b4c4f48-e575-4140-b38d-1c268c5a4de3

# License
This project is distributed under the GNU Affero General Public License V3.0. Please read the LICENSE file.

# Modules and technical documentation
- Main technical documentation for the project: [TradEmploi documentation](docs/documentation.md)
- Source code and technical documentation for the [TradEmploi-backend](https://github.com/France-Travail/TradEmploi-BackEnd)
- Source code and technical documentation for the [TradEmploi-frontend](https://github.com/France-Travail/TradEmploi-FrontEnd)
