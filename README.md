# smarte-buchhaltung.online

Website von Smarte Buchhaltung. Online. – Nadine Rau und Mike Trepte, Kassel.

Statische Seite ohne Build-Schritt: HTML, eine CSS-Datei, lokal eingebundene Schriften (keine Verbindung zu Google).

## Aufbau

- `index.html` – Startseite
- `lexware-abc.html` – Lexware Office ABC (A–Z, jeder Buchstabe mit eigenem Anker, z. B. `lexware-abc.html#e`)
- `css/site.css` – alle Styles, Farben und Schriften oben als Variablen
- `fonts/` – Archivo, Source Sans 3, IBM Plex Mono (Lizenzen liegen daneben)
- `img/` – Fotos
- `schnittstellen.html`, `ueber-uns.html`, `impressum.html`, `datenschutz.html` – Unterseiten
- `llms.txt`, `robots.txt`, `sitemap.xml` – für Suchmaschinen und KI-Systeme

## Veröffentlichen

Jeder Push auf `main` wird per GitHub Action auf Strato in den Ordner `smarte_buchhaltung_Webspace_2026/` geladen.
Dafür braucht das Repo drei Secrets: `FTP_SERVER`, `FTP_USERNAME`, `FTP_PASSWORD`.
Größere Änderungen erst auf einem eigenen Branch vorbereiten und ansehen, dann nach `main`.

## Kontaktformular

Sendet per Webhook an Boost.space (wie Leadership Masters), erkennbar am Feld `source = smarte-buchhaltung`.
Auf anderen Adressen als smarte-buchhaltung.online (Vorschau, lokal) wird nichts gesendet.

