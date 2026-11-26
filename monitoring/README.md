<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Beobachtung: was gelesen wird und was daraus folgte

[English](README.en.md)

Wie global-law jedes Land beobachtet: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). Diese Seite zeigt dasselbe nur für Lucerne: jedes Lesen einer amtlichen Quelle, wann, und was daraus folgte (Vorschriften hinzugefügt, geändert und entfernt). Maschinenlesbar in [data/checks/](../data/checks/) (JSON Lines, Schema `lexifina-check/1`), in `git log` als Commits mit `Kind: check` und Monat für Monat in [checks/](checks/).

**Letzte Prüfung:** 2026-11-26 06:33 UTC, Lucerne: Systematische Sammlung (srl.lu.ch): 98 Adressen gelesen; 0 hinzugefügt, 0 geändert, 0 entfernt; keine Änderung; 44 nicht veröffentlicht, davon 0 ohne Grund.

## Quellen

| Quelle | Ordner | Wie oft | Letzte erfolgreiche Prüfung | Letztes Ergebnis | Stand |
| --- | --- | --- | --- | --- | --- |
| [Lucerne: Systematische Sammlung (srl.lu.ch)](https://srl.lu.ch/) | `<act>/` | täglich | 2026-11-26 06:33 UTC | keine Änderung | beobachtet |

## Die letzten 30 Tage

| Beginn (UTC) | Quelle | Gelesen | Hinzugefügt | Geändert | Entfernt | Nicht veröffentlicht (ohne Grund) | Ergebnis | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-26 06:31](checks/2026-11.md#ch-lexwork-lucerne-20261126t063135z) | lexwork-lucerne | 98 | 0 | 0 | 0 | 44 (0) | keine Änderung | — |
| [2026-11-25 07:03](checks/2026-11.md#ch-lexwork-lucerne-20261125t070306z) | lexwork-lucerne | 447 | 127 | 0 | 0 | 44 (0) | Änderungen gefunden | [297](https://github.com/lexifina/switzerland-lucerne-law/compare/2438dbf24230...922d7128acdc) |
| [2026-11-24 14:49](checks/2026-11.md#ch-lexwork-lucerne-20261124t144910z) | lexwork-lucerne | 500 | 161 | 3 | 0 | 164 (0) | die Prüfung ist fehlgeschlagen | — |
| [2026-11-24 12:09](checks/2026-11.md#ch-lexwork-lucerne-20261124t120903z) | lexwork-lucerne | 253 | 161 | 2 | 0 | 165 (0) | die Prüfung ist fehlgeschlagen | — |

## Selbst prüfen

```
python tools/checktrail.py                      # die letzte Prüfung jeder Quelle
python tools/checktrail.py --day 2026-11-23     # jede Prüfung eines Tages
python tools/checktrail.py --act <id>           # wann eine Vorschrift gesehen und veröffentlicht wurde
git log --grep='^Kind: check' --format='%ci %s'  # die Prüfungen in der Historie
```

Rechtskraft hat nur die amtliche Verkündung; die Texte hier sind Kopien zum Lesen und Suchen.
