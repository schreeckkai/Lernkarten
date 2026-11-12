# Mathe-Schreck – interaktive Lernkarten

**Mathematische Begriffe, Rechenverfahren und Zusammenhänge aktiv wiederholen.**

➡️ **[Lernkarten-Trainer mit einem Beispielstapel öffnen](https://schreeckkai.github.io/Lernkarten/trainer.html?deck=Q1.1.1)**

Dieses Projekt verbindet thematisch geordnete Mathematik-Lernkarten mit einem browserbasierten Trainer. Die Sammlung befindet sich im Aufbau und wird schrittweise erweitert. Karteninhalte und Trainer sind getrennt: Neue Stapel können als JSON-Dateien ergänzt werden.

## Lernprinzip und Funktionen

- Vorderseite zunächst selbst beantworten, anschließend die Rückseite aufdecken.
- Bearbeitung in Blöcken von bis zu fünf Karten.
- Vor- und Zurückblättern sowie Mischen des aktuellen Blocks.
- Aufdeckbare Lückentexte (Cloze) für entsprechend gestaltete Karten.
- Mathematischer Formelsatz mit KaTeX.
- Anzeige des Bearbeitungsstands innerhalb der aktuellen Sitzung.

Der Trainer unterstützt selbstständige Wiederholung und Selbstkontrolle. Er bewertet Antworten nicht automatisch und ist kein adaptives Spaced-Repetition-System. Die Fortschrittsanzeige ist kein Nachweis des Lernerfolgs.

## Direkt ausprobieren

| Kartensammlung | Einstieg |
|---|---|
| Q1.1.1 | [Trainer öffnen](https://schreeckkai.github.io/Lernkarten/trainer.html?deck=Q1.1.1) |
| Q1.1.4 | [Trainer öffnen](https://schreeckkai.github.io/Lernkarten/trainer.html?deck=Q1.1.4) |
| Periodische Prozesse | [Trainer öffnen](https://schreeckkai.github.io/Lernkarten/trainer.html?deck=E5.1/periodische-prozesse) |
| Ableitung von Sinus und Kosinus | [Trainer öffnen](https://schreeckkai.github.io/Lernkarten/trainer.html?deck=E.5.2/ableitung-sinus-kosinus) |
| Ableitung mit der Kettenregel | [Trainer öffnen](https://schreeckkai.github.io/Lernkarten/trainer.html?deck=E5.3/ableitung-mit-kettenregel) |
| Tag der offenen Tür (Mittelstufe, leicht) | [Trainer öffnen](https://schreeckkai.github.io/Lernkarten/trainer.html?deck=ToT/tag-der-offenen-tuer) |

## Eigene Karten ergänzen

Der Trainer lädt über den URL-Parameter `deck` eine JSON-Datei. Der Parameter enthält den Pfad **ohne** die Endung `.json`.

Beispiel für einen einfachen Stapel:

```json
[
  {
    "front": "Was beschreibt eine Ableitung an einer Stelle?",
    "back": "Die lokale Änderungsrate beziehungsweise die Steigung der Tangente."
  }
]
```

Eine Datei `mein-stapel.json` lässt sich über `trainer.html?deck=mein-stapel` auswählen. Inhalt, mathematische Richtigkeit und Darstellung neuer Karten sollten vor dem Einsatz geprüft werden.

## Technischer Aufbau

- `trainer.html`: Trainer mit dynamischem Laden von JSON-Stapeln.
- `karten.html`: weitere Kartenansicht im Repository.
- JSON-Dateien und Themenordner: getrennt gepflegte Lerninhalte.
- HTML, CSS und JavaScript; KaTeX für Formeln; Veröffentlichung über GitHub Pages.

Für das Laden der Stapel sollte die gehostete Seite oder ein lokaler Webserver verwendet werden; ein bloßer Doppelklick auf die HTML-Datei kann durch Browserbeschränkungen beim Nachladen von JSON scheitern. Externe Bibliotheken und Webschriften benötigen eine Internetverbindung.

## Entwicklungsstand

Trainer und mehrere Kartensammlungen sind vorhanden. Das Repository enthält außerdem Testdateien und Platzhalter; nicht jede Datei ist ein fertig aufbereiteter Lernstapel. Ziel ist eine erweiterbare Sammlung für den Mathematikunterricht, keine bereits vollständige Abdeckung aller Oberstufenthemen.

**Ein Projekt von Kai · [GitHub-Profil](https://github.com/schreeckkai)**