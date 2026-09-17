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

- `mark.svg` – das Icon allein (Amboss-Motiv in Blau-Grün-Verlauf auf dunkler Kachel), frei skalierbar, z. B. als Favicon oder App-Icon nutzbar.
- `logo-lockup-dark.png` / `logo-lockup-light.png` – Icon + Schriftzug "ChatSchmiede" (Sora) für dunkle bzw. helle Hintergründe, z. B. für Dokumente oder Social-Media-Profile.
- `logo-mark-512.png` – Rasterexport des Icons in 512×512px.
- `favicon.ico` – Multi-Size-Favicon (16/32/48px) für Browser-Tabs.
- `favicon-16.png`, `favicon-32.png` – einzelne PNG-Favicon-Größen.
- `apple-touch-icon.png` (180×180) – Homescreen-Icon für iOS/Safari.
- `icon-192.png`, `icon-512.png` – App-/Android-Icon-Größen (z. B. für ein Web-App-Manifest).
- `social-card.png` (1200×630) – Vorschaubild für Link-Previews (Open Graph / Twitter Card).

Auf der Website selbst wird das Icon direkt als Inline-SVG eingebunden (scharf bei jeder Auflösung), der Schriftzug läuft live in der Sora-Schriftart mit. `index.html` verlinkt zusätzlich `favicon.ico`, die Apple-Touch-Icon- und die Social-Card-Datei im Kopfbereich.

## SEO / Google-Auffindbarkeit

`index.html` enthält bereits die technische Grundausstattung, damit Google die Seite sauber lesen und anzeigen kann:

- Aussagekräftiger `<title>` und `<meta name="description">` mit Kernbegriffen ("KI-Chatbot-Agentur")
- `og:*` / `twitter:card`-Tags für gute Link-Vorschauen (nutzen `social-card.png`)
- `<link rel="canonical">` gegen doppelten Content
- JSON-LD-Strukturdaten (`ProfessionalService`) für Rich-Snippets in der Google-Suche
- `robots.txt` und `sitemap.xml` im Projekt-Root

**Vor dem Live-Gang ersetzen:** `www.chatschmiede.de` ist ein Platzhalter – vor Veröffentlichung in `index.html` (canonical, JSON-LD, og:image/og:url), `robots.txt` und `sitemap.xml` durch die echte Domain ersetzen.

Das allein reicht aber nicht, um bei Google *gefunden* zu werden – das ist nur die technische Basis. Was zusätzlich nötig ist: Domain bei der Google Search Console anmelden und Sitemap einreichen, ein Google-Unternehmensprofil (Google Maps/Local) anlegen und pflegen, Inhalte mit den Suchbegriffen der Zielgruppe ergänzen (z. B. eigene Seiten/Blogartikel zu "KI-Chatbot für [Branche]"), sowie Backlinks von anderen Websites (Verzeichnisse, Partner, Presse) aufbauen. SEO wirkt erfahrungsgemäß erst nach einigen Wochen bis Monaten; für sofortige Sichtbarkeit eignet sich ergänzend Google Ads.
