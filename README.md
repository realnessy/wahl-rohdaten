# wahl-rohdaten

Öffentliche Wahldaten für [wahldaten.grok.me](https://wahldaten.grok.me).

Kein Programmcode. Nur die Dateien der Wahlämter und die daraus gebauten JSON-Dateien.

Der Zweig `main` enthält die fünf veröffentlichten Wahlen. Weitere Wahlen liegen auf dem Zweig `extra`.

Abruf ausschließlich über jsDelivr:

https://cdn.jsdelivr.net/gh/realnessy/wahl-rohdaten@main/public/v1/index.json

- `public/v1/index.json` — eine Zeile je Wahl
- `public/v1/<wahl>/index.json` — Gesamtergebnis und Wahlkreise, ohne Gemeinden und ohne Konflikte
- `public/v1/<wahl>/conflicts/index.json` — nur Anzahlen
- `public/v1/<wahl>/conflicts/wk-….json.gz` — Konflikte eines Wahlkreises
- `public/v1/<wahl>/wk-….json.gz` — Ergebnisse bis zum Wahlbezirk, ohne Konflikte
- `public/v1/de-bt-2025/gemeinden-01.json.gz` bis `gemeinden-16.json.gz`, und dasselbe unter `de-eu-2024` — Stimmen je achtstelligem Gemeindeschlüssel. Berlin ist leer. Der zwölfstellige Schlüssel in der Wahlkreis- und Kreisdatei bleibt.
- `public/rohdaten/` — unveränderte Dateien der Behörden. Eine Datei über 20 MB liegt als `name;part-1`, `name;part-2` und so weiter. Aneinandergehängt sind das die ursprünglichen Bytes.

Die Zahlen sind nicht neu gerechnet. Sie sind nur anders abgelegt.
