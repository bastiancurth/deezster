<div align="center">

# 💿 DEEZSTER 2.3
### Die ultimative Musik-Timeline & Highscore Challenge

![Deezster Logo](logo.png)
*(Füge hier dein Logo ein oder lösche die Zeile)*

[**🔴 LIVE DEMO HIER KLICKEN**](https://DEIN-USERNAME.github.io/DEIN-REPO-NAME/)

</div>

---

## 🎵 Was ist Deezster?

**Deezster** ist eine interaktive Musik-Quiz-App, die direkt im Browser läuft. Inspiriert vom Brettspiel "Hitster", nutzt sie die riesige Bibliothek von Deezer, um deine Musikkenntnisse auf die Probe zu stellen.

Die Version 2.3 kommt im modernen **"Premium Glass"-Design**, bietet zwei völlig unterschiedliche Spielmodi und eine intelligente Logik, um echte Aufnahmejahre von Remasters zu unterscheiden.

## ✨ Features

* **2 Spielmodi:** Wähle zwischen strategischem Einordnen (Timeline) oder schnellem Wissen (Highscore).
* **Smart Year Detection:** Ein Algorithmus prüft ISRC-Daten, um das *echte* Aufnahmejahr zu finden, selbst wenn das Album ein "Remaster 2011" ist.
* **Kein Login nötig:** Sofort loslegen, keine Anmeldung bei Deezer erforderlich.
* **Deezer Integration:** Zugriff auf Millionen von Songs und 30-Sekunden-Previews.
* **Responsive Design:** Fühlt sich auf dem Smartphone wie eine native App an.
* **Visuelle Effekte:** Animierte Vinyl-Platten, dynamische Hintergründe und Glassmorphism-UI.

---

## 🎮 Die Spielmodi

### 1. 📅 Timeline Modus (Das Original)
Das klassische Prinzip für Strategen.
* **Ziel:** Ordne Songs chronologisch auf deinem Zeitstrahl ein.
* **Ablauf:** Du hörst einen Song und musst entscheiden: War er *vor* oder *nach* den Songs, die schon liegen? Oder genau dazwischen?
* **Regeln:** Du hast **3 Leben**. Ein Fehler kostet ein Herz.
* **Gewinnbedingung:** Erreiche das Ziel von 10, 15 oder 20 korrekten Karten (einstellbar).

### 2. ⚡ Highscore Jagd (Quiz)
Das schnelle Spiel für Zwischendurch ("Sudden Death").
* **Ziel:** Errate den Songtitel aus 4 Möglichkeiten.
* **Score-System:** Je schneller du antwortest, desto mehr Punkte gibt es (Max. 1000 pro Song).
* **Regeln:** Ein einziger Fehler bedeutet sofortiges **Game Over**!
* **Visuals:** Ein Timer-Balken zeigt dir den Zeitdruck an.

---

## 🛠️ Technologie & Setup

Das Projekt ist "Serverless" und läuft zu 100% im Client (Browser).

* **Frontend:** HTML5, CSS3, Vanilla JavaScript.
* **API:** Deezer API (via JSONP für CORS-Umgehung ohne Proxy).
* **Hosting:** Optimiert für **GitHub Pages**.

### Installation (Eigene Version hosten)

1.  **Repository erstellen:** Erstelle ein neues Repo auf GitHub.
2.  **Dateien hochladen:** Lade die `index.html` (und optional ein `logo.png`) hoch.
3.  **Pages aktivieren:**
    * Gehe im Repo zu `Settings` -> `Pages`.
    * Wähle unter "Branch" `main` (oder `master`) und speichere.
4.  **Fertig:** Nach ca. 1 Minute ist dein Spiel unter `https://deinuser.github.io/deinrepo/` erreichbar.

---

## 🤓 Für Entwickler: Der "Remaster-Fix"

Ein häufiges Problem bei Musik-APIs ist, dass bei "Best Of" Alben das Jahr der Compilation (z.B. 2010) statt des Songs (z.B. 1975) geliefert wird.

Deezster 2.3 löst das durch einen **ISRC-Check**:
1.  Die App holt das Album-Datum.
2.  Sie prüft den ISRC-Code des Tracks (Zeichen 6 & 7 stehen oft für das Jahr).
3.  Sie vergleicht beide und wählt intelligent das **ältere, plausible Jahr** aus.

```javascript
// Beispiel Logik
if (isrcYear < albumYear && isrcYear > 1900) {
    finalYear = isrcYear; // Nimm das echte Aufnahmejahr!
}

## ⚠️ Wichtiger Hinweis zur API

Dieses Projekt nutzt die *öffentliche* Deezer API über einen *öffentlichen* CORS-Proxy.
* Es ist **kein API-Key** notwendig.
* Für ein Hobby-Projekt funktioniert dies gut. Bei sehr vielen gleichzeitigen Nutzern könnte der öffentliche Proxy jedoch an seine Grenzen stoßen und die Musik könnte langsamer laden.

## 👏 Credits

* Musikdaten bereitgestellt von [Deezer](https://www.deezer.com).
* Inspiriert durch das Spielprinzip von Hitster.
* Icons by [FontAwesome](https://fontawesome.com/).

---

<div align="center">
Erstellt mit ❤️ und viel Musik.
</div>
