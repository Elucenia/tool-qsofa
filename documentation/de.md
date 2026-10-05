<!-- ELUCENIA technical documentation · qsofa · de · no clinical/professional/rights approval -->

# qSOFA (schneller SOFA)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/qsofa)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Atemfrequenz ≥ 22 Atemzüge/min

`fr`

### Veränderter Bewusstseinszustand (Glasgow \< 15)

`mental`

### Systolischer Druck ≤ 100 mmHg

`pas`

## Fassung der Methode

qSOFA/Sepsis-3/Seymour 2016: AF≥22/systolisch≤100/Bewusstseinsänderung, 0–3; SSC 2021 empfiehlt kein alleiniges Screening

## Dokumentierte Formel

Je ein Punkt: Atemfrequenz ≥ 22/min, veränderter Bewusstseinszustand und systolisch ≤ 100 mmHg. Positiv ab 2 Punkten.

## Grenzen und Population

qSOFA 2016 ist ein Instrument zur Risikobeurteilung bei Erwachsenen mit Infektionsverdacht, keine Diagnose und kein alleiniger Test zum Ausschluss einer Sepsis. Eine niedrige Punktzahl beseitigt den klinischen Verdacht nicht. SSC 2021 empfiehlt, qSOFA nicht als einziges Screening-Instrument zu verwenden; die offiziellen SSC 2026-Leitlinien bevorzugen weiterhin andere Instrumente für das Screening im Krankenhaus. Notfallbeurteilung und Notfallbehandlung dürfen nicht auf die Punktzahl warten. Dieser Schwellenwert für Erwachsene belegt keine Anwendung bei Kindern.

## Referenzen

- [Seymour CW et al. Assessment of clinical criteria for sepsis: for the Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0288)

- [Singer M et al. The Third International Consensus Definitions for Sepsis and Septic Shock (Sepsis-3). JAMA, 2016.](https://doi.org/10.1001/jama.2016.0287)

- [Evans L et al. Surviving sepsis campaign: international guidelines for management of sepsis and septic shock 2021. Intensive Care Med, 2021.](https://doi.org/10.1007/s00134-021-06506-y)

- [SSC adult guidelines2021](https://www.sccm.org/clinical-resources/guidelines/guidelines/surviving-sepsis-guidelines-2021)

- [SSC adult guidelines2026, current official page as observed2026-10-03](https://www.sccm.org/survivingsepsiscampaign/guidelines-and-resources/surviving-sepsis-campaign-adult-guidelines)

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
