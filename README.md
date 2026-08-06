https://florianalternativ-cmyk.github.io/it-survival-9to5/



# IT-SURVIVAL — Mobile Edition V4

Ein vollständiges, statisches Mobile-Browsergame im Retro-Pixelstil. Keine Installation, kein Build-Schritt und keine externen Abhängigkeiten: `index.html` enthält das komplette Spiel.

## Neues Test-Repository veröffentlichen

1. Auf GitHub ein **neues leeres Repository** anlegen.
2. Alle Dateien aus dem ZIP einschließlich `.github` und `.nojekyll` direkt in den Repository-Root hochladen.
3. Unter **Settings → Pages → Build and deployment** als Source **GitHub Actions** auswählen.
4. Den Workflow **Deploy IT-SURVIVAL to GitHub Pages** abwarten.
5. Die angezeigte Test-URL öffnen. Die bisherige Repository-Version bleibt davon unberührt.

Alternativ funktioniert **Deploy from a branch → main → /(root)**.

## Änderungen in Mobile V4

### HDMI und USB: echtes Kabelziehen

- Dreh-Schaltflächen und Klick-zum-Einstecken wurden entfernt.
- Das Kabel wird jetzt gedrückt gehalten und über den Bildschirm zum Anschluss gezogen.
- Beim HDMI-Puzzle scrollt die Werkbank sanft automatisch, sobald der Stecker den oberen oder unteren Rand erreicht.
- Der Stecker schwebt während des Ziehens über der Hardware und bleibt unter dem Finger.
- Zielanschlüsse leuchten beim Annähern auf.
- Loslassen über dem richtigen Port schließt das Puzzle ab; ein einfacher Port-Klick reicht nicht mehr.
- Das gleiche Drag-Prinzip gilt für die USB-Maus.
- Die Maus wurde höher und natürlicher proportioniert; Kabel, Rad, Licht und Seitentaste wurden überarbeitet.

### Spielbalance

- Kaffee sinkt jetzt um **1 Punkt alle 4 Sekunden**.
- Das liegt exakt zwischen dem ursprünglichen 2-Sekunden- und dem zuletzt verwendeten 6-Sekunden-Takt.
- Während Dialogen bleibt der Verbrauch pausiert.
- Neue Aufgaben erscheinen weiterhin variabel nach **3–8 Sekunden**.

### Emojis

- Emojis sind wieder im HUD, bei Stimmungen, ausgewählten Dialogen, Meldungen und Enden vorhanden.
- Die Menge bleibt deutlich unter der ursprünglichen Fassung.
- Eigene Pixel-Icons für Malware und Hardware bleiben erhalten.

## Repository-Struktur

```text
.github/workflows/deploy-pages.yml  GitHub-Pages-Deployment
.nojekyll                           Statische Dateien unverändert ausliefern
index.html                          Fertige selbstständige Website
index.source.html                   Lesbare ungebündelte HTML-Fassung
style.css                           Styles und Hardwaregrafik
characters.js                      Pixelportraits
story.js                           Story und Quests
minigames.js                       Minigames und Kabel-Autoscroll
game.js                            State-Machine und Scheduler
QA.md                              Testprotokoll
REPO-SETUP.md                      Veröffentlichungsschritte
VERSION.txt                        Build-Information
```

## Lokaler Test

`index.html` kann direkt im Browser geöffnet werden. Es sind kein Webserver, kein Paketmanager und kein Build notwendig.
