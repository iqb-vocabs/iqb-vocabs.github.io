[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

Das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de) nutzt GitHub für die Veröffentlichung von Metadatendefinitionen: Vokabulare und Metadatenprofile.

# Vokabulare
Die Vokabulare des IQB sind in Gruppen angelegt. Jede Gruppe ist in einem separaten Repository bei GitHub als CSV-Dateien (s. jeweils Link 'GitHub') geführt und fasst thematisch verwandte Vokabulare zusammen. In einem Gruppenrepository wird außerdem die Transformation in ttl-Dateien durchgeführt - jeweils für alle Vokabulare einer Gruppe in einem Arbeitsgang. Für diese Umsetzung nutzt das IQB eine eigene (TypeScript-)Programmierung [csv2ttl](https://github.com/iqb-vocabs/csv2ttl#readme).

Jede Gruppe ist bei [SkoHub](https://skohub.io) (s. jeweils Link 'SkoHub') gespiegelt. Dadurch steht automatisch eine ansprechende Präsentation im Html-Format zur Verfügung. Außerdem stellt SkoHub eine Übersetzung eines Vokabulars in eine JSON-Form zur Verfügung, was die Verwendung der Vokabulare in Programmierungen wesentlich erleichtert. Die SkoHub-Darstellung sowie die JSON-Form sind über eine w3id erreichbar, die in der SkoHub-Darstellung angezeigt wird. Die Spiegelung der ttl-Dateien nach SkoHub erfolgt durch einen Webhook bei GitHub, d. h. sie wird automatisch bei Aktualisierung des GitHub-Repositories ausgelöst.

## Veröffentlicht
### Bildungsstandards

|      |                             Anschauen/ Browsen                             |                  Code-Repo                   |
|:--------------|:--------------------------------------------------------------------------:|:--------------------------------------------:|
| Deutsch Sek I 2022 | [Html SkoHub](https://skohub.io/iqb-vocabs/v34/heads/master/index.de.html) | [GitHub](https://github.com/iqb-vocabs/v34)  |
| Fremdsprachen Sek I 2023 | [Html SkoHub](https://skohub.io/iqb-vocabs/v56/heads/master/index.de.html) | [GitHub](https://github.com/iqb-vocabs/v56)  |
| Deutsch Primar 2022 | [Html SkoHub](https://skohub.io/iqb-vocabs/v12/heads/master/index.de.html) | [GitHub](https://github.com/iqb-vocabs/v12)  |
| Mathematik Primar 2022 | [Html SkoHub](https://skohub.io/iqb-vocabs/v10/heads/master/index.de.html) | [GitHub](https://github.com/iqb-vocabs/v10)  |

## In Vorbereitung
* Bildungsstandards Mathematik Sek I 2022

# Lizenz
Für alle Vokabulare des IQB gilt [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

![PictureLoad:CC BY-SA 4.0](https://github.com/iqb-vocabs/iqb-vocabs.github.io/blob/master/assets/licenseCC_BY-SA.png)
