<!-- ELUCENIA technical documentation · timi-sca · de · no clinical/professional/rights approval -->

# TIMI-Score (ACS ohne ST-Hebung)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/timi-sca)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Alter ≥ 65 Jahre

`idade`

### ≥ 3 Risikofaktoren für koronare Herzkrankheit

`fr`

### Bekannte Koronarstenose ≥ 50 %

`dac`

### ASS-Einnahme in den letzten 7 Tagen

`aas`

### ≥ 2 Angina-pectoris-Episoden in 24 Stunden

`angina`

### ST-Abweichung ≥ 0,5 mm

`st`

### Erhöhter Nekrosemarker

`marc`

## Fassung der Methode

TIMI UA/NSTEMI/Antman 2000: 7 Faktoren 0–1, Gesamt 0–7; ohne TIMI STEMI

## Dokumentierte Formel

Ein Punkt je vorhandenem Merkmal (Gesamt 0 bis 7).

## Grenzen und Population

Diese TIMI-Version wurde bei instabiler Angina und Infarkt ohne ST-Hebung für zusammengesetzte Endpunkte nach 14 Tagen entwickelt und ist nicht die TIMI-Version für STEMI. Die Faktoren haben spezifische zeitliche und klinische Definitionen. Raten historischer Studien bestimmen ohne passende Beurteilung und Leitlinie weder individuelles Risiko noch heutige Behandlung.

## Referenzen

- [Antman EM et al. The TIMI risk score for unstable angina/non–ST elevation MI. JAMA, 2000.](https://doi.org/10.1001/jama.284.7.835)

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

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Nutzen einer frühen invasiven Strategie

| Ergebnisdetails | |
| --- | --- |
| Tod, Myokardinfarkt oder dringende Revaskularisation innerhalb von 14 Tagen | 13,2% |


### 2

Nutzen einer frühen invasiven Strategie

| Ergebnisdetails | |
| --- | --- |
| Tod, Myokardinfarkt oder dringende Revaskularisation innerhalb von 14 Tagen | 26,2% |


### 3

Niedriges Risiko

| Ergebnisdetails | |
| --- | --- |
| Tod, Myokardinfarkt oder dringende Revaskularisation innerhalb von 14 Tagen | 4,7% |

