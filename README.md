---
markmap:
  initialExpandLevel: 1
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

- *Lernmethode:* Überwachtes Lernen<br>(→ labeled Data notwendig)
  - *Anwendung:* z. B. Klassifikation (→ diskrete Ergebnismenge)
  - *Anwendung:* z. B. Regression (→ stetige Ergebnismenge)
- *Lernmethode:* Unüberwachtes Lernen<br>(→ unlabeled Data ausreichend)
  - *Anwendung:* z. B. Clustering
  - *Anwendung:* z. B. Dimensionsreduktion
- *Lernmethode:* Bestärkendes Lernen
  - *Anwendung:* z. B. Optimieren oder Nachtrainieren von ML-Modellen

### Generative KI-Modelle

- Generative Adversarial Networks (GAN)
  - Bestandteile
    - Generator → erstellt neue Inhalte, die den Quelldaten ähneln
    - Diskriminator → bewertet die erzeugten Inhalte
  - Gegenseitiges Spiel: Generator versucht Diskriminator zu täuschen
- Transformatoren
  - Beispiele: GPT-4, LLaMA, BERT, Wu-Dao
  - Speziell für die Verarbeitung von sequenziellen Daten entwickelt, wie z.B. Text
  - Ahmen kognitive Aufmerksamkeit nach, um auf verschiedene Teile der<br>Eingabesequenz zu „achten“ und die wichtigsten Teile zu identifizieren
- Variational Autoencoder
  - Oft für Bildgenerierung eingesetzt (z. B. in Stable Diffusion)
  - Bestandteile
    - Encoder → vereinfacht komplizierte Daten<br>*(Anschaulicher Vergleich: Maler 1 erstellt eine Reihe<br>einfacher Skizzen einer Szene)*
    - Decoder → versucht, Originaldaten aus den vom<br>Encoder vereinfachten Daten zu rekonstruieren<br>*(Anschaulicher Vergleich: Maler 2 wählt eine dieser<br>Skizzen aus und versucht, daraus ein Bild zu malen,<br>das die Originalszene möglichst genau abbildet, ohne<br>jedoch die Originalszene selbst zu kennen)*
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
  - → [Ausprobieren](https://tome.app/van-laar)
- [Decktopus](https://www.decktopus.com/)
  - → [Ausprobieren](https://app.decktopus.com/dashboard/decks)
- [Beautiful.ai](https://www.beautiful.ai/)
  - → [Ausprobieren](https://www.beautiful.ai/library/owned_by_me)

### Audio

#### Anwendungsfälle

- Text → Sprache
- Sprache → Text
- Sprache → Sprache (Übersetzung)
- Text → Musik
- Musik → Musik
- Kombination aus Referenz-Musik und Text-Prompt → Musik
- Audiobearbeitung<br><small>z. B. Hintergrundgeräusche entfernen, automatische Optimierungen</small>

#### Tools

##### Text → Sprache

- [ElevenLabs](https://beta.elevenlabs.io/)<br><small>inkl. Voice Cloning</small>
  - → [Ausprobieren](https://beta.elevenlabs.io/speech-synthesis)
- [PlayHT](https://play.ht/)<br><small>inkl. Voice Cloning</small>
  - → [Ausprobieren](https://play.ht/studio/)
- [WondercraftAI](https://www.wondercraft.ai)<br><small>Komplette Podcast-Produktion aus geschriebenem Text</small>
  - → [Ausprobieren](https://app.wondercraft.ai/podcasts/create)

##### Sprache → Text

- [Happy Scribe](https://www.happyscribe.com/de)<br><small>Untertitel und Transkription für Videos</small>
  - → [Ausprobieren](https://www.happyscribe.com/v2/2846538/folders/2778948)
- [AudioPen](https://audiopen.ai/)<br><small>Audiotranskription + automatisches „Aufräumen“ und Zusammenfassen</small>

##### Sprache → Sprache

- [CloneDub](https://www.clonedub.com/)<br><small>(funktioniert noch nicht wirklich gut)</small>
- [SoftVC VITS Singing Voice Conversion](https://github.com/svc-develop-team/so-vits-svc)<br><small>Stimmenaustausch, teilweise in Echtzeit, gern verwendet für Gesang</small>
  - [Celebrity Voice Models](https://huggingface.co/QuickWick/Music-AI-Voices/tree/main)
  - [Celebrity Voice Models](https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main)


##### Musikgenerierung

- [Mubert](https://mubert.com/)
  - → [Ausprobieren](https://mubert.com/render)
- [AIVA](https://www.aiva.ai/)
  - → [Ausprobieren](https://creators.aiva.ai/)
- [beatoven.ai](https://www.beatoven.ai/)
  - → [Ausprobieren](https://sync.beatoven.ai/workspace)
- [MusicGen](https://github.com/facebookresearch/audiocraft)
  - → [Ausprobieren bei Hugging Face](https://huggingface.co/spaces/facebook/MusicGen)
  - → [Ausprobieren bei MusicGen-Looper](https://replicate.com/andreasjansson/musicgen-looper)
- [The Watson Beat](https://github.com/cognitive-catalyst/watson-beat)<br><small>KI-Modell erstellt aus einer einfachen Melodie und Stilanweisungen<br>eine komplette Komposition inkl. Arrangement für mehrere Instrumente</small>
  - [Audio-Beispiele](https://www.youtube.com/watch?v=Z5ymVzTUU6Y)
- [DeepComposer](https://aws.amazon.com/de/deepcomposer/)<br><small>Grundprinzip wie bei The Watson Beat, aber umgesetzt als Keyboard<br>(Hardware) mit direktem Anschluss an KI-Modelle in der AWS-Cloud</small>
  - [Demo-Video von 2019](https://www.youtube.com/watch?v=XH2EbK9dQlg&t=453s)
- [MusicLM](https://google-research.github.io/seanet/musiclm/examples/)<br><small>(Modell leider noch nicht veröffentlicht, aber Beispiel-Clips verfügbar)<br>→ „Story Mode“ sieht für Video-Soundtracks sehr vielversprechend aus</small>
- [Synthesizer V](https://dreamtonics.com/synthesizerv/)<br><small>Generierung von künstlichen Gesangsstimmen, die echte Texte singen</small>
- 😉 [Image to Music](https://huggingface.co/spaces/fffiloni/img-to-music)
- 😉 [Voicemod](https://www.voicemod.net/text-to-song/)<br><small>„Your musical meme machine“</small>

##### Audiobearbeitung

- [DeRoom](https://www.accentize.com/deroom/)<br><small>(kommt in fast allen sepp.med-Videos im Einsatz)</small>
- [DialogueEnhance](https://www.accentize.com/dialogueenhance/)<br><small>(kommt in fast allen sepp.med-Videos im Einsatz)</small>
- [TuneFlow](https://tuneflow.com/)<br><small>kostenlose DAW mit einer Reihe eingebauter KI-Funktionen</small>

### Video

#### Anwendungsfälle

- Text-Prompt → Video
- Video → Video
- Kombination aus Referenz-Video und Bild-/Text-Prompt → Video
- Videopbearbeitung per Text-Prompt
- Automatisierte Videopersonalisierung

#### Beispiele dafür,<br>was derzeit machbar ist

- [„Synthetic Summer“](https://www.privateisland.tv/home/synthetic-summer) (wahrscheinlich mit Gen-2 generiert)
- [Zeroscope-Beispielvideo 1](https://twitter.com/pharmapsychotic/status/1673825814906048512)
- [Zeroscope-Beispielvideo 2](https://twitter.com/cerspense/status/1672365482454958080)
- [Zeroscope-Beispielvideo 3](https://twitter.com/veryVANYA/status/1673695807147585538)
- [Zeroscope-Beispielvideo 4](https://twitter.com/dotsimulate/status/1673780493848805379)
- [Zeroscope-Beispielvideo 5](https://www.reddit.com/r/aivideo/comments/14kikmr/just_walking_through_the_ages/)

#### Tools

##### Text Prompt → Video

- [Gen-2](https://runwayml.com/ai-magic-tools/gen-2/)
  - → [Ausprobieren](https://app.runwayml.com/video-tools/teams/MichaelvanLaar/assets)
- [Zeroscope](https://huggingface.co/spaces/fffiloni/zeroscope)
  - → [Ausprobieren](https://huggingface.co/spaces/fffiloni/zeroscope)
- [Kaiber](https://kaiber.ai/)
  - → [Ausprobieren](https://kaiber.ai/dashboard)
- [Teach-O-Matic](https://www.teachomatic.net/)<br><small>*„Create AI how-to videos from text instructions. It runs on Replicate, LangChain, and GPT-4.“*</small>
- [D-ID](https://www.d-id.com/)<br><small>Talking-Head-Videos mit virtuellen Avataren</small>
  - → [Ausprobieren](https://studio.d-id.com/)
- [Fliki](https://fliki.ai/)<br><small>Videos aus Text-to-Speech-Audiospuren und Stock-Videoclips oder Bildern zusammenbauen</small>
  - [Ausprobieren](https://app.fliki.ai/files)

##### Video → Video

- [Gen-1](https://runwayml.com/ai-magic-tools/gen-1/)<br><small>Modifizierung von Referenz-Videos mithilfe eines Referenz-Bildes oder eines Text-Prompts</small>
  - → [Ausprobieren](https://app.runwayml.com/video-tools/teams/MichaelvanLaar/assets)

##### Video → Animation

- 😉 [Animated Drawings](https://sketch.metademolab.com/)
  - → [Ausprobieren](https://sketch.metademolab.com/canvas)

##### Videobearbeitung

- [vidyo.ai](https://vidyo.ai/)<br><small>„Make short videos from long ones instantly“</small>
  - [Ausprobieren](https://app.vidyo.ai/home)
- [Runway Video Inpainting](https://runwayml.com/inpainting/)<br><small>unerwünschte (auch bewegte!) Objekte aus Videos entfernen</small>
- Adobe Premiere Pro (Beta)<br><small>Videoschnitt per Transkript</small>

##### Automatisierte Videopersonalisierung

- [Maverick](https://www.trymaverick.com/)

#### [Anleitung: Kurzfilm erstellen mit einer Kombination mehrerer Tools](https://www.youtube.com/watch?v=5kBxR-kliXc)

### 3D-Modelle

#### Anwendungsfälle

- Text-Prompt → 3D-Modell
- Text-Prompt → Textur
- 2D-Bild → 3D-Modell
- 2D-Bild → 3D-Textur
- Ggf. demnächst Alternative zum klassischen finalen Rendern von (Roh-)Modellen (inkl. Texturen, Beleuchtung usw.)

#### Tools

- [Meshy](https://www.meshy.ai/)
  - → [Ausprobieren](https://discord.com/channels/1080050109062058044/1083607466719330334)

### Bilder<br>(Pixelgrafiken)

#### Anwendungsfälle

- Text-Prompt → Bild
- Bild → Bild
- Kombination aus Bild- und Text-Prompt → Bild
- Bildbearbeitung per Text-Prompt

#### Tools

##### Bildgenerierung

- [Midjourney](https://www.midjourney.com/)
  - → [Ausprobieren](https://discord.com/channels/@me/1054540775469355008)
  - [Dokumentation](https://docs.midjourney.com/)
- [Stable Diffusion](https://stability.ai/stablediffusion)
  - → [Ausprobieren bei DreamStudio](https://beta.dreamstudio.ai/)
  - → [Ausprobieren (inkl. ControlNet) bei RunDiffusion](https://app.rundiffusion.com/)
  - → [Ausprobieren bei Playground AI](https://playgroundai.com/)
  - [Civitai](https://civitai.com/)<br><small>Marketplatz für nachtrainierte Stable-Diffusion-Modelle</small>
- [DALL·E](https://openai.com/dall-e-2)
  - → [Ausprobieren](https://labs.openai.com/)
- [Adobe Firefly](https://firefly.adobe.com/)
- [Adobe Photoshop Beta](https://www.adobe.com/de/products/photoshop.html)
- [Canva Text zu Bild](https://www.canva.com/apps/text-zu-bild)
- [Microsoft Designer](https://designer.microsoft.com/)
- [Zyng](https://www.zyngai.com/)<br><small>Spezialtool für Produktbild-Inszenierungen</small>
  - → [Ausprobieren](https://app.zyngai.com/)
- [InsightFace face swapping](https://insightface.ai/)<br><small>Gesichter in Fotos oder KI-generierten Bildern austauschen</small>
  - → [Ausprobieren](https://discord.com/channels/1125538374145552414/1125539703324684418)

##### Utilities

###### Prompt-Erstellung und -Optimierung

- [IMI Prompt](https://www.imiprompt.com/builder)<br><small>Midjourney Prompt Builder</small>
- [promptoMANIA Prompt Builder](https://promptomania.com/prompt-builder/)<br><small>für verschiedene Bildgenerierungs-Tools</small>
- Midjourney Shorten Command
- [PromptBase](https://promptbase.com/)<br><small>Prompt Marketplace</small>

###### Stil-Referenzen

- [Midlibrary](https://www.midlibrary.io/)<br><small>*„The most advanced library of genres, artistic movements,<br>techniques, titles, and artists’ styles for Midjourney AI“*</small>

###### Bild → Prompt

- [CLIP Interrogator](https://huggingface.co/spaces/pharma/CLIP-Interrogator)
- [CLIP Interrogator 2.1](https://huggingface.co/spaces/fffiloni/CLIP-Interrogator-2)
- [Midjourney Describe Command](https://docs.midjourney.com/docs/describe)

### Text / Chat

#### Anwendungsfälle

- Texterstellung
- Textüberarbeitung und -optimierung
- Übersetzung
- Zusammenfassungen
- Textanalysen (z. B. Sentimentanalysen)
- Chatbots (z. B. für Customer-Support, Wissensvermittlung, )
- Programmcode-Erstellung, -Optimierung, -Debugging
- In Kombination mit anderen Tools (z. B. Websuche, Plugins, APIs):<br>User Interface für nahezu beliebige Anwendungsfälle,<br>die sich mit Sprache und/oder Text abbilden lassen
- Automone Agenten zur selbständigen, mehrstufigen Lösung von komplexen Aufgaben
- …

#### Tools

##### Einzelne Modelle

- [OpenAI GPT](https://openai.com/gpt-4)
  - [Playground](https://platform.openai.com/playground)
  - [ChatGPT](https://chat.openai.com/)
- [Bard](https://bard.google.com/)<br><small>Wird von Google in Europa wegen der DSGVO nicht angeboten,<br>kann aber per VPN (z. B. mit Standort UK) verwendet werden.</small>
- [Bing Chat](https://www.bing.com/search?q=Bing+AI&showconv=1&FORM=hpcodx)<br><small>GPT-4-basiert, nur mit dem Edge-Browser nutzbar.</small>
- [OpenChatKit](https://huggingface.co/spaces/togethercomputer/OpenChatKit)
- [Nutzung verschiedener Modelle bei Forefront](https://www.forefront.ai/)
- [Nutzung verschiedener Modelle bei nat.dev OpenPlayground](https://nat.dev/)

##### Textüberarbeitung

- [DeepL Write](https://www.deepl.com/write)
- [LanguageTool](https://languagetool.org/)

##### Übersetzung

- [DeepL Translator](https://www.deepl.com/translator)
  - Trainingsdaten: [Linguee](https://www.linguee.de/)

##### Beispiele für (oft überflüssige)<br>Drittanbieter-Apps

- [Rix](https://hashnode.com/rix)
- [Scrip AI](https://scripai.com/)
- [analogenie](https://analogenie.com/)
- [ELI5](https://explainlikeimfive.io/)
- [Samwell](https://www.samwell.ai/)

##### Kombination verschiedener Tools

- [Blobr ChatGPT plugin generator](https://www.blobr.io/api-gateway-chatgpt-plugins)<br><small>No-Code-GUI zum Erstellen eigener ChatGPT-Plugins,<br>mit denen auf jede verfügbare API zugegriffen werden kann</small>
- [LangChain](https://langchain.com/)<br><small>Zusammenbauen von eigenen Apps (z. B. Chatbots)<br>durch Kombination verschiedener APIs und Tools</small>
- [FlowiseAI](https://flowiseai.com/)<br><small>No-Code-/Low-Code-GUI zur Erstellung von LangChain-Apps</small>
- [embedchain](https://github.com/embedchain/embedchain)<br><small>Für Entwickler: LangChain-basiertes Python-Framework zum Erstellen von Chatbots<br>auf GPT-Basis (via OpenAI-API), die sich nur auf selbst bereitgestellte Inhalte beziehen</small>
- [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT)
- [CustomGPT](https://customgpt.ai/)<br><small>Chatbots auf GPT-Basis (via OpenAI-API), die sich nur auf selbst bereitgestellte Inhalte beziehen<br>(Einbindung auf der sepp.med-Website aufgrund der DSGVO schwierig)</small>
- [Chatbase](https://www.chatbase.co/)<br><small>Chatbots auf GPT-Basis (via OpenAI-API), die sich nur auf selbst bereitgestellte Inhalte beziehen<br>(Einbindung auf der sepp.med-Website aufgrund der DSGVO schwierig)</small>
- [OpenChat](https://openchat.so/)<br><small>Chatbots auf GPT-Basis (via OpenAI-API), die sich nur auf selbst bereitgestellte Inhalte beziehen<br>und auf Wunsch lokal gehostet werden können (weil Open-Source-Projekt)<br>(Einbindung auf der sepp.med-Website trotz DSGVO ggf. möglich)</small>

##### Utilities

###### Prompt-Erstellung, -optimierung<br>und -speicherung

- [Prompt Vibes](https://www.promptvibes.com/)
- [Awesome ChatGPT Prompts](https://prompts.chat/)
- [Prompt Perfect](https://promptperfect.jina.ai/)
  - → [Ausprobieren](https://promptperfect.jina.ai/home)
- [PromptDrive](https://promptdrive.ai/)

###### Erkennung KI-generierter Texte

- [GPTZero](https://gptzero.me/)
- [GPT Radar](https://gptradar.com/)
- [ZeroGPT Detector](https://www.zerogptdetector.com/)
- [AI Text Classifier](https://platform.openai.com/ai-text-classifier)

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
