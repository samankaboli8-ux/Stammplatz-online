# stammgast-online

Oeffentliche Seiten des Chatbot-Produkts, ausgeliefert von Netlify aus dem Ordner `public/`
(https://stammgast-online.netlify.app/). Kein Build - was hier liegt, wird so ausgeliefert.

Alles hier schreibt das Projekt "Claude Chatbot Workflow" (`scripts/veroeffentlichung.py`):

- `public/datenschutz/<kunde>/index.html` - die Datenschutzerklaerung eines Kunden,
  aus `render_datenschutz.py --tenant <kunde> ... --veroeffentlichen`
- Startseite, `impressum/`, `datenschutz/index.html` (Datenschutzhinweis dieser Website), `404.html`,
  `robots.txt`, `netlify.toml` - aus `veroeffentlichung.py --einrichten`, Angaben aus `vorlage/legal/anbieter.json`

Nichts von Hand aendern: der naechste Lauf ueberschreibt es. Die Seiten sind absichtlich nicht
fuer Suchmaschinen freigegeben (robots.txt, X-Robots-Tag) - der Link steht im Chat.
