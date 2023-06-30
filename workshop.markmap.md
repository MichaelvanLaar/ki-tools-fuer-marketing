---
markmap:
  # initialExpandLevel: 1
  # maxWidth: 300
  colorFreezeLevel: 2
  color:
  - '#1B1D1C'
  - '#B2B2B2'
  - '#FBBA00'
  - '#0D3174'
---

# KI-Tools fürs<br>Marketing

## KI-Grundlagen

### Begriffe

- Künstliche Intelligenz (KI, AI)
- Machine Learning (ML)
- Künstliche neuronale Netzwerke
- Deep Learning (DL)
- Large Language Model (LLM)

### Arten von KI

- Schwache KI (weak/narrow AI)
- Starke KI (strong/general AI)

### Erstellung eines ML-Modells

- Zuerst Training
  - Pretraining
  - Finetuning
- Dann Praxiseinsatz
- Ggf. selbständiges kontinuierliches Weiterlernen

### ML-Lernmethoden<br>und -Anwendungen

- *Lernmethode:* Überwachtes Lernen<br>(🡪 labeled Data notwendig)
  - *Anwendung:* z. B. Klassifikation (🡪 diskrete Ergebnismenge)
  - *Anwendung:* z. B. Regression (🡪 stetige Ergebnismenge)
- *Lernmethode:* Unüberwachtes Lernen<br>(🡪 unlabeled Data ausreichend)
  - *Anwendung:* z. B. Clustering
  - *Anwendung:* z. B. Dimensionsreduktion
- *Lernmethode:* Bestärkendes Lernen
  - *Anwendung:* z. B. Optimieren oder Nachtrainieren von ML-Modellen

### Generative KI-Modelle

- Generative Adversarial Networks (GAN)
  - Bestandteile
    - Generator 🡪 erstellt neue Inhalte, die den Quelldaten ähneln
    - Diskriminator 🡪 bewertet die erzeugten Inhalte
  - Gegenseitiges Spiel: Generator versucht Diskriminator zu täuschen
- Transformatoren
  - Beispiele: GPT-4, LLaMA, BERT, Wu-Dao
  - Speziell für die Verarbeitung von sequenziellen Daten entwickelt, wie z.B. Text
  - Ahmen kognitive Aufmerksamkeit nach, um auf verschiedene Teile der<br>Eingabesequenz zu „achten“ und die wichtigsten Teile zu identifizieren
- Variational Autoencoder
  - Oft für Bildgenerierung eingesetzt (z. B. in Stable Diffusion)
  - Bestandteile
    - Encoder 🡪 vereinfacht komplizierte Daten<br>*(Anschaulicher Vergleich: Maler 1 erstellt eine Reihe<br>einfacher Skizzen einer Szene)*
    - Decoder 🡪 versucht, Originaldaten aus den vom<br>Encoder vereinfachten Daten zu rekonstruieren<br>*(Anschaulicher Vergleich: Maler 2 wählt eine dieser<br>Skizzen aus und versucht, daraus ein Bild zu malen,<br>das die Originalszene möglichst genau abbildet, ohne<br>jedoch die Originalszene selbst zu kennen)*
- Denoising Diffusion Models
  - Oft für Bildgenerierung eingesetzt (z. B. in Stable Diffusion)
  - Trainingsprinzip
    - *Schritt 1* Vermischung des Ausgangsbildes mit Rauschen<br>(schrittweise stärker werdend) und Protokollierung
    - *Schritt 2:* Versuch der Wiederherstellung des Ausgangsbildes<br>aus dem Rauschen anhand der Protokolle
  - Ziel des Trainings
    - Modell erhält durch die Analyse der Vereinfachungsschritte<br>(Bildrauschen) vieler unterschiedlicher Bilder desselben Motivs<br>eine „Vorstellung“ vom Motiv, unabhängig von den Parametern<br>(z. B. Perspektive, Beleuchtung usw.) eines konkreten Bildes
    - Modell lernt „Rezepte“ für die Wiederherstellung verschiedener<br>Arten von Bildern aus Rauschen
  - *Anwendung:* Erstellung völlig „neuer“ Bilder eines Motivs
    - Funktioniert als „Text to Image“ meist in Kombination<br> mit anderen ML-Techniken und unter Zuhilfenahme<br>von labeled Data im Trainingsprozess
    - Sehr anschauliche Erklärung zum Nachlesen:<br>[How Stable Diffusion Works](https://mccormickml.com/2022/12/21/how-stable-diffusion-works/)

## Anwendungsgebiete<br>und Tools

### Präsentationen

#### Anwendungsfälle

- Inhaltsideen und Inhaltsstruktur
- Erstellung von ganzen Folien (Text, Grafik, Bild)
- Optimierung von Folienlayouts

#### Tools

- [Tome](https://tome.app/)
  - 🡪 [Ausprobieren](https://tome.app/van-laar)
- [Beautiful.ai](https://www.beautiful.ai/)
  - 🡪 [Ausprobieren](https://www.beautiful.ai/library/owned_by_me)

### Audio

#### Anwendungsfälle

- Text 🡪 Sprache
- Sprache 🡪 Text
- Text 🡪 Musik
- Musik 🡪 Musik
- Audiobearbeitung<br><small>z. B. Hintergrundgeräusche entfernen, automatische Optimierung</small>

#### Tools

- [ElevenLabs](https://beta.elevenlabs.io/)
  - 🡪 [Ausprobieren](https://beta.elevenlabs.io/speech-synthesis)
##### Musikgenerierung

- [MusicGen](https://github.com/facebookresearch/audiocraft)
-  🡪 [Ausprobieren](https://huggingface.co/spaces/facebook/MusicGen)
- [AIVA](https://www.aiva.ai/)
  - 🡪 [Ausprobieren](https://creators.aiva.ai/)
- 😉 [Voicemod](https://www.voicemod.net/text-to-song/)<br><small>„Your musical meme machine“</small>

### Video

#### Anwendungsfälle

- Text-Prompt 🡪 Video
- Video 🡪 Video
- Kombination aus Video- und Bild-/Text-Prompt 🡪 Video
- Videopbearbeitung per Text-Prompt

#### Tools

##### Text Prompt 🡪 Video

- [Runway Gen-2](https://runwayml.com/ai-magic-tools/gen-2/)
  - 🡪 [Ausprobieren](https://app.runwayml.com/video-tools/teams/MichaelvanLaar/assets)
- [Zeroscope](https://huggingface.co/spaces/fffiloni/zeroscope)
  - [Beispielvideo 1](https://twitter.com/pharmapsychotic/status/1673825814906048512)
  - [Beispielvideo 2](https://twitter.com/cerspense/status/1672365482454958080)
  - [Beispielvideo 3](https://twitter.com/veryVANYA/status/1673695807147585538)
  - [Beispielvideo 4](https://twitter.com/dotsimulate/status/1673780493848805379)
  - [Beispielvideo 5](https://www.reddit.com/r/aivideo/comments/14kikmr/just_walking_through_the_ages/)
  - 🡪 [Ausprobieren](https://huggingface.co/spaces/fffiloni/zeroscope)
- [Kaiber](https://kaiber.ai/)
  - 🡪 [Ausprobieren](https://kaiber.ai/dashboard)
- [D-ID](https://www.d-id.com/)<br><small>Talking-Head-Videos mit virtuellen Avataren</small>
  - 🡪 [Ausprobieren](https://studio.d-id.com/)

##### Video 🡪 Video

- [Runway Gen-1](https://runwayml.com/ai-magic-tools/gen-1/)<br><small>Modifizierung von Referenz-Videos mithilfe eines Referenz-Bildes oder eines Text-Prompts</small>
  - 🡪 [Ausprobieren](https://app.runwayml.com/video-tools/teams/MichaelvanLaar/assets)

##### Videobearbeitung

- [Runway Video Inpainting](https://runwayml.com/inpainting/)<br><small>unerwünschte (auch bewegte!) Objekte aus Videos entfernen</small>
- Adobe Premiere Pro (Beta)<br><small>Videoschnitt per Transkript</small>

#### [Anleitung: Kurzfilm erstellen mit einer Kombination mehrerer Tools](https://www.youtube.com/watch?v=5kBxR-kliXc)

### 3D-Modelle

#### Anwendungsfälle

- Text-Prompt 🡪 3D-Modell
- Text-Prompt 🡪 Textur
- 2D-Bild 🡪 3D-Modell
- 2D-Bild 🡪 3D-Textur
- Ggf. demnächst Alternative zum klassischen finalen Rendern von (Roh-)Modellen (inkl. Texturen, Beleuchtung usw.)

#### Tools

- [Meshy](https://www.meshy.ai/)
  - 🡪 [Ausprobieren](https://discord.com/channels/1080050109062058044/1083607466719330334)

### Bilder<br>(Pixelgrafiken)

#### Anwendungsfälle

- Text-Prompt 🡪 Bild
- Bild 🡪 Bild
- Kombination aus Bild- und Text-Prompt 🡪 Bild
- Bildbearbeitung per Text-Prompt

#### Tools

### Text / Chat

#### Anwendungsfälle

#### Tools

##### Einzelne Modelle

##### Drittanbieter-Apps

- [nat.dev OpenPlayground](https://nat.dev/)

##### Kombination verschiedener Tools

- [Blobr ChatGPT plugin generator](https://www.blobr.io/api-gateway-chatgpt-plugins)<br><small>No-Code-GUI zum Erstellen eigener ChatGPT-Plugins,<br>mit denen auf jede verfügbare API zugegriffen werden kann</small>
- [LangChain](https://langchain.com/)<br><small>Zusammenbauen von eigenen Apps (z. B. Chatbots)<br>durch Kombination verschiedener APIs und Tools</small>
- [FlowiseAI](https://flowiseai.com/)<br><small>No-Code-/Low-Code-GUI zur Erstellung von LangChain-Apps</small>

## Prompt Engineering,<br>Tipps und Weiterbildung

### Prompt Engineering

- [GPT best practices](https://platform.openai.com/docs/guides/gpt-best-practices)
- [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)
- [Learn Prompting](https://learnprompting.org/docs/intro)
- [Prompt Engineering Guide](https://www.promptingguide.ai/)

### Lernplattformen

- [KI-Campus](https://ki-campus.org/)
- [DeepLearning.AI](https://www.deeplearning.ai/)

### KI-Grundlagen-Kurse

- [Einführung in die KI](https://ki-campus.org/courses/einfuehrungki2020)
- [KI für alle: Einführung in die Künstliche Intelligenz](https://ki-campus.org/courses/kifueralle-hhu)

### Wissenssammlungen

- [AI Canon](https://a16z.com/2023/05/25/ai-canon/) von Andreessen Horowitz (a16z)<br><small>*„a curated list of resources we’ve relied on to get smarter about modern AI“*</small>
- [AI glossary by a16z](https://a16z.com/ai-glossary/)

### Tool-Übersichten

- [Futurepedia](https://www.futurepedia.io/)
- [There’s An AI For That](https://theresanaiforthat.com/)
- [TailwindAI](https://www.tailwindai.com/)
