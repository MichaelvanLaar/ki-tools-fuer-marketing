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

- Generative Adversarial Netzworks (GAN)
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
- [Beautiful.ai](https://www.beautiful.ai/)

### Audio

#### Anwendungsfälle

#### Tools

### Video

#### Anwendungsfälle

#### Tools

##### Musikgenerierung

- 😉 [Voicemod](https://www.voicemod.net/text-to-song/)<br><small>„Your musical meme machine“</small>
### Bilder

#### 3D-Modelle

###### Anwendungsfälle

- Text Prompt 🡪 3D Model
- Text Prompt 🡪 Texture
- 2D Image 🡪 3D Model
- 2D Image 🡪 3D Texture

###### Tools

- [Meshy](https://www.meshy.ai/)

#### Pixelgrafiken

###### Anwendungsfälle

- Text Prompt 🡪 Image
- Image 🡪 Image
- Kombination aus Bild- und Text-Prompt
- Bildbearbeitung per Text-Prompt

###### Tools

#### Vektorgrafiken

### Text / Chat

## Prompt Engineering,<br>Tipps und Weiterbildung

### Prompt Engineering

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

- [AI Canon](https://a16z.com/2023/05/25/ai-canon/) von Andreessen Horowitz (a16z)<br><small>(*„a curated list of resources we’ve relied on to get smarter about modern AI“*)</small>
- [AI glossary by a16z](https://a16z.com/ai-glossary/)
### Tool-Übersichten

- [Futurepedia](https://www.futurepedia.io/)
- [There’s An AI For That](https://theresanaiforthat.com/)
- [TailwindAI](https://www.tailwindai.com/)