[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de) nutzt GitHub für die Veröffentlichung von Metadatendefinitionen: Vokabulare und Metadatenprofile. Außerdem sind hier Module und Komponenten veröffentlicht, die die Nutzung der Metadatendefinitionen in Webanwendungen unterstützen (TypeScript, Angular) oder der Validierung und Dokumentation der Metadatendefinitionen dienen. 

# Metadatenprofile

Für Datenobjekte speichert das IQB Metadaten. Welche Daten dies genau sein sollen, wird in sog. Metadatenprofilen definiert. Bei GitHub sind diese Profile als JSON-Dateien gespeichert, jeweils mehrere thematisch verwandte Profile zusammen in einem Repository, dem sog. Profil-Store.

Folgende Profile sind veröffentlicht:

* [IQB Deutsch Primar](https://github.com/iqb-vocabs/p12/tree/master/docs#readme) (Aufgaben, Items)
* [IQB Mathematik Primar](https://github.com/iqb-vocabs/p11/tree/master/docs#readme) (Aufgaben, Items)
* [IQB Französisch Sekundarstufe I](https://github.com/iqb-vocabs/p52/tree/master/docs#readme) (Aufgaben, Items)
* [IQB Englisch Sekundarstufe I](https://github.com/iqb-vocabs/p53/tree/master/docs#readme) (Aufgaben, Items)
* [IQB TB-Fragebögen](https://github.com/iqb-vocabs/p60/tree/master/docs#readme) (Aufgaben, Items)
* [VerbundFDB-Metadatenprofil: Kernset Bildungsforschung](https://iqb-vocabs.github.io/p80/) (Aufgaben)
  

Das IQB führt ein Register von Metadatenprofilen, um es Anwendungen zu erleichtern, passende Profile bestimmten Objekten zuzuweisen. Das [Register finden Sie hier](https://github.com/iqb-vocabs/profile-registry).

Typdefinitionen für Metadatenprofile und Metadaten-Werte [finden Sie hier](https://github.com/iqb-vocabs/metadata#readme) (TypeScript).

# Vokabulare
Die Vokabulare des IQB sind in Gruppen angelegt. Jede Gruppe ist in einem separaten Repository bei GitHub als CSV-Dateien (s. jeweils Link 'GitHub') geführt und fasst thematisch verwandte Vokabulare zusammen. In einem Gruppenrepository wird außerdem die Transformation in ttl-Dateien durchgeführt - jeweils für alle Vokabulare einer Gruppe in einem Arbeitsgang. Für diese Umsetzung nutzt das IQB eine eigene (TypeScript-)Programmierung [csv2ttl](https://github.com/iqb-vocabs/csv2ttl#readme).

Jede Gruppe ist bei [SkoHub](https://skohub.io) (s. jeweils Link 'SkoHub') gespiegelt. Dadurch steht automatisch eine ansprechende Präsentation im Html-Format zur Verfügung. Außerdem stellt SkoHub eine Übersetzung eines Vokabulars in eine [JSON-Form](#json-abruf-von-vokabularen) zur Verfügung, was die Verwendung der Vokabulare in Programmierungen wesentlich erleichtert. Die SkoHub-Darstellung sowie die JSON-Form sind über eine w3id erreichbar, die in der SkoHub-Darstellung angezeigt wird. Die Spiegelung der ttl-Dateien nach SkoHub erfolgt durch einen Webhook bei GitHub, d. h. sie wird automatisch bei Aktualisierung des GitHub-Repositories ausgelöst.

## Veröffentlichte Vokabulare

### Bildungsstandards

* [Deutsch Sek I 2022](https://skohub.io/iqb-vocabs/v34/heads/master/index.de.html)
* [Fremdsprachen Sek I 2023](https://skohub.io/iqb-vocabs/v56/heads/master/index.de.html)
* [Deutsch Primar 2022](https://skohub.io/iqb-vocabs/v12/heads/master/index.de.html)
* [Mathematik Primar 2022](https://skohub.io/iqb-vocabs/v10/heads/master/index.de.html)
* [Mathematik Sek I 2022](https://skohub.io/iqb-vocabs/v51/heads/master/index.de.html)

### Aufgaben und Items allgemein

* [Itemformate](https://skohub.io/iqb-vocabs/v27/heads/master/index.de.html)
* [Textvorgabe Fremdsprachen](https://skohub.io/iqb-vocabs/v25/heads/master/index.de.html)
* [Allgemeine Kompetenzen Fremdsprachen](https://skohub.io/iqb-vocabs/v26/heads/master/index.de.html)
* [Textvorgabe Deutsch](https://skohub.io/iqb-vocabs/v28/heads/master/index.de.html)
* [IQB Fragebögen](https://skohub.io/iqb-vocabs/v37/heads/master/index.de.html)

### Forschungsdaten

* [Konstrukte](https://skohub.io/iqb-vocabs/v87/heads/master/index.de.html)
* [VerbundFDB: Kontrolliertes Vokabular](https://skohub.io/iqb-vocabs/v85/heads/master/index.de.html)

## JSON-Abruf von Vokabularen

Für die Referenzierung eines Vokabular-Eintrages in einem Datenobjekt muss das Vokabular über einen persistenten - also dauerhaften - Identifier verfügen. Wir benutzen perma-id bei [w3id.org](https://w3id.org/). Für die Auflösung beispielsweise des Eintrags
```
Vokabular: Bildungsstandards Fremdsprachen Sek I 2023 - Anforderungsbereiche
Vokabulareintrag: Anforderungsbereich I
```

ist die permanente URL
```
https://w3id.org/iqb/v51/a1/c6u
```
zu verwenden.

Für den Abruf eines kompletten Vokabulars im handlichen JSON-Format muss die URL des Vokabulars um `/index.json` erweitert werden:
```
https://w3id.org/iqb/v51/a1/index.json
```
