---
markmap:
  embedAssets: true
  initialExpandLevel: 1
  # maxWidth: 300
  colorFreezeLevel: 2
  color:
    - "#1B1D1C"
    - "#B2B2B2"
    - "#FBBA00"
    - "#0D3174"
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

- _Lernmethode:_ Überwachtes Lernen<br>(→ labeled Data notwendig)
  - _Anwendung:_ z. B. Klassifikation (→ diskrete Ergebnismenge)
  - _Anwendung:_ z. B. Regression (→ stetige Ergebnismenge)
- _Lernmethode:_ Unüberwachtes Lernen<br>(→ unlabeled Data ausreichend)
  - _Anwendung:_ z. B. Clustering
  - _Anwendung:_ z. B. Dimensionsreduktion
- _Lernmethode:_ Bestärkendes Lernen
  - _Anwendung:_ z. B. Optimieren oder Nachtrainieren von ML-Modellen

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
    - Encoder → vereinfacht komplizierte Daten<br>_(Anschaulicher Vergleich: Maler 1 erstellt eine Reihe<br>einfacher Skizzen einer Szene)_
    - Decoder → versucht, Originaldaten aus den vom<br>Encoder vereinfachten Daten zu rekonstruieren<br>_(Anschaulicher Vergleich: Maler 2 wählt eine dieser<br>Skizzen aus und versucht, daraus ein Bild zu malen,<br>das die Originalszene möglichst genau abbildet, ohne<br>jedoch die Originalszene selbst zu kennen)_
- Denoising Diffusion Models
  - Oft für Bildgenerierung eingesetzt (z. B. in Stable Diffusion)
  - Trainingsprinzip
    - _Schritt 1_ Vermischung des Ausgangsbildes mit Rauschen<br>(schrittweise stärker werdend) und Protokollierung
    - _Schritt 2:_ Versuch der Wiederherstellung des Ausgangsbildes<br>aus dem Rauschen anhand der Protokolle
  - Ziel des Trainings
    - Modell erhält durch die Analyse der Vereinfachungsschritte<br>(Bildrauschen) vieler unterschiedlicher Bilder desselben Motivs<br>eine „Vorstellung“ vom Motiv, unabhängig von den Parametern<br>(z. B. Perspektive, Beleuchtung usw.) eines konkreten Bildes
    - Modell lernt „Rezepte“ für die Wiederherstellung verschiedener<br>Arten von Bildern aus Rauschen
  - _Anwendung:_ Erstellung völlig „neuer“ Bilder eines Motivs
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
- [Decktopus](https://www.decktopus.com/)
- [Beautiful.ai](https://www.beautiful.ai/)

### Audio

#### Anwendungsfälle

- Text → Sprache
- Sprache → Text
- Sprache → Sprache (Übersetzung)
- Text → Musik
- Musik → Musik
- Kombination aus Referenz-Musik und Text-Prompt → Musik
- Text → Soundeffekt (z. B. für Filmproduktion)
- Audiobearbeitung<br><small>z. B. Hintergrundgeräusche entfernen, automatische Optimierungen</small>

#### Tools

##### Text → Sprache

- [ElevenLabs](https://beta.elevenlabs.io/)<br><small>inkl. Voice Cloning</small>
- [PlayHT](https://play.ht/)<br><small>inkl. Voice Cloning</small>
- [WondercraftAI](https://www.wondercraft.ai)<br><small>Komplette Podcast-Produktion aus geschriebenem Text</small>
- [BARK](https://github.com/serp-ai/bark-with-voice-clone)<br><small>inkl. Voice Cloning<br>(Open Source)</small>
- [VoiceBox](https://voicebox.metademolab.com/)<br><small>Voice Cloning auf Basis von nur wenigen Sekunden Sprachaufnahme<br>(Modell leider noch nicht veröffentlicht, aber Beispiel-Clips verfügbar)</small>
- [SoundStorm](https://google-research.github.io/seanet/soundstorm/examples/)<br><small>Voice Cloning auf Basis von nur wenigen Sekunden Sprachaufnahme<br>(Modell leider noch nicht veröffentlicht, aber Beispiel-Clips verfügbar)</small>
- 😉 [Uberduck](https://uberduck.ai/)

##### Sprache → Text

- [Happy Scribe](https://www.happyscribe.com/de)<br><small>Untertitel und Transkription für Videos</small>
- [AudioPen](https://audiopen.ai/)<br><small>Audiotranskription + automatisches „Aufräumen“ und Zusammenfassen</small>

##### Sprache → Sprache

- [CloneDub](https://www.clonedub.com/)<br><small>(funktioniert noch nicht wirklich gut)</small>
- [SoftVC VITS Singing Voice Conversion](https://github.com/svc-develop-team/so-vits-svc)<br><small>Stimmenaustausch, teilweise in Echtzeit, gern verwendet für Gesang</small>
  - [Celebrity Voice Models](https://huggingface.co/QuickWick/Music-AI-Voices/tree/main)
  - [Celebrity Voice Models](https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main)

##### Musikgenerierung

- [Splash](https://www.splashmusic.com/)
  - [BeatBot](https://beatbot.fm/)
  - [Splash Pro](https://pro.splashmusic.com/)
- [Mubert](https://mubert.com/)
- [AIVA](https://www.aiva.ai/)
- [beatoven.ai](https://www.beatoven.ai/)
- [MusicGen](https://github.com/facebookresearch/audiocraft)
  - [Ausprobieren bei Hugging Face](https://huggingface.co/spaces/facebook/MusicGen)
  - [Ausprobieren bei MusicGen-Looper](https://replicate.com/andreasjansson/musicgen-looper)
- [The Watson Beat](https://github.com/cognitive-catalyst/watson-beat)<br><small>KI-Modell erstellt aus einer einfachen Melodie und Stilanweisungen<br>eine komplette Komposition inkl. Arrangement für mehrere Instrumente</small>
  - [Audio-Beispiele](https://www.youtube.com/watch?v=Z5ymVzTUU6Y)
- [DeepComposer](https://aws.amazon.com/de/deepcomposer/)<br><small>Grundprinzip wie bei The Watson Beat, aber umgesetzt als Keyboard<br>(Hardware) mit direktem Anschluss an KI-Modelle in der AWS-Cloud</small>
  - [Demo-Video von 2019](https://www.youtube.com/watch?v=XH2EbK9dQlg&t=453s)
- [MusicLM](https://google-research.github.io/seanet/musiclm/examples/)<br><small>(Modell leider noch nicht veröffentlicht, aber Beispiel-Clips verfügbar)<br>→ „Story Mode“ sieht für Video-Soundtracks sehr vielversprechend aus</small>
- [SingSong](https://storage.googleapis.com/sing-song/index.html)<br><small><i>„Generating musical accompaniments from singing“</i><br>(Modell leider noch nicht veröffentlicht, aber Beispiel-Clips verfügbar)</small>
- [Moûsai](https://anonymous0.notion.site/anonymous0/Mo-sai-Text-to-Audio-with-Long-Context-Latent-Diffusion-b43dbc71caf94b5898f9e8de714ab5dc)<br><small><i>„Text-to-Audio with Long-Context Latent Diffusion“</i><br>(Modell leider noch nicht veröffentlicht, aber Beispiel-Clips verfügbar)</small>
- [AudioLDM](https://audioldm.github.io/)<br><small><i>„Text-to-Audio Generation with
Latent Diffusion Models“</i><br>(Modell leider noch nicht veröffentlicht, aber Beispiel-Clips verfügbar)<br>→ Interessant offenbar auch für die Generierung von Soundeffekten für Video-/Filmproduktion</small>
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
- KI-generierte Aninationen oder Animationen aus KI-generierten Bestandteilen
- Automatische Übersetzung gesprochener Texte in eine andere Sprache<br>+ Neuvertonung mit geclonter Stimme + automatische lippensynchrone Anpassung des Videos
- Videobearbeitung per Text-Prompt
- Automatisierte Videopersonalisierung

#### Beispiele dafür, was mit Text-to-<br>Video-Tools derzeit machbar ist

- [„Synthetic Summer“](https://www.privateisland.tv/home/synthetic-summer) (wahrscheinlich mit Gen-2 generiert)
- [„Cursed Heidi“](https://www.youtube.com/watch?v=0A2-Af5JEWU) (mit Gen-2 generiert)
- [Zeroscope-Beispielvideo 1](https://twitter.com/pharmapsychotic/status/1673825814906048512)
- [Zeroscope-Beispielvideo 2](https://twitter.com/cerspense/status/1672365482454958080)
- [Zeroscope-Beispielvideo 3](https://twitter.com/veryVANYA/status/1673695807147585538)
- [Zeroscope-Beispielvideo 4](https://twitter.com/dotsimulate/status/1673780493848805379)
- [Zeroscope-Beispielvideo 5](https://www.reddit.com/r/aivideo/comments/14kikmr/just_walking_through_the_ages/)
- [KI-generierte „South Park“-Folgen](https://vimeo.com/user94220217)<br><small>Echtheit bisher nicht geklärt, einiges deutet auf einen Hoax hin.</small>
  - [Research Paper zur verwendeten Technologie-Kombination](https://fablestudio.github.io/showrunner-agents/)
  - [Hintergrundrecherche](https://www.youtube.com/watch?v=Oo0HvBtXqMg)

#### Tools

##### Text Prompt → Video

- [Gen-2](https://runwayml.com/ai-magic-tools/gen-2/)
- [Zeroscope](https://huggingface.co/spaces/fffiloni/zeroscope)
- [Pika](https://www.pika.art/)
- [Kaiber](https://kaiber.ai/)
- [Teach-O-Matic](https://www.teachomatic.net/)<br><small>_„Create AI how-to videos from text instructions. It runs on Replicate, LangChain, and GPT-4.“_</small>
- [D-ID](https://www.d-id.com/)<br><small>Talking-Head-Videos mit virtuellen Avataren</small>
- [Fliki](https://fliki.ai/)<br><small>Videos aus Text-to-Speech-Audiospuren und Stock-Videoclips oder Bildern zusammenbauen</small>

##### Video → Video

- [Gen-1](https://runwayml.com/ai-magic-tools/gen-1/)<br><small>Modifizierung von Referenz-Videos mithilfe eines Referenz-Bildes oder eines Text-Prompts</small>

##### Bild → Animation

- 😉 [Animated Drawings](https://sketch.metademolab.com/)

##### Automatische Übersetzung gesprochener Texte<br>+ Neuvertonung mit geclonter Stimme<br>+ automatische lippensynchrone Anpassung des Videos

- [HeyGen](https://labs.heygen.com/video-translate)

##### Videobearbeitung

- [vidyo.ai](https://vidyo.ai/)<br><small>„Make short videos from long ones instantly“</small>
- [Runway Video Inpainting](https://runwayml.com/inpainting/)<br><small>unerwünschte (auch bewegte!) Objekte aus Videos entfernen</small>
- Adobe Premiere Pro (Beta)<br><small>Videoschnitt per Transkript</small>

##### Automatisierte<br>Videopersonalisierung

- [Maverick](https://www.trymaverick.com/)

#### [Anleitung: Kurzfilm erstellen mit<br>einer Kombination mehrerer Tools](https://www.youtube.com/watch?v=5kBxR-kliXc)

### 3D-Modelle

#### Anwendungsfälle

- Text-Prompt → 3D-Modell
- Text-Prompt → Textur
- 2D-Bild → 3D-Modell
- 2D-Bild → 3D-Textur
- Ggf. demnächst Alternative zum klassischen finalen Rendern von (Roh-)Modellen (inkl. Texturen, Beleuchtung usw.)

#### Tools

- [Meshy](https://www.meshy.ai/)

### Bilder<br>(Pixelgrafiken)

#### Anwendungsfälle

- Text-Prompt → Bild
- Bild → Bild
- Kombination aus Bild- und Text-Prompt → Bild
- Bildbearbeitung per Text-Prompt
- Experimentell: [Rekonstruktion visueller Eindrücke aus menschlicher Gehirnaktivität](https://sites.google.com/view/stablediffusion-with-brain/)

#### Tools

##### Bildgenerierung

- [Midjourney](https://www.midjourney.com/)
- [DALL·E 3](https://openai.com/dall-e-3)
- [Stable Diffusion](https://stability.ai/stablediffusion)
  - [Ausprobieren bei DreamStudio](https://beta.dreamstudio.ai/)
  - [Ausprobieren bei Clipdrop](https://clipdrop.co/tools)
  - [Nutzung (inkl. ControlNet) bei RunDiffusion](https://rundiffusion.com/)
  - [Nutzung bei Playground AI](https://playgroundai.com/)
  - [Civitai](https://civitai.com/)<br><small>Marketplatz für nachtrainierte Stable-Diffusion-Modelle</small>
- [Adobe Firefly](https://firefly.adobe.com/)
- [Adobe Photoshop Beta](https://www.adobe.com/de/products/photoshop.html)
- [Canva Text zu Bild](https://www.canva.com/apps/text-zu-bild)
- [Microsoft Designer](https://designer.microsoft.com/)
- [Zyng](https://www.zyngai.com/)<br><small>Spezialtool für Produktbild-Inszenierungen</small>
- [Subject-Diffusion](https://oppo-mente-lab.github.io/subject_diffusion/)<br><small>Bilder beliebiger Vorgabe-Objekte, -Tiere oder -Menschen anhand von nur einem einzigen Foto erzeugen</small>
- [InsightFace Face Swapping](https://insightface.ai/)<br><small>Gesichter in Fotos oder KI-generierten Bildern austauschen</small>
  - [Nutzung via Discord](https://github.com/deepinsight/insightface/tree/master/web-demos/swapping_discord)

##### Bildbearbeitung

- [Adobe Photoshop Beta](https://www.adobe.com/de/products/photoshop.html)
- [Tracejourney](https://www.tracejourney.com/)<br><small>Midjourney-Bilder (oder auch andere Bilder) direkt<br>in Discord in Vektorgrafiken umwandeln lassen</small>
  - [Nutzung via Discord](https://discord.gg/8ynJNQz3Sm)
- [Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)<br><small>KI-basiertes Bild-Upscaling bis zu 600%</small>
- [Upscale.media](https://www.upscale.media/)<small>KI-basiertes Bild-Upscaling bis zu 400%</small>
- [Pixelcut Upscaler](https://create.pixelcut.ai/upscaler)<small>KI-basiertes Bild-Upscaling bis zu 400%</small>
- [DragGAN](https://vcai.mpi-inf.mpg.de/projects/DragGAN/)
  - [Ausprobieren via Google Colab Notebook](https://colab.research.google.com/drive/1hHtcuYAn_twAoSl_i6Trr4DoH70Zg_Oo?usp=sharing)
  - [Eigenen Bilder so umwandeln, dass man sie mit DragGAN bearbeiten kann](https://colab.research.google.com/drive/1lQeo-9p9tWRAnnFAAvQes_zpGdcPJVGj?usp=sharing)
  - [Anleitungsvideo fürs Ausprobieren](https://www.youtube.com/watch?v=ud6k0AVzw4M)
- [FreeDrag](https://lin-chen.site/projects/freedrag/)<br><small>„Nachfolger“ von DragGAN, mit besseren Fähigkeiten</small>

##### Utilities

###### Prompt-Erstellung<br>und -Optimierung

- [IMI Prompt](https://www.imiprompt.com/builder)<br><small>Midjourney Prompt Builder</small>
- [promptoMANIA Prompt Builder](https://promptomania.com/prompt-builder/)<br><small>für verschiedene Bildgenerierungs-Tools</small>
- Midjourney Shorten Command
- [PromptBase](https://promptbase.com/)<br><small>Prompt Marketplace</small>

###### Stil-Referenzen

- [Midlibrary](https://www.midlibrary.io/)<br><small>_„The most advanced library of genres, artistic movements,<br>techniques, titles, and artists’ styles for Midjourney AI“_</small>
- [Beginners Guide to Photorealistic Images in Midjourney](https://www.linkedin.com/posts/rory-flynn-ai_beginners-guide-to-photorealistic-images-activity-7098715018350735361-F3W-?utm_source=share&utm_medium=member_desktop)

###### Bild → Prompt

- [CLIP Interrogator](https://huggingface.co/spaces/pharma/CLIP-Interrogator)
- [CLIP Interrogator 2.1](https://huggingface.co/spaces/fffiloni/CLIP-Interrogator-2)
- [Midjourney Describe Command](https://docs.midjourney.com/docs/describe)

### Text / Chat

#### Anwendungsfälle

- Unterstützung bei Ideenfindung und Konzeption
- Inhaltsstrukturierung
- Texterstellung
- Textüberarbeitung und -optimierung
- Übersetzung
- Zusammenfassungen
- Textanalysen (z. B. Sentimentanalysen)
- Chatbots (z. B. für Customer-Support, Wissensvermittlung)
- Programmcode-Erstellung, -Optimierung, -Debugging
- Datenanalyse<br><small>(ChatGPT kennt die entsprechenden statistischen Methoden und<br>kann selbstständig ein entsprechendes Analyse-Programm in<br>Python programmieren, Ausführen und die Ergebnisse interpretieren)</small>
- In Kombination mit anderen Tools (z. B. Websuche, Plugins, APIs):<br>User Interface für nahezu beliebige Anwendungsfälle,<br>die sich mit Sprache und/oder Text abbilden lassen
- Bei multimodalen Tools: Kombination aus der Ein- und Ausgabe von Texten, Bildern, Audiodaten und Videos möglich
- Automone Agenten zur selbständigen, mehrstufigen Lösung von komplexen Aufgaben
- …

#### Tools

##### Einzelne Modelle

- [OpenAI GPT](https://openai.com/gpt-4)
  - [Playground](https://platform.openai.com/playground)
  - [ChatGPT](https://chat.openai.com/)<br><small>in der kostenpflichtigen Version „ChatGPT Plus“ multimodal sowie mit Plugins und Programmcode-Erstellung und -Ausführung on demand in den Fähigkeiten stark erweiterbar</small>
- [Bing Chat](https://www.bing.com/search?q=Bing+AI&showconv=1&FORM=hpcodx)<br><small>GPT-4-basiert, nur mit dem Edge-Browser nutzbar.</small>
- [Claude](https://claude.ai/)<br><small>Derzeit nur in USA und UK verfügbar,<br>kann aber per VPN (z. B. mit Standort UK) verwendet werden.</small>
- [Bard](https://bard.google.com/)
- [Llama 2](https://ai.meta.com/llama/)<br><small>(Open Source)<small>
  - [Ausprobieren bei Hugging Face](https://huggingface.co/spaces/ysharma/Explore_llamav2_with_TGI)
- [OpenChatKit](https://openchatkit.net/)<br><small>(Open Source)</small>
- [Nutzung verschiedener Modelle bei Forefront](https://www.forefront.ai/)
- [Nutzung verschiedener Modelle bei nat.dev OpenPlayground](https://nat.dev/)
- [Nutzung verschiedener Open-Source-Modelle lokal und offline via GPT4ALL](https://gpt4all.io/)<br><small>Setzt je nach Modell leistungsfähige Hardware voraus, um zu funktionieren.</small>

##### Textüberarbeitung

- [DeepL Write](https://www.deepl.com/write)
- [LanguageTool](https://languagetool.org/)

##### Übersetzung

- [DeepL Translator](https://www.deepl.com/translator)
  - Trainingsdaten: [Linguee](https://www.linguee.de/)

##### KI-Texterstellungs-Features als<br>Unterstützungsfunktion in anderen Apps

- [Magic Write in Canva](https://www.canva.com/magic-write/)
- [AI Caption Writer in SmarterQueue](https://smarterqueue.com/features/ai_caption_writer?src=sidenav)

##### Beispiele für (oft überflüssige)<br>Drittanbieter-Apps

- [Rix](https://hashnode.com/rix)
- [Scrip AI](https://scripai.com/)
- [analogenie](https://analogenie.com/)
- [ELI5](https://explainlikeimfive.io/)
- [Samwell](https://www.samwell.ai/)
- [Pico](https://picoapps.xyz/)<br><small><i>„GPT4-powered text-to-app platform“</i></small>

##### Kombination verschiedener Tools

- [Blobr ChatGPT plugin generator](https://www.blobr.io/api-gateway-chatgpt-plugins)<br><small>No-Code-GUI zum Erstellen eigener ChatGPT-Plugins,<br>mit denen auf jede verfügbare API zugegriffen werden kann</small>
- [LangChain](https://langchain.com/)<br><small>Zusammenbauen von eigenen Apps (z. B. Chatbots)<br>durch Kombination verschiedener APIs und Tools</small>
- [FlowiseAI](https://flowiseai.com/)<br><small>No-Code-/Low-Code-GUI zur Erstellung von LangChain-Apps</small>
- [Floneum](https://floneum.com/)<br><small><i>„A graph editor for local AI workflows“</i></small>
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
- [PromptDrive](https://promptdrive.ai/)

###### Erkennung KI-generierter Texte

- [GPTZero](https://gptzero.me/)
- [GPT Radar](https://gptradar.com/)
- [ZeroGPT Detector](https://www.zerogptdetector.com/)

## Prompt Engineering,<br>Tipps und Weiterbildung

### Prompt Engineering

- [GPT best practices](https://platform.openai.com/docs/guides/gpt-best-practices)
- [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)
- [Learn Prompting](https://learnprompting.org/docs/intro)
- [Prompt Engineering Guide](https://www.promptingguide.ai/)
- [gpt-prompt-engineer](https://github.com/mshumer/gpt-prompt-engineer)<br><small>Halbautomatisches Promt-Engineering-Tool</small>

### Lernplattformen

- [KI-Campus](https://ki-campus.org/)
- [DeepLearning.AI](https://www.deeplearning.ai/)

### KI-Grundlagen-Kurse

- [Einführung in die KI](https://ki-campus.org/courses/einfuehrungki2020)
- [KI für alle: Einführung in die Künstliche Intelligenz](https://ki-campus.org/courses/kifueralle-hhu)

### Wissenssammlungen

- [AI Canon](https://a16z.com/2023/05/25/ai-canon/) von Andreessen Horowitz (a16z)<br><small>_„a curated list of resources we’ve relied on to get smarter about modern AI“_</small>
- [AI glossary by a16z](https://a16z.com/ai-glossary/)

### Tool-Übersichten

- [Futurepedia](https://www.futurepedia.io/)
- [There’s An AI For That](https://theresanaiforthat.com/)
- [TailwindAI](https://www.tailwindai.com/)
