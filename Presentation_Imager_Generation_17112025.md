 <!--
author:   Prof. Dr. Hannes Hesse
email:    hannes.hesse@ovgu.de
version:  1.0.0
language: de
narrator: Deutsch Female

comment:  KI-Bildgenerierung in Forschung und Lehre - Praktische Anwendung und kritische Reflexion

icon: https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/ChatGPT_logo.svg/1024px-ChatGPT_logo.svg.png

-->

# KI-Bildgenerierung in Forschung und Lehre

**Übung: KI in der Forschung und Lehre**

Hannes Tegelbeckers 
Otto-von-Guericke-Universität Magdeburg

---

## Lernziele

Nach dieser Einheit können Sie:

- Unterschiede zwischen Text- und Bildprompts verstehen und anwenden
- Einen systematischen Workflow für Bildgenerierung entwickeln
- Kostenlose und proprietäre KI-Tools für Bildung einsetzen
- Typische Schwächen von Bildgeneratoren erkennen
- Kritisch über Realität vs. digitale Realität reflektieren

---

## 1. Prompting für Bildgenerierung

### Grundlegende Unterschiede zu Text-LLMs

**Text-LLMs (ChatGPT, Claude)**

- Sequenziell und konversationell
- Kontextverständnis über mehrere Nachrichten
- Iterative Verfeinerung durch Dialog

**Bild-KIs (DALL-E, Midjourney, Stable Diffusion)**

- Meist single-shot Generation
- Keine Dialogfähigkeit (mit Ausnahmen)
- Parametrische Steuerung wichtiger als Dialog

---

### Positive Prompts

**Funktion:** Beschreiben, WAS im Bild erscheinen soll

**Struktur-Empfehlung:**

```
[Hauptobjekt] + [Aktion/Zustand] + [Setting/Kontext] + 
[Stil] + [Technische Parameter]
```

**Beispiel:**

```
Ein Lehrer erklärt Schülern KI-Konzepte an einem 
interaktiven Whiteboard, modernes Klassenzimmer mit 
Tageslicht, fotorealistischer Stil, warm und einladend, 
16:9 Format, hochauflösend
```

---

### Negative Prompts

**Funktion:** Beschreiben, WAS NICHT im Bild erscheinen soll

**Typische Ausschlüsse:**

- Unerwünschte visuelle Artefakte
- Qualitätsmängel
- Stilistische Fehler
- Inhaltliche Störungen

**Beispiel:**

```
Negative Prompt: verschwommen, niedrige Qualität, 
verzerrte Gesichter, zusätzliche Gliedmaßen, Wasserzeichen, 
Text, unrealistische Proportionen, schlechte Beleuchtung
```

---

### Prompt-Gewichtung und Modifikatoren

**Gewichtung** (je nach Tool unterschiedlich):

```
(wichtiges Konzept:1.5), [weniger wichtiges Konzept:0.8]
```

**Stilmodifikatoren:**

- `ultra detailed, 8K resolution`
- `in the style of [Künstler/Bewegung]`
- `cinematic lighting, dramatic composition`
- `photorealistic, hyperrealistic`

**Technische Parameter:**

- Aspect Ratio: `--ar 16:9` oder `--aspect 1:1`
- Quality: `--q 2` (höhere Qualität)
- Stylize: `--s 750` (künstlerische Freiheit)

---

## 2. Systematischer Workflow

### Phase 1: Konzeption & Planung

1. **Zielsetzung klären**
   - Wofür wird das Bild benötigt?
   - Welche Zielgruppe?
   - Welcher Kontext (Präsentation, Arbeitsblatt, Social Media)?

2. **Recherche & Inspiration**
   - Referenzbilder sammeln
   - Stilrichtung definieren
   - Farbpalette überlegen

---

### Phase 2: Prompt-Entwicklung

**Strukturierte Prompt-Komponenten:**

#### #1 Hauptobjekt/Subjekt
```
Ein [spezifisches Objekt/Person/Konzept]
```

#### #2 Aktion/Zustand
```
[tut/ist/zeigt/präsentiert] [Aktivität]
```

#### #3 Setting/Szene
```
in/an/auf [Ort, Umgebung, Kontext]
```

#### #4 Atmosphäre/Stimmung
```
[Adjektive für Gefühl und Atmosphäre]
```

---

#### #5 Stil
```
[Kunststil, fotografischer Stil, Design-Ansatz]
```

**Beispiele:**
- Fotorealistisch
- Cartoon/Comic
- Aquarell/Ölgemälde
- Technische Illustration
- Infografik-Stil
- 3D-Render

#### #6 Technische Spezifikationen
```
[Auflösung], [Format], [Beleuchtung], [Perspektive]
```

---

### Phase 3: Iteration & Verfeinerung

**Iterativer Prozess:**

1. **Erste Generation:** Basis-Prompt testen
2. **Analyse:** Was funktioniert? Was fehlt?
3. **Anpassung:** Prompt verfeinern
4. **Variationen:** Seeds ändern, Parameter anpassen
5. **Auswahl:** Best-of-X wählen

**Tipp:** Dokumentieren Sie erfolgreiche Prompts für spätere Wiederverwendung!

---

### Phase 4: Nachbearbeitung

**Optionale Schritte:**

- **Inpainting:** Fehlerhafte Bereiche korrigieren
- **Upscaling:** Auflösung erhöhen
- **Color Grading:** Farbstimmung anpassen
- **Compositing:** Mehrere Generierungen kombinieren
- **Text-Overlay:** Beschriftungen hinzufügen (extern)

---

### Workflow-Checkliste

- [ ] Zielsetzung und Verwendungszweck definiert
- [ ] Referenzmaterial gesammelt
- [ ] Strukturierten Prompt erstellt (#Background, #Object, #Scene, etc.)
- [ ] Negativprompt formuliert
- [ ] Stil und technische Parameter festgelegt
- [ ] Format/Ratio passend gewählt
- [ ] Mehrere Variationen generiert
- [ ] Beste Version ausgewählt
- [ ] Bei Bedarf nachbearbeitet
- [ ] Lizenz/Nutzungsrechte geprüft

---

## 3. KI-Tools für die Bildung

### Kostenlose Tools (Educational Use)

#### 1. **ChatGPT mit DALL-E 3 (OpenAI)**

**Vorteile:**
- Dialogbasierte Bildgenerierung
- Iterative Verfeinerung möglich
- Kontextverständnis aus Konversation
- Gute Textdarstellung in Bildern

**Einschränkungen:**
- Nur 2 Bilder/Tag in kostenloser Version
- Erfordert OpenAI-Account

**Einsatz in der Bildung:**
- Schnelle Visualisierung im Unterricht
- Iterative Entwicklung von Konzepten
- Erklärung + Bild in einem Workflow

**Zugang:** https://chat.openai.com

#### 2. **Leonardo.AI (Free Tier)**

**Vorteile:**
- 150 Credits/Tag kostenlos
- Hochwertige Modelle
- Canvas-Editor für Nachbearbeitung
- Viele Preset-Stile

**Einsatz in der Bildung:**
- Charakterentwicklung für Storytelling
- Historische Rekonstruktionen
- Wissenschaftliche Illustrationen

**Zugang:** https://leonardo.ai

---

#### 3. **Canva for Education (mit Magic Studio)**

**Vorteile:**
- Kostenlos für verifizierte Lehrkräfte
- KI-Bildgenerierung + Design-Tools kombiniert
- Templates für Unterrichtsmaterialien
- Einfache Nachbearbeitung im selben Tool

**Einsatz in der Bildung:**
- Komplette Arbeitsblätter mit KI-Bildern
- Präsentationen erstellen
- Social Media für Schulprojekte

**Zugang:** https://canva.com/education

---

#### 4. **Ideogram.ai (Free)**

**Vorteile:**
- Hervorragende Textdarstellung
- Kostenlos nutzbar
- Poster und Designs
- Community-Inspiration

**Einsatz in der Bildung:**
- Poster für Klassenzimmer
- Infografiken mit Text
- Motivationsmaterial

**Zugang:** https://ideogram.ai

---

### Proprietäre/Premium-Tools

#### 1. **Adobe Firefly (Adobe Creative Cloud)**

**Kosten:** Teil der Adobe CC Subscription (~60€/Monat)

**Vorteile:**
- Kommerzielle Nutzung ohne Einschränkungen
- Integration in Photoshop, Illustrator
- "Generative Fill" für präzise Bearbeitung
- Trainiert nur auf lizenzierte Inhalte

**Einsatz:** Professionelle Materialerstellung

---

#### 2. **Midjourney V6**

**Kosten:** Ab $10/Monat (Basic), $30/Monat (Standard)

**Vorteile:**
- Höchste künstlerische Qualität
- Starke Community
- Konsistente Charaktere
- Fortgeschrittene Stilkontrolle

**Einsatz:** Hochwertige Bildungsmaterialien, Publikationen

---

#### 3. **Canva Pro mit Magic Studio**

**Kosten:** ~12€/Monat (kostenlos für verifizierte Lehrkräfte via Canva for Education)

**Vorteile:**
- KI-Bildgenerierung + Design-Tools
- Templates für Bildungsmaterialien
- Einfache Bedienung
- Team-Kollaboration

**Einsatz:** Komplette Unterrichtsmaterial-Erstellung



## 4. Typische Schwächen von KI-Bildgenerierung

### 1. Text und Schrift

**Problem:** Unleserlicher, falscher oder deformierter Text

**Beispiele:**
- Schilder mit Kauderwelsch
- Bücher mit unsinnigen "Buchstaben"
- Logos mit verzerrten Texten

**Ausnahmen:** DALL-E 3, Ideogram (verbessert)

**Workaround:** Text extern hinzufügen (Photoshop, Canva)

---

### 2. Zahlen und Mengen

**Problem:** Falsche Anzahl von Objekten

**Beispiele:**
- "Drei Äpfel" → Generiert 2 oder 5 Äpfel
- Falsche Finger-Anzahl (klassisches Problem!)
- Ungenaue Wiederholungsmuster

**Workaround:** 
- Sehr spezifische Prompts
- Mehrere Generierungen, beste auswählen
- Nachbearbeitung

---

### 3. Körperproportionen und Anatomie

**Problem:** Unnatürliche oder unmögliche Körperhaltungen

**Beispiele:**
- Zusätzliche oder fehlende Gliedmaßen
- Falsche Gelenkbiegungen
- Verschmelzende Körperteile

**Verbesserung:** Neuere Modelle deutlich besser

**Workaround:** 
- "Anatomically correct" im Prompt
- Negative Prompts nutzen

---

### 4. Räumliche Kohärenz

**Problem:** Perspektive und räumliche Beziehungen

**Beispiele:**
- Schatten in falsche Richtungen
- Objekte schweben ohne Grund
- Größenverhältnisse stimmen nicht

**Workaround:** 
- Präzise Positionsbeschreibungen
- Referenz auf Perspektive im Prompt

---

### 5. Konsistenz über mehrere Bilder

**Problem:** Charaktere/Objekte sehen anders aus

**Beispiel:** Serie von Unterrichtsmaterialien mit "derselben" Person

**Neuere Lösungen:**
- Midjourney: Character Reference (--cref)
- Leonardo: Character Consistency
- Custom Models (LoRA)

**Workaround:** Seed-Wiederverwendung, Image-to-Image

---

### 6. Komplexe Interaktionen

**Problem:** Mehrere Personen in komplexer Interaktion

**Beispiele:**
- Händeschütteln (verschmolzene Hände)
- Sportszenen mit mehreren Personen
- Werkzeugnutzung

**Workaround:** 
- Vereinfachen der Szene
- Schrittweise Komposition
- Inpainting für Problemzonen

---

### 7. Hintergrund-Anomalien

**Problem:** Unerklärliche oder surreale Hintergrundelemente

**Beispiele:**
- Schwebende Objekte ohne Kontext
- Geometrische Unmöglichkeiten
- "Traum-artige" Verzerrungen
- Unlogische Architektur

**Ursache:** KI "erfindet" Füllmaterial für unklare Bereiche

**Workaround:**
- Hintergrund explizit im Prompt beschreiben
- "Clean background" oder "simple background" verwenden
- Später manuell ausschneiden/ersetzen

---

### Schwächen-Übersicht für Lehrende

**Besonders vorsichtig bei:**

✗ Mathematischen Darstellungen mit Zahlen  
✗ Anatomischen Illustrationen  
✗ Texthaltigen Designs  
✗ Technischen Zeichnungen mit Präzisionsanforderungen  
✗ Kulturell sensiblen Darstellungen  

**Besser geeignet für:**

✓ Atmosphärische Szenen  
✓ Stilistische Illustrationen  
✓ Konzeptvisualisierungen  
✓ Diverse Stockfoto-Alternativen  
✓ Kreative Inspiration  

---

## 5. Realität vs. Digitale Realität

### Die Erosion der visuellen Wahrheit

**Historischer Kontext:**

- Fotografie galt lange als "Beweis"
- "Seeing is believing" verliert Gültigkeit
- Deepfakes und hyperrealistische KI-Bilder

**Konsequenzen:**

1. Vertrauenskrise in visuelle Medien
2. Notwendigkeit neuer Medienkompetenz
3. Ethische und rechtliche Herausforderungen

---

### Was ist "echt"?

**Philosophische Fragen:**

- Ist ein KI-generiertes Bild einer historischen Szene "echt"?
- Hat ein Bild ohne physische Kamera-Aufnahme weniger Wert?
- Wo liegt die Grenze zwischen "Illustration" und "Täuschung"?

**Praktische Kategorien:**

1. **Fotografische Wahrheit:** Echte Aufnahme
2. **Bearbeitete Realität:** Foto mit Nachbearbeitung
3. **Photo-bashing:** Mix aus Foto und KI/Malerei
4. **Vollständig Synthetisch:** 100% KI-generiert

---

### Zwecke von "nicht-echten" Bildern

#### Legitime Anwendungen

**1. Bildung & Illustration**
- Visualisierung abstrakter Konzepte
- Historische Rekonstruktionen
- Unmögliche/teure Szenarien darstellen

**2. Kreativität & Kunst**
- Künstlerischer Ausdruck
- Weltenbau (Worldbuilding)
- Konzeptentwicklung

**3. Inklusion & Diversität**
- Kostenlos diverse Darstellungen
- Vermeidung von Stock-Photo-Stereotypen
- Repräsentation erhöhen

---

#### Problematische Anwendungen

**1. Desinformation**
- Fake News mit "Beweisfotos"
- Historische Falschdarstellungen
- Politische Manipulation

**2. Betrug**
- Fake-Profile auf Social Media
- Täuschende Werbung
- Identitätsdiebstahl

**3. Urheberrechtsverletzungen**
- Nachahmung geschützter Stile
- "Laundering" von urheberrechtlich geschützten Inhalten

---

### Erkennungsstrategien für Lernende

**Visuelle Hinweise auf KI-Generierung:**

1. **Hände und Finger prüfen**
   - Häufigste Fehlerquelle
   
2. **Text und Schrift beachten**
   - Unleserlich oder sinnlos?
   
3. **Konsistenz der Beleuchtung**
   - Schatten passen zusammen?
   
4. **Unnatürliche Symmetrie**
   - Zu perfekt, um wahr zu sein?
   
5. **Hintergrund-Details**
   - "Verwaschene" oder inkonsistente Bereiche?

---

### Technische Nachweismethoden

**Emerging Technologies:**

- **Metadata-Analyse:** C2PA, Content Credentials
- **KI-Detektoren:** Hugging Face AI Detection
- **Reverse Image Search:** Originalquelle finden
- **Blockchain-Zertifizierung:** Authentizität nachweisen

**Problem:** Katz-und-Maus-Spiel zwischen Generierung und Detektion

---

### Medienkompetenz im KI-Zeitalter

**Neue Kernkompetenzen für Lehrende und Lernende:**

1. **Kritische Bildanalyse**
   - Nicht jedes Bild für bare Münze nehmen
   - Quellen prüfen
   - **Reflexion über Herkunft und Qualität als zentrale Lernaufgabe**

2. **Transparenz fordern**
   - Kennzeichnungspflicht für KI-Bilder
   - Disclosure verlangen

3. **Ethisches KI-Nutzung**
   - Ehrliche Kennzeichnung eigener KI-Bilder
   - Keine Täuschungsabsicht

4. **Urheberrecht verstehen**
   - Lizenzen beachten
   - Fair Use verstehen

5. **Bildkompetenz als Schlüsselqualifikation**
   - Herkunft hinterfragen
   - Manipulation erkennen
   - Eigene visuelle Kommunikation bewusst gestalten

---

### Handlungsempfehlungen für Lehrende

**DO's:**

✓ KI-Bilder transparent kennzeichnen  
✓ Kritisches Denken fördern  
✓ Quellenangaben machen  
✓ Ethische Nutzung vorleben  
✓ Alternativen zu Stock Photos nutzen  

**DON'Ts:**

✗ KI-Bilder als "echte Fotos" ausgeben  
✗ Urheberrechte ignorieren  
✗ Kritiklose Übernahme von KI-Ausgaben  
✗ Sensible Themen ohne Kontext darstellen  
✗ Lernende mit KI täuschen  

---

## 6. Praktische Übung

### Aufgabe für Studierende

**Szenario:** Erstellen Sie Bildmaterial für eine Unterrichtseinheit

**Schritte:**

1. Wählen Sie ein Forschungs- oder Lehrthema
2. Definieren Sie 3 Bilder, die Sie benötigen
3. Entwickeln Sie strukturierte Prompts (#Object, #Scene, #Style...)
4. Generieren Sie Bilder mit einem kostenlosen Tool
5. Dokumentieren Sie Ihre Prompts und Ergebnisse
6. Reflektieren Sie: Was funktionierte? Was nicht?

**Abgabe:** Prompts + Bilder + kurze Reflexion (1 Seite)

---

### Reflexionsfragen

1. **Technisch:** Welche Schwächen zeigten sich in Ihren Generierungen?

2. **Didaktisch:** Unterstützen die Bilder Ihre Lernziele?

3. **Ethisch:** Haben Sie die Bilder als KI-generiert gekennzeichnet?

4. **Praktisch:** War der Aufwand gerechtfertigt im Vergleich zu Stock-Fotos?

---

## 7. Zusammenfassung

### Key Takeaways

1. **Strukturierte Prompts** sind essentiell (Objekt, Szene, Stil, Parameter)
2. **Iteration** ist normal – erste Versuche sind selten perfekt
3. **Kostenlose Tools** sind für Bildungszwecke absolut ausreichend
4. **Schwächen kennen** – besonders bei Text, Zahlen, Anatomie
5. **Kritisch bleiben** – Unterscheidung Real/Digital wird schwieriger
6. **Transparent arbeiten** – KI-Nutzung ehrlich kommunizieren

---

### Best Practices

**Workflow-Regel:**

> Planen → Prompten → Prüfen → Verfeinern → Kennzeichnen

**Ethik-Regel:**

> Wenn Sie sich fragen "Sollte ich kennzeichnen, dass dies KI ist?" 
> – Dann lautet die Antwort: JA.

**Qualitäts-Regel:**

> Generieren Sie immer mehrere Varianten und wählen Sie bewusst aus.

## Diskussion & Fragen

**Diskussionsthemen:**

- Sollten KI-Bilder im akademischen Kontext zugelassen werden?
- Wie gehen wir mit "AI-Washing" um (KI behaupten, aber Stock-Foto nutzen)?
- Brauchen wir neue Standards für visuelle Zitation?

**Ihre Fragen?**

---

## Kontakt & Lizenz

**Hannes Tegelbeckers*  
Otto-von-Guericke-Universität Magdeburg  
hannes.tegelbeckers@ovgu.de

**Lizenz:** CC-BY-SA 4.0  
Sie dürfen dieses Material teilen und bearbeiten unter Nennung der Quelle.

**Diese Präsentation wurde erstellt mit:** LiaScript + Claude (Anthropic)  
→ Transparenz in der KI-Nutzung!
