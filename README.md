[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

Das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de) nutzt GitHub für die Veröffentlichung von Metadatendefinitionen: Vokabulare und Metadatenprofile. Diese Repositorien werden derzeit schrittweise aufgebaut und ergänzt um ein [Wiki](https://github.com/iqb-vocabs/iqb-vocabs.github.io/wiki), um wichtige Konzepte, Tools und Nutzungsszenarien zu erläutern.

# Bildungsstandards 2004/2005
## Primarstufe

* [Deutsch](https://github.com/iqb-vocabs/Bildungsstandard-Deutsch-Primar)
* [Mathematik](https://github.com/iqb-vocabs/Bildungsstandard-Mathe-Primar)

## Sekundarstufe I (HSA/MSA)

* [Deutsch](https://github.com/iqb-vocabs/Bildungsstandard-Deutsch-Sek-I)
* [Mathematik](https://github.com/iqb-vocabs/Bildungsstandard-Mathe-Sek1)
* [Erste Fremdsprache](https://github.com/iqb-vocabs/Bildungsstandard-Fremdsprachen-Sek1)
* Naturwissenschaften: [Chemie](https://github.com/iqb-vocabs/Bildungsstandard-Chemie-Sek1), [Biologie](https://github.com/iqb-vocabs/Bildungsstandard-Biologie-Sek1), [Physik](https://github.com/iqb-vocabs/Bildungsstandard-Physik-Sek1)


# Repositories alphabetisch:
{% for repository in site.github.public_repositories %}{% if repository.archived == false %}

[{{ repository.name }}]({{ repository.html_url }}) {% endif %}{% endfor %}
