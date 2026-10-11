# Photovoltaik pro Gemeinde in Deutschland (Marktstammdatenregister, Stand 02.10.2026)

Offene Tabelle mit dem Photovoltaik-Bestand **aller 10.759 Gemeinden** in Deutschland: Anlagen in Betrieb, installierte Leistung (kWp), Balkonkraftwerke, Gebäude- und Freiflächenanlagen, Speicher, Anlagen je 1.000 Einwohner und Zubau Januar–Juli 2026 gegenüber 2025. Es ist dieselbe Datei, aus der **[solarzahlen.de](https://solarzahlen.de)** seine Gemeinde-, Kreis- und Länderseiten erzeugt.

- Gemeindeseiten (Beispiele): [Köln](https://solarzahlen.de/photovoltaik/nordrhein-westfalen/koeln), [Passau](https://solarzahlen.de/photovoltaik/bayern/passau), [Paderborn](https://solarzahlen.de/photovoltaik/nordrhein-westfalen/paderborn)
- Kreisseiten, z. B. [Rottal-Inn](https://solarzahlen.de/photovoltaik/bayern/kreis/rottal-inn)
- Ranglisten: https://solarzahlen.de/rankings · Methodik: https://solarzahlen.de/methodik · Presse und Zitierzeile: https://solarzahlen.de/presse
- Live-Datei (immer aktuell): https://solarzahlen.de/daten/bestand

## Datei

`data/photovoltaik-gemeinden-deutschland-2026-10-02.csv` — UTF-8, Komma als Trenner, Punkt als Dezimalzeichen, 10.759 Zeilen, 31 Spalten. Umgewandelt aus der Live-Datei (dort Semikolon und Dezimalkomma). Die Spalte `url` verweist auf die Gemeindeseite, sofern es eine gibt (717 Gemeinden); alle anderen Gemeinden stecken in ihrer Kreisseite.

| Spalte | Bedeutung |
|---|---|
| `ags` | Amtlicher Gemeindeschlüssel |
| `name`, `bundesland`, `kreis` | Gemeinde, Land, Kreis |
| `einheiten_in_betrieb` | PV-Einheiten in Betrieb |
| `kwp` | Gemeldete Bruttoleistung (Modulleistung) in kWp, Betreiberangabe, Ausreißer nicht gefiltert |
| `balkonkraftwerke`, `gebaeudesolaranlagen`, `freiflaeche`, `sonstige` | Einheiten nach Art |
| `einwohner` | Einwohner (Destatis) |
| `anlagen_je_1000` | Einheiten je 1.000 Einwohner |
| `median_gebaeude_kwp` | Median der Leistung von Gebäudeanlagen |
| `speicher_ja`, `speicher_angabe` | Einheiten mit `SpeicherAmGleichenOrt` = 1 / Einheiten, bei denen das Feld ausgefüllt ist (leere Felder zählen nicht als „kein Speicher“) |
| `neu_okt2025_sep2026` | Neue Einheiten Okt. 2025 – Sep. 2026 |
| `neu_jan_jul_2025`, `neu_jan_jul_2026`, `kwp_jan_jul_*` | Zubau Januar–Juli |
| `*_fenster_*`, `fenster_beginn`, `fenster_ende` | Vergleichsfenster; `*_gleicher_stand` = Vorjahr mit gleichem Meldestand |
| `export_datum`, `quelle` | Datenstand und Exportdatei der Bundesnetzagentur |
| `url` | Gemeindeseite auf solarzahlen.de (leer, wenn keine eigene Seite) |

## Lesehinweise
- Das Marktstammdatenregister erfasst gemeldete Anlagen; Nachmeldungen verändern besonders die letzten Monate. Deshalb gibt es den Vergleich „gleicher Stand“.
- „In Betrieb“ = EinheitBetriebsstatus 35. Stillgelegte Anlagen fehlen, auch im Vorjahresfenster; der Vergleich ist kein vollständiger historischer Zubau.
- Details: https://solarzahlen.de/methodik

## Quelle und Lizenz
Quelle: Marktstammdatenregister, Bundesnetzagentur für Elektrizität, Gas, Telekommunikation, Post und Eisenbahnen, Gesamtdatenexport_20261002_26.2.zip, Stand 02.10.2026. Lizenz der Quelldaten: Datenlizenz Deutschland – Namensnennung – Version 2.0 (dl-de/by-2-0), https://www.govdata.de/dl-de/by-2-0. **Daten geändert:** Aggregation nach Gemeinde, Kreis und Land und Zuordnung veralteter Gemeindeschlüssel.

Lizenz dieser Tabelle: **Datenlizenz Deutschland – Namensnennung – Version 2.0 (dl-de/by-2-0)**, https://www.govdata.de/dl-de/by-2-0 (Text in `LICENSE`).

**Datenquelle: Bundesnetzagentur, Marktstammdatenregister (dl-de/by-2-0).** Quellenvermerk bei Weiterverwendung: „solarzahlen.de. Quelle: Marktstammdatenregister, Bundesnetzagentur (dl-de/by-2-0), Daten geändert“ mit Link auf https://solarzahlen.de.

Unabhängiges Projekt, keine Verbindung zur Bundesnetzagentur.

## Zitieren
Mancera Villa, J. (2026). *Photovoltaik pro Gemeinde in Deutschland, Stand 02.10.2026* [Datensatz]. solarzahlen.de. https://solarzahlen.de/presse

---

**English summary.** Solar PV stock for all 10,759 German municipalities from the Federal Network Agency's Marktstammdatenregister (export of 2 Oct 2026): units in operation, kWp, balcony plants, storage, units per 1,000 inhabitants, and January–July 2026 vs 2025 additions. Municipality pages: https://solarzahlen.de
