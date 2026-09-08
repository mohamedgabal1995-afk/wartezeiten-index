# Wartezeiten-Index: Terminvorlauf bei deutschen Kfz-Zulassungsstellen

Offener Datensatz (CC BY 4.0) mit dem laufend gemessenen Vorlauf bis zum nächsten regulär buchbaren Termin bei Kfz-Zulassungsbehörden in Deutschland. Die Messung liest mehrmals täglich die öffentlich sichtbare Verfügbarkeit in den offiziellen Terminportalen von 398 Zulassungsbehörden aus. Es werden keine Termine gebucht, blockiert oder reserviert.

**Live-Daten (bei jeder Messung neu erzeugt):** https://zulassungsautomat.de/wartezeiten-index.json  
**Rangliste und Erläuterungen:** https://zulassungsautomat.de/wartezeiten  
**Methodik und Grenzen:** https://zulassungsautomat.de/wartezeiten/methodik

## Stand dieser Momentaufnahme

Erzeugt: 2026-09-08T14:58:33+00:00  
Ämter in der Rangliste: 234 - Median bundesweit: 5 Tage - am schnellsten: Köln - am längsten: Stadt Bremerhaven

Die Datei `wartezeiten-index-2026-09-08.json` ist eine Kopie des Live-Endpunkts vom 8. September 2026. Für aktuelle Werte bitte den Live-Endpunkt verwenden.

## Aufbau der JSON-Datei

- `national`: Kennzahlen bundesweit (Median, Anzahl gemessener Ämter, schnellstes und langsamstes Amt)
- `offices`: ein Eintrag je Zulassungsstelle mit `city`, `bundesland`, `vorlauf_median_days`, `vorlauf_min_days`, `vorlauf_max_days`, `vorlauf_latest_days`, `measurements`, `distinct_days`, `latest_checked_at`, `booking_url`, `termin_system`, `in_ranking`
- `offices_no_slots`: Ämter, bei denen die letzte Prüfung im gesamten Buchungsfenster keinen Termin fand
- `rules`: Aufnahmeregeln (mindestens drei Messungen an verschiedenen Tagen, Referenzleistung Neuzulassung)

## Regeln der Rangliste

Ein Amt kommt erst nach mindestens drei Messungen an verschiedenen Tagen in die Rangliste und nur mit derselben Referenzleistung, der Neuzulassung. Kurzfristig durch Stornierungen frei werdende Termine fließen nicht in die Kennzahlen ein.

## Lizenz und Zitierweise

Daten und Texte stehen unter [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Verwendung, auch redaktionell, ist mit Quellenangabe erlaubt:

> Quelle: Wartezeiten-Index, zulassungsautomat.de (CC BY 4.0)

Zulassungsbehörden, die eine Zahl für falsch halten, können sie gegen den gespeicherten Messbeleg prüfen lassen; Korrekturen werden öffentlich vorgenommen.

## Herausgeber

Zulassungsautomat, Im Werth 11, 46282 Dorsten, info@zulassungsautomat.de. Zulassungsautomat ist ein privater Kfz-Zulassungsdienst und keine Behörde.

---

## English summary

Open dataset (CC BY 4.0) of appointment lead times at German vehicle registration offices (Kfz-Zulassungsstellen), measured several times a day from the official booking portals of 398 authorities. Read-only measurement, no bookings are made. Live endpoint: https://zulassungsautomat.de/wartezeiten-index.json. Method: https://zulassungsautomat.de/wartezeiten/methodik. Attribution: "Source: Wartezeiten-Index, zulassungsautomat.de (CC BY 4.0)".
