<!-- ELUCENIA technical documentation · abcd2 · de · no clinical/professional/rights approval -->

# ABCD²-Score

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/abcd2)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Alter ≥ 60 Jahre

`idade`

### Blutdruck ≥ 140/90 mmHg bei der Erstbeurteilung

`pa`

### Klinische Manifestation

`clinica`

- `0` — Andere Symptome
- `1` — Sprachstörung ohne Schwäche
- `2` — Einseitige Schwäche

### Symptomdauer

`duracao`

- `0` — \< 10 min
- `1` — 10 bis 59 min
- `2` — ≥ 60 min

### Diabetes

`dm`

## Fassung der Methode

ABCD²/Johnston 2007: Alter/Blutdruck/Klinik/Dauer/Diabetes, Gesamt 0–7

## Dokumentierte Formel

Alter ≥60: 1 · Blutdruck ≥140/90: 1 · C Klinik: einseitige Schwäche 2, Sprache ohne Schwäche 1 · Dauer: ≥60 min 2, 10 bis 59 min 1 · Diabetes 1. Gesamt 0 bis 7.

## Grenzen und Population

Prognosescore nach TIA-Diagnose, vorwiegend für das Schlaganfallrisiko nach 2 Tagen untersucht, mit zusätzlichen Analysen nach 7 und 90 Tagen. Er bestätigt keine TIA-Diagnose. Die in den Originalkohorten beobachteten Wahrscheinlichkeiten sind keine universelle individuelle Vorhersage.

## Referenzen

- [Johnston SC et al. Validation and refinement of scores to predict very early stroke risk after transient ischaemic attack. Lancet, 2007.](https://doi.org/10.1016/S0140-6736(07)60150-0)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
