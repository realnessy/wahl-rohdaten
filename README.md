# wahl-rohdaten

Öffentliche Wahldaten für [wahldaten.grok.me](https://wahldaten.grok.me).

Kein Programmcode. Nur die Dateien der Wahlämter und die daraus gebauten JSON-Dateien.

Abruf ausschließlich über jsDelivr:

https://cdn.jsdelivr.net/gh/realnessy/wahl-rohdaten@main/public/v1/index.json

- `public/v1/index.json` — eine Zeile je Wahl
- `public/v1/<wahl>/index.json` — Gesamtergebnis und Wahlkreise, ohne Gemeinden und ohne Konflikte
- `public/v1/<wahl>/conflicts/index.json` — nur Anzahlen
- `public/v1/<wahl>/conflicts/wk-….json.gz` — Konflikte eines Wahlkreises
- `public/v1/<wahl>/wk-….json.gz` — Ergebnisse bis zum Wahlbezirk, ohne Konflikte
- `public/rohdaten/` — unveränderte Dateien der Behörden

Die Zahlen sind nicht neu gerechnet. Sie sind nur anders abgelegt.
