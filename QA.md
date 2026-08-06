# Mobile-V4-Abnahme

## Kabelinteraktion

- [x] HDMI funktioniert ausschließlich durch Ziehen und Loslassen
- [x] USB funktioniert ausschließlich durch Ziehen und Loslassen
- [x] kein vorheriges Drehen mehr erforderlich
- [x] Port-Klick allein löst die Aufgabe nicht
- [x] schwebender Stecker bleibt während des Ziehens unter dem Finger
- [x] sanfter Autoscroll am oberen und unteren Rand
- [x] HDMI-Autoscroll bringt die GPU-Anschlüsse in den sichtbaren Bereich
- [x] Annäherungs-Highlight an Anschlüssen
- [x] falsche Ports erzeugen weiterhin passende Rückmeldung
- [x] Mausgrafik neu proportioniert

## Balance und Ablauf

- [x] Kaffeeabzug: 1 Punkt je 4 Sekunden
- [x] kein Kaffeeabzug während Dialogen
- [x] nächste Aufgabe nach 3–8 Sekunden
- [x] maximal gemessene Ticket-Wartezeit: 8,34 Sekunden
- [x] Router-Sequenz startet weiterhin erst nach explizitem Touch

## Funktionstests

- selbstständige `index.html` allein in leerem Ordner gestartet
- 0 zusätzliche Netzwerk- oder Dateianfragen
- Touch-Start erfolgreich
- alle 10 Minigames plus DRUCKO 5000 abgeschlossen
- HDMI-Drag mit echtem Edge-Autoscroll geprüft
- USB-Drag geprüft
- Kaffee-Hold-Geste geprüft
- Story-Scheduler, Pflicht-Events, Enden und Restart geprüft
- keine Konsolenfehler

## Viewports

- 320 × 568
- 360 × 740 bei Device-Pixel-Ratio 3
- 390 × 844
- 412 × 915

## Visuelle Einzelprüfung

Start, Board, HDMI-Start, HDMI während Autoscroll, USB-Start, USB während Drag und Endscreen wurden einzeln geprüft. Zusätzlich wurden alle 17 Hauptzustände ohne Konsolenfehler neu gerendert.
