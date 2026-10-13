# PC-Werkstatt

Eine persönliche Lernseite, mit der man den Computer Schritt für Schritt lernt – in sieben Schritten:

1. Tippen mit 10 Fingern (9 Lektionen und das Spiel „Buchstabenregen“)
2. Die Maus (Klicken, Doppelklick, Rechtsklick, Ziehen)
3. Tastenkürzel (Quiz mit der echten Tastatur)
4. Word (Texte gestalten)
5. Excel (Zellen, Formeln, Summe)
6. Dateien & Ordner (Übungs-Explorer und „Speichern unter“)
7. Internet & E-Mail (Suchen, Werbung erkennen, Mails, Betrug erkennen)

Am Ende gibt es eine Urkunde zum Ausdrucken. Alles läuft im Browser – ohne Anmeldung, ohne Server, ohne Installation.

## Was im Paket ist

| Datei / Ordner | Inhalt |
|---|---|
| `index.html` | die komplette Seite |
| `fonts/` | die Schriften und ihre Lizenztexte |
| `README.md` | diese Anleitung |

Zum Ausprobieren ohne GitHub: einfach `index.html` doppelklicken.

## Auf GitHub Pages veröffentlichen (nur im Browser, ohne Zusatzprogramme)

1. Auf [github.com](https://github.com) anmelden (oder kostenlos registrieren).
2. Rechts oben auf **+** → **New repository**. Als Namen zum Beispiel `pc-werkstatt` eintragen. Sichtbarkeit **Public** wählen (im kostenlosen Konto ist GitHub Pages nur für öffentliche Repositories verfügbar). Dann **Create repository**.
3. Auf der noch leeren Seite des Repositorys auf **uploading an existing file** klicken (oder **Add file → Upload files**). `index.html`, `README.md` und den ganzen Ordner `fonts` in das Fenster ziehen. Unten auf **Commit changes** klicken.
4. Oben auf **Settings** → links **Pages**. Unter **Build and deployment** bei **Source** „Deploy from a branch“ wählen, als Branch `main` und als Ordner `/ (root)`, dann **Save**.
5. Nach ein bis zwei Minuten ist die Seite erreichbar unter:
   `https://DEIN-BENUTZERNAME.github.io/pc-werkstatt/`

### Alternativ mit git

```bash
git init
git add .
git commit -m "PC-Werkstatt"
git branch -M main
git remote add origin https://github.com/DEIN-BENUTZERNAME/pc-werkstatt.git
git push -u origin main
```

Danach wie oben Schritt 4 (Pages einschalten).

## Persönlich machen

Es gibt zwei Wege:

- **Auf der Seite (empfohlen):** Startseite → „⚙️ Persönlich machen“. Dort lassen sich Vorname, eine persönliche Nachricht, Wohnort, Hobbys, Lieblingsessen, wichtige Menschen und ein Haustier eintragen. Diese Angaben tauchen in Tipp-Sätzen, E-Mails, auf der Startseite und auf der Urkunde auf. Sie werden **nur im Browser auf diesem Computer** gespeichert.
- **In der Datei:** Ganz oben im `<script>`-Teil von `index.html` steht `CONFIG` mit `name`, `von` und `nachricht`. Das sind die Voreinstellungen für alle, die die Seite öffnen. **Achtung: Auf GitHub ist diese Datei öffentlich lesbar.** Private Details deshalb nicht hier eintragen.

## Datenschutz

- Kein Login, kein Tracking, keine Cookies. Fortschritt und persönliche Angaben bleiben im Browser (`localStorage`) des Computers, auf dem geübt wird. Ein anderer Computer oder Browser beginnt von vorne.
- Die Schriften werden aus dem Ordner `fonts/` geladen, nicht von Google-Servern. Hintergrund: Das Landgericht München I hat 2022 das Einbinden von Google Fonts direkt von Google-Servern ohne Einwilligung als DSGVO-Verstoß gewertet (Az. 3 O 17493/20).
- GitHub protokolliert beim Aufruf einer GitHub-Pages-Seite laut eigener Dokumentation die IP-Adresse der Besucher aus Sicherheitsgründen.
- Die Seite ist für Suchmaschinen gesperrt (`noindex`). Wer den Link kennt, kann sie trotzdem öffnen.
- Österreich: Für Websites gilt grundsätzlich die Offenlegungspflicht nach § 25 Mediengesetz. Ob und in welchem Umfang das für eine private Übungsseite greift, bitte selbst prüfen (das ist keine Rechtsberatung).

## Gut zu wissen

- Gemacht für einen Computer mit Tastatur und Maus, österreichisch-deutsche Tastenbelegung (QWERTZ).
- Alle Webseiten, Firmen und Mail-Adressen in den Übungen sind erfunden und enden auf `.example` – eine Endung, die nur für Beispiele reserviert ist.

## Quellen

- GitHub Pages, Verfügbarkeit und Datenerfassung: https://docs.github.com/de/pages/getting-started-with-github-pages/what-is-github-pages
- LG München I, Urteil vom 20.01.2022, Az. 3 O 17493/20 (Google Fonts), Zusammenfassung u. a. der Landesbeauftragten für den Datenschutz Niedersachsen: https://lfd.niedersachsen.de/download/190184

## Schriften und Lizenzen

Atkinson Hyperlegible (© Braille Institute of America), Atkinson Hyperlegible Mono und Bricolage Grotesque stehen unter der SIL Open Font License 1.1. Die Lizenztexte liegen im Ordner `fonts/`.
