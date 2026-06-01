<!--
  SETUP — ersetzen Sie diese beiden Platzhalter vor der Veröffentlichung überall:
    {{WEBSITE_URL}}    →  Ihre offizielle Website, z. B. https://veo-automation.example.com
    {{EXTENSION_URL}}  →  die URL Ihres Chrome-Web-Store-Eintrags (ohne Query-String)
  Die Erweiterungslinks hängen pro Sprachdatei bereits ?hl={lang} an. Führen Sie ein globales
  Suchen/Ersetzen über alle 7 README-Dateien hinweg durch (README.md, README_zh/ko/ja/de/fr/ru.md).
-->

[![Im Chrome Web Store installieren](https://img.shields.io/badge/⬇_Installieren-Chrome_Web_Store-success?style=for-the-badge&logo=googlechrome&logoColor=white)]({{EXTENSION_URL}}?hl=de)
[![Website](https://img.shields.io/badge/🌐_Website-Besuchen-blue?style=for-the-badge)]({{WEBSITE_URL}})

# 🎬 VEO Automation — Google Flow Automatisierung für VEO 3 Videos & Nano Banana Bilder im Batch

[![English](https://img.shields.io/badge/English-blue)](README.md) [![中文](https://img.shields.io/badge/中文-red)](README_zh.md) [![한국어](https://img.shields.io/badge/한국어-orange)](README_ko.md) [![日本語](https://img.shields.io/badge/日本語-purple)](README_ja.md) [![Deutsch](https://img.shields.io/badge/Deutsch-green)](README_de.md) [![Français](https://img.shields.io/badge/Français-yellow)](README_fr.md) [![Русский](https://img.shields.io/badge/Русский-lightgrey)](README_ru.md)

> **VEO Automation** ist die Chrome-Erweiterung, die [Google Flow](https://labs.google/fx/tools/flow) in ein Studio für Batch-Generierung verwandelt. Stellen Sie hunderte Prompts in die Warteschlange, erzeugen Sie **VEO 3** Videos und **Nano Banana** Bilder in großen Mengen und laden Sie jedes Ergebnis automatisch herunter — Schluss mit dem Babysitten einzelner Prompts.

**Keywords, die dieser Leitfaden abdeckt:** Google Flow Automatisierung · VEO Automatisierung · VEO 3 Stapelgenerierung (VEO 3 batch generation) · Nano Banana Bilder Batch · KI-Video Massengenerator (bulk AI video generator) · VEO Videos automatisch herunterladen · Google Flow Chrome-Erweiterung.

---

## 📑 Inhaltsverzeichnis

- [Warum VEO Automation](#-warum-veo-automation)
- [Hauptfunktionen](#-hauptfunktionen)
- [Installation](#-installation)
- [Schnellstart](#-schnellstart)
- [Generierungsmodi](#-generierungsmodi)
- [Einstellungsreferenz](#️-einstellungsreferenz)
- [Tipps & Best Practices](#-tipps--best-practices)
- [Fehlerbehebung](#-fehlerbehebung)
- [FAQ](#-faq)
- [Datenschutz & Berechtigungen](#-datenschutz--berechtigungen)
- [Preise](#-preise)

---

## 🚀 Warum VEO Automation

Google Flow ist leistungsstark, aber die offizielle Oberfläche zwingt Sie, **einen Prompt nach dem anderen** auszuführen und **jede Datei einzeln** herunterzuladen. Wenn Sie Inhalte in großem Umfang produzieren — Kurzvideos, Marketing-Creatives, Storyboards, Produktaufnahmen — wird diese manuelle Schleife zum Engpass.

VEO Automation beseitigt ihn:

- **Liste einfügen, weggehen.** Werfen Sie dutzende oder hunderte Prompts hinein, und die Erweiterung verarbeitet sie nacheinander, inklusive Wiederholungen, während Sie etwas anderes tun.
- **VEO 3 Videos *und* Nano Banana Bilder in einem Tool.** Die meisten Automatisierungen kümmern sich nur um Video. Diese hier verarbeitet sowohl die Video-Modelle von Google Flow als auch das Bildmodell Nano Banana im Batch — aus einer einzigen Seitenleiste.
- **Dateien landen automatisch auf der Festplatte.** Jedes fertige Video und Bild wird umbenannt und in einem projektspezifischen Ordner gespeichert — kein Rechtsklick-Speichern-Marathon.

Wenn Sie nach einem *Google Flow Batch-Tool*, einem *VEO 3 Massengenerator* oder einer Möglichkeit gesucht haben, *Nano Banana Bilder automatisch herunterzuladen*, dann ist genau dafür dieses Tool gebaut.

---

## ✨ Hauptfunktionen

| Funktion | Was sie leistet |
| --- | --- |
| 🚀 **Batch-Warteschlange** | Fügen Sie unbegrenzt viele Prompts zu einer Warteschlange hinzu; die Aufgaben laufen automatisch nacheinander ab. |
| 📝 **Text-zu-Video (VEO 3)** | Fügen Sie Prompts ein oder laden Sie eine `.txt`-Datei mit hunderten Zeilen hoch, um Videos in Masse zu produzieren. |
| 🖼️ **Bild-zu-Video (VEO 3)** | Erwecken Sie Standbilder mit Start-Frame- / End-Frame-Steuerung zum Leben. |
| 🎨 **Text-zu-Bild (Nano Banana)** | Erzeugen Sie Bilder aus Textbeschreibungen im Batch. |
| 🔄 **Bild-zu-Bild (Nano Banana)** | Transformieren oder bearbeiten Sie Referenzbilder in großem Umfang. |
| 💾 **Automatischer Download** | Speichert fertige Videos und Bilder sofort auf Ihrem Rechner, geordnet nach Projektordner. |
| 🔁 **Automatische Wiederholung** | Netzwerk-Aussetzer oder „Erstellung fehlgeschlagen“ auf Googles Seite? Es wartet und wiederholt automatisch. |
| 🔗 **Clip-Verkettung (Concat)** | Fügen Sie 8-Sekunden-Segmente zu längeren, durchgehenden Videos zusammen. |
| ⚙️ **Tiefe Anpassung** | Wählen Sie Modell, Seitenverhältnis (16:9 / 9:16 / 1:1), Ausgaben pro Prompt (1–4), gleichzeitige Ausführung und Verzögerung pro Prompt. |
| 🌍 **7 Sprachen** | English, 中文, 한국어, 日本語, Deutsch, Français, Русский. |

---

## 📥 Installation

### Chrome Web Store (empfohlen)

1. Öffnen Sie den [**VEO-Automation-Eintrag**]({{EXTENSION_URL}}?hl=de) im Chrome Web Store.
2. Klicken Sie auf **Zu Chrome hinzufügen** → **Erweiterung hinzufügen**.
3. Heften Sie die Erweiterung an: Klicken Sie auf das Puzzleteil-Symbol in der Chrome-Symbolleiste und dann auf die Stecknadel neben **VEO Automation**, damit sie beim nächsten Mal nur einen Klick entfernt ist.

> **Kompatibilität:** Chrome 137+ (und Chromium-basierte Browser wie Edge und Brave). Die Erweiterung öffnet sich als **Seitenleiste** neben Google Flow.

---

## ⚡ Schnellstart

1. **Google Flow öffnen.** Gehen Sie zu [labs.google/fx/tools/flow](https://labs.google/fx/tools/flow) und öffnen (oder erstellen) Sie ein Projekt. Die Erweiterung wird nur auf Flow-Projektseiten aktiv.
2. **Seitenleiste öffnen.** Klicken Sie auf das VEO-Automation-Symbol. Melden Sie sich an, um Ihr Tageskontingent freizuschalten.
3. **Modus wählen.** Wählen Sie einen der fünf Generierungsmodi (siehe unten).
4. **Prompts hinzufügen.** Tippen Sie sie ein oder laden Sie eine `.txt`-Datei hoch.
5. **Auf Ausführen klicken.** Beobachten Sie, wie die Warteschlange jede Aufgabe verarbeitet, bei Fehlern wiederholt und Ergebnisse automatisch herunterlädt.

> ℹ️ **Hinweis zum „Debugging“-Banner.** Während die Erweiterung läuft, zeigt Chrome oben eine Leiste mit *„… wird debuggt“* an. Das ist erforderlich: Google Flow akzeptiert nur echte, vertrauenswürdige Benutzereingaben, daher steuert die Erweiterung die Seite über die offizielle Debugging-Schnittstelle von Chrome. Das ist keine Malware — es ist der Preis für zuverlässige Automatisierung. Schließen Sie das Banner nicht, während ein Batch läuft.

---

## 🎛️ Generierungsmodi

### 1. Text-zu-Video — VEO 3

Produzieren Sie Videos direkt aus Text in Masse.

1. Wählen Sie **Text-zu-Video**.
2. Geben Sie Prompts in das Feld ein (trennen Sie jeden Prompt durch eine **Leerzeile**) **oder** klicken Sie auf **.txt hochladen**, um eine Prompt-Liste zu importieren.
3. Legen Sie die Dauer fest (einzelner 8-s-Clip oder **Concat** für längere verkettete Videos).
4. Klicken Sie auf **Ausführen**.

**Beispiel-Prompt-Liste:**

```
Ein einsamer Leuchtturm auf einer Klippe zur goldenen Stunde, Wellen brechen darunter, langsame kinematische Kamerafahrt nach vorne.

Eine neonbeleuchtete Tokioter Gasse im Regen, Spiegelungen auf nassem Asphalt, aufsteigender Dampf, Handkamera-Anmutung.

Luftaufnahme im Gleitflug über einen Herbstwald, tiefer Morgennebel zwischen den Bäumen, warmes Licht.
```

### 2. Bild-zu-Video — VEO 3

Erwecken Sie Standbilder zum Leben.

1. Wählen Sie **Bild-zu-Video**.
2. Klicken Sie auf **Bilder auswählen** (Mehrfachauswahl unterstützt) und ziehen Sie sie, um sie nach Name, Datum oder eigener Reihenfolge zu sortieren.
3. Schreiben Sie einen Prompt pro Bild (durch Leerzeile getrennt).
4. Wählen Sie die Dauer und klicken Sie dann auf **Ausführen**.

> **Tipp:** Verwenden Sie einen Start-Frame + End-Frame, um zu steuern, wie die Bewegung beginnt und endet. Konfigurieren Sie 1–2 Bilder pro Prompt in den Einstellungen.

### 3. Text-zu-Bild — Nano Banana

Erzeugen Sie Bilder aus Beschreibungen, im Batch.

1. Wählen Sie **Text-zu-Bild**.
2. Geben Sie detaillierte Bild-Prompts ein (durch Leerzeile getrennt).
3. Legen Sie Seitenverhältnis und Bildqualität in den Einstellungen fest.
4. **Ausführen** — jedes Bild wird automatisch in der von Ihnen gewählten Auflösung heruntergeladen (1K / 2K / 4K).

### 4. Bild-zu-Bild — Nano Banana

Bearbeiten oder verändern Sie den Stil von Referenzbildern in großem Umfang.

1. Wählen Sie **Bild-zu-Bild**.
2. Laden Sie Quellbilder hoch.
3. Schreiben Sie Transformations-Prompts (z. B. *„dieselbe Figur, Cyberpunk-Outfit, Dachterrasse bei Nacht“*).
4. **Ausführen**, um Varianten basierend auf Ihren Referenzen zu erzeugen.

> **Figuren automatisch per Dateiname zuordnen (optional):** Benennen Sie Ihre Referenzen `dog.png`, `cat.png`, `duck.png`. Ein Prompt, der *„Hund spielt mit Katze“* erwähnt, zieht automatisch `dog.png` und `cat.png` heran. Perfekt, um Figuren über eine Serie hinweg konsistent zu halten.

### 5. Warteschlangen-Verwaltung

- Sehen Sie jede ausstehende Aufgabe in der **Prompt-Warteschlange**.
- **Entfernen** Sie Aufgaben, die Sie nicht mehr benötigen, oder **stoppen** Sie einen laufenden Batch.
- Verfolgen Sie den Fortschritt pro Prompt in Echtzeit.

---

## ⚙️ Einstellungsreferenz

Öffnen Sie den Tab **Einstellungen**, um das Verhalten anzupassen.

**Allgemein**
- **Standardmodus** — wird bei jedem Öffnen der Seitenleiste automatisch ausgewählt.
- **Standard-Seitenverhältnis** — 16:9, 9:16 oder 1:1.
- **Ausgaben pro Prompt** — 1–4 Videos/Bilder pro Prompt.
- **Gleichzeitige Prompts** — führen Sie 1–6 Prompts gleichzeitig aus.
- **Prompt-Verzögerung** — warten Sie 0–300 s zwischen Prompts, um die Serverlast zu verringern.

**Modelle**
- **Video-Modell** — wählen Sie Ihr VEO-Modell (z. B. VEO 3 / VEO 3 Fast).
- **Bild-Modell** — Nano Banana für Text-zu-Bild und Bild-zu-Bild.

**Download**
- **Videoqualität** — 720p, 1080p oder aus.
- **Bildqualität** — 1K, 2K, 4K oder aus.
- Dateien werden im Chrome-Downloads-Ordner gespeichert, ein Unterordner pro Projekt.

**Erweitert**
- **Maximale Wiederholungen** — 1–20 Versuche bei Fehlern.
- **Standard-Video-Frame** — 8 s oder Concat.
- **Max. Bilder pro Prompt** — pro Modus einstellbar.
- **Sprache** — wechseln Sie die Oberfläche zwischen 7 Sprachen.

---

## 💡 Tipps & Best Practices

**Prompts schreiben**
- Seien Sie präzise bei Motiv, Stil, Kamerabewegung und Beleuchtung.
- Englische Prompts sind auf Google Flow tendenziell am zuverlässigsten.
- Trennen Sie Prompts durch eine einzelne Leerzeile.

**Durchsatz vs. Stabilität**
- Außerhalb der Stoßzeiten: ~3 gleichzeitige Prompts funktionieren gut.
- Zu Stoßzeiten: gehen Sie auf 2 herunter und erhöhen Sie die Verzögerung auf ~30 s — weniger „Erstellung fehlgeschlagen“-Fehler.
- Mehr gleichzeitige Ausführung = schneller, aber weniger stabil; passen Sie es nach Geschmack an.

**Assets verwalten**
- Benennen Sie Referenzbilder eindeutig, damit die automatische Zuordnung funktioniert.
- Bleiben Sie bei PNG / JPG / GIF, idealerweise jeweils unter 10 MB.

**Zuverlässigkeit**
- Lassen Sie die **automatische Wiederholung** für unbeaufsichtigte Batches über Nacht aktiviert.
- Höhere Verzögerung = geringere Serverlast = weniger Fehler.

---

## 🔧 Fehlerbehebung

| Symptom | Ursache & Lösung |
| --- | --- |
| **Erweiterung tut nichts** | Sie müssen sich auf einer Google-Flow-**Projektseite** befinden. Stellen Sie sicher, dass die Erweiterung aktiviert ist, aktualisieren Sie die Seite und öffnen Sie die Seitenleiste erneut. |
| **„Video kann nicht erstellt werden“** | Google Flow ist vorübergehend überlastet. Keine Sorge — die Erweiterung wartet und wiederholt etwa alle 30 s, bis ein Platz frei wird. |
| **Videos/Bilder werden nicht heruntergeladen** | In Chrome: **Einstellungen → Downloads → deaktivieren** Sie *„Vor dem Download von Dateien nach dem Speicherort fragen“*. Prüfen Sie anschließend die Download-Qualität in den Einstellungen erneut. |
| **„Richtlinienfehler“** | Ihr Prompt oder Bild hat Googles Inhaltsrichtlinie ausgelöst. Das Tool überspringt diese Aufgabe und geht automatisch zur nächsten über. |
| **Generierung schlägt ständig fehl** | Prüfen Sie Ihre Verbindung, vergewissern Sie sich, dass die Prompts gültig sind, erhöhen Sie die maximalen Wiederholungen und sehen Sie sich die Browser-Konsole nach Hinweisen an. |
| **Die Seite hat von selbst herausgezoomt** | Beabsichtigt — das Tool passt den Zoom an, um Schaltflächen präzise zu finden. Ändern Sie den Zoom nicht manuell, während ein Batch läuft. |
| **„Wird debuggt“-Banner verschwindet nicht** | Während des Laufs zu erwarten (siehe Schnellstart). Es verschwindet, wenn der Batch fertig ist oder Sie ihn stoppen. |

---

## ❓ FAQ

**Ist VEO Automation mit Google verbunden?**
Nein. Es ist ein unabhängiges Drittanbieter-Tool, das die öffentliche Google-Flow-Web-App automatisiert. Es ist nicht mit Google verbunden, wird nicht von Google unterstützt und steht in keiner Beziehung zu Google.

**Was ist Nano Banana?**
Nano Banana ist das Bildmodell, das über Google Flow verfügbar ist. Mit VEO Automation können Sie Nano Banana Bilder im Batch erzeugen und automatisch herunterladen — zusammen mit Ihren VEO 3 Videos, aus derselben Warteschlange.

**Kann ich wirklich hunderte Videos auf einmal generieren?**
Ja. Laden Sie eine `.txt`-Datei mit Prompts hoch (oder fügen Sie eine lange Liste ein), und die Warteschlange verarbeitet sie nacheinander mit automatischen Wiederholungen. Der praktische Durchsatz hängt von der Auslastung von Google Flow und Ihren Einstellungen für gleichzeitige Ausführung und Verzögerung ab.

**Funktioniert es für vertikale Kurzvideos?**
Ja — stellen Sie das Seitenverhältnis auf **9:16** für TikTok / Reels / Shorts, **16:9** für YouTube oder **1:1** für quadratisch ein.

**Wohin gelangen meine Dateien?**
In Ihren Chrome-Downloads-Ordner, geordnet in einen Unterordner pro Projekt, automatisch umbenannt, sodass sie sich leicht sortieren lassen.

**Brauche ich einen API-Schlüssel?**
Nein. Es steuert Ihre eigene angemeldete Google-Flow-Sitzung im Browser — kein separater API-Schlüssel und kein Entwicklerkonto erforderlich.

**Werden meine Daten irgendwohin gesendet?**
Ihre Prompts, Bilder und Videos werden in Ihrem Browser auf Google Flow verarbeitet. Die Erweiterung speichert Einstellungen lokal. Siehe [Datenschutz & Berechtigungen](#-datenschutz--berechtigungen).

**Welche Browser werden unterstützt?**
Chrome 137+ und Chromium-basierte Browser (Edge, Brave). Eine Seitenleiste ist erforderlich.

---

## 🔒 Datenschutz & Berechtigungen

- **Läuft in Ihrem Browser.** Die Automatisierung findet in Ihrer eigenen Google-Flow-Sitzung statt.
- **Minimale Daten.** Einstellungen werden im lokalen Chrome-Speicher abgelegt. Die Erweiterung verkauft oder sammelt Ihre kreativen Inhalte nicht.
- **Eng gefasste Berechtigungen.** Der Host-Zugriff ist auf `labs.google/*` (zur Automatisierung von Flow) und das eigene Backend der Erweiterung (für Anmeldung und Kontingent) beschränkt.
- **Die Debugger-Berechtigung** wird ausschließlich verwendet, um vertrauenswürdige Eingabeereignisse an Google Flow zu senden, was die Seite erfordert — siehe [Schnellstart](#-schnellstart).

Vollständige Details: [{{WEBSITE_URL}}]({{WEBSITE_URL}})

---

## 💳 Preise

VEO Automation ist **Freemium**:

- **Kostenlos** — ein tägliches Generierungskontingent, das sich jeden Tag zurücksetzt. Ideal zum Ausprobieren und für die gelegentliche Nutzung.
- **Pro** — höheres oder unbegrenztes Kontingent für Power-User, die große Batches fahren.

Melden Sie sich in der Seitenleiste an, um Ihr aktuelles Kontingent zu sehen. Verwalten Sie Ihren Tarif unter [{{WEBSITE_URL}}]({{WEBSITE_URL}}).

---

## 🌐 Links

- **Installieren:** [Chrome Web Store]({{EXTENSION_URL}}?hl=de)
- **Website:** [{{WEBSITE_URL}}]({{WEBSITE_URL}})
- **Google Flow:** [labs.google/fx/tools/flow](https://labs.google/fx/tools/flow)

---

_Haftungsausschluss: VEO Automation ist ein unabhängiges Projekt und **nicht** mit Google oder dem Google-Flow-Team verbunden, wird nicht von ihnen unterstützt und steht in keiner Beziehung zu ihnen. „VEO“, „Nano Banana“, „Google Flow“ und „Google“ sind Marken von Google LLC. Die Nutzung dieses Tools unterliegt den Nutzungsbedingungen von Google._
