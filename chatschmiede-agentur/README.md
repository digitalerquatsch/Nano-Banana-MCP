# ChatSchmiede

Landingpage-Konzept für **ChatSchmiede**, eine erfundene Agentur für KI-Chatbots.

`index.html` ist eine eigenständige, statische Single-Page-Website (kein Build-Schritt nötig). Design­richtung angelehnt an [botbuildr.de/s/agentflow](https://botbuildr.de/s/agentflow): dunkles Theme, Blau-Akzent (`#3b82f6`), Sora für Headlines, Inter für Fließtext, Badge-Pills und Glow-Hintergrund.

Inhalt:

- Hero mit Live-Chat-Demo (animierter Beispielverlauf)
- Vertrauensbereich (DSGVO / EU-Hosting)
- Leistungsübersicht (Kundenservice-, Vertriebs-, Messenger- und interne Wissens-Bots)
- 5-stufigem Entwicklungsprozess (Funke → Schmieden → Härten → Zünden → Pflegen)
- Preispaketen (Starter / Business / Enterprise)
- Kurzem "Über uns" und Kontakt-Sektion mit Mailto-CTA

Einfach `index.html` im Browser öffnen, um die Seite anzusehen. Alle Firmen-, Kontakt- und Preisangaben sind Platzhalter für dieses Konzept.

## Logo

Im Ordner `logo/` liegen die Markenassets:

- `mark.svg` – das Icon allein (Blitz/Funke-Motiv in Blau-Grün-Verlauf auf dunkler Kachel), frei skalierbar, z. B. als Favicon oder App-Icon nutzbar.
- `logo-lockup-dark.png` / `logo-lockup-light.png` – Icon + Schriftzug "ChatSchmiede" (Sora) für dunkle bzw. helle Hintergründe, z. B. für Dokumente oder Social-Media-Profile.
- `logo-mark-512.png` – Rasterexport des Icons in 512×512px.

Auf der Website selbst wird das Icon direkt als Inline-SVG eingebunden (scharf bei jeder Auflösung), der Schriftzug läuft live in der Sora-Schriftart mit.
