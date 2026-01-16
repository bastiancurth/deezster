<div align="center">

# DEEZSTER

<img src="logo.png" alt="Deezster Logo" width="300" height="auto">

### Das Musik-Quiz für die Hosentasche.
### Errate das Jahr, powered by Deezer.

[Live Demo ansehen](https://DEIN-USERNAME.github.io/DEIN-REPO-NAME/)

</div>

---

## 🎵 Über das Projekt

**Deezster** ist ein interaktives Musik-Quiz, inspiriert von dem bekannten Brettspiel "Hitster". Es ist eine One-Page Web-App, die du im Browser auf deinem Handy oder Desktop spielen kannst.

Das Ziel ist simpel: Du hörst einen 30-sekündigen Ausschnitt eines Songs und musst erraten, in welchem Jahr er veröffentlicht wurde. Je näher du dran bist, desto besser!

## ✨ Features

* **Keine Anmeldung nötig:** Sofort loslegen.
* **Deezer Integration:** Nutze die riesige Musikbibliothek von Deezer.
* **Playlist Suche:** Suche direkt in der App nach Playlists (z.B. "80er Rock", "Disney", "Techno Bunker") oder nutze die vorgegebenen Vorschläge.
* **Responsive Design:** Sieht auf dem Smartphone aus wie eine native App.
* **Vinyl Animation:** Eine sich drehende Schallplatte zeigt an, wenn Musik spielt.
* **Direktes Feedback:** Farbliche Markierung, wie nah dein Tipp am richtigen Jahr lag.

## 🛠️ Technologie-Stack

Das Projekt ist bewusst simpel gehalten und kommt ohne eigenes Backend aus ("Serverless").

* **Frontend:** Reines HTML5, CSS3 und Vanilla JavaScript (keine Frameworks).
* **Datenquelle:** Öffentliche [Deezer API](https://developers.deezer.com/api) (für Songs, Cover und Hörproben).
* **Proxy:** Nutzt einen öffentlichen CORS-Proxy (z.B. `allorigins.win`), um API-Anfragen direkt aus dem Browser zu ermöglichen.

## 🚀 Installation & Nutzung lokal

Da es sich um eine statische Seite handelt, ist die "Installation" sehr einfach:

1.  **Repository klonen:**
    ```bash
    git clone [https://github.com/DEIN-USERNAME/DEIN-REPO-NAME.git](https://github.com/DEIN-USERNAME/DEIN-REPO-NAME.git)
    ```
2.  **Ordner öffnen:**
    Navigiere in den heruntergeladenen Ordner.
3.  **Starten:**
    Öffne einfach die Datei `index.html` in deinem bevorzugten Webbrowser (Chrome, Firefox, Edge, Safari).

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
