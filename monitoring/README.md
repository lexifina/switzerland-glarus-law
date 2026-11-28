<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Beobachtung: was gelesen wird und was daraus folgte

[English](README.en.md)

Wie global-law jedes Land beobachtet: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). Diese Seite zeigt dasselbe nur für Glarus: jedes Lesen einer amtlichen Quelle, wann, und was daraus folgte (Vorschriften hinzugefügt, geändert und entfernt). Maschinenlesbar in [data/checks/](../data/checks/) (JSON Lines, Schema `lexifina-check/1`), in `git log` als Commits mit `Kind: check` und Monat für Monat in [checks/](checks/).

**Letzte Prüfung:** 2026-11-28 06:11 UTC, Glarus: Systematische Sammlung (gesetze.gl.ch): 137 Adressen gelesen; 0 hinzugefügt, 1 geändert, 0 entfernt; Änderungen gefunden; 8 nicht veröffentlicht, davon 0 ohne Grund.

## Quellen

| Quelle | Ordner | Wie oft | Letzte erfolgreiche Prüfung | Letztes Ergebnis | Stand |
| --- | --- | --- | --- | --- | --- |
| [Glarus: Systematische Sammlung (gesetze.gl.ch)](https://gesetze.gl.ch/) | `<act>/` | täglich | 2026-11-28 06:11 UTC | Änderungen gefunden | beobachtet |

## Die letzten 30 Tage

| Beginn (UTC) | Quelle | Gelesen | Hinzugefügt | Geändert | Entfernt | Nicht veröffentlicht (ohne Grund) | Ergebnis | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-28 06:08](checks/2026-11.md#ch-lexwork-glarus-20261128t060853z) | lexwork-glarus | 137 | 0 | 1 | 0 | 8 (0) | Änderungen gefunden | — |
| [2026-11-27 06:14](checks/2026-11.md#ch-lexwork-glarus-20261127t061448z) | lexwork-glarus | 188 | 0 | 1 | 0 | 7 (0) | Änderungen gefunden | — |
| [2026-11-26 06:21](checks/2026-11.md#ch-lexwork-glarus-20261126t062118z) | lexwork-glarus | 79 | 0 | 0 | 0 | 5 (0) | keine Änderung | — |
| [2026-11-25 06:45](checks/2026-11.md#ch-lexwork-glarus-20261125t064513z) | lexwork-glarus | 255 | 129 | 0 | 0 | 5 (0) | Änderungen gefunden | [211](https://github.com/lexifina/switzerland-glarus-law/compare/0c2e59621dab...82f3b815ba98) |
| [2026-11-24 14:44](checks/2026-11.md#ch-lexwork-glarus-20261124t144444z) | lexwork-glarus | 178 | 129 | 0 | 0 | 132 (0) | die Prüfung ist fehlgeschlagen | — |
| [2026-11-24 12:06](checks/2026-11.md#ch-lexwork-glarus-20261124t120603z) | lexwork-glarus | 279 | 132 | 1 | 0 | 139 (0) | die Prüfung ist fehlgeschlagen | — |

## Selbst prüfen

```
python tools/checktrail.py                      # die letzte Prüfung jeder Quelle
python tools/checktrail.py --day 2026-11-23     # jede Prüfung eines Tages
python tools/checktrail.py --act <id>           # wann eine Vorschrift gesehen und veröffentlicht wurde
git log --grep='^Kind: check' --format='%ci %s'  # die Prüfungen in der Historie
```

Rechtskraft hat nur die amtliche Verkündung; die Texte hier sind Kopien zum Lesen und Suchen.
