[![oereb-handbuch](https://github.com/sogis/oereb-handbuch/actions/workflows/main.yml/badge.svg)](https://github.com/sogis/oereb-handbuch/actions/workflows/main.yml)
# oereb-handbuch
Handbuch OEREB-Kataster Kanton Solothurn

## System Requirements

* Java
* Gradle
* AsciidoctorJ / AsciidoctorPDF

## General usage

Clone this repository:

```
git clone https://github.com/sogis/oereb-handbuch.git $HOME/Projekte/oereb-handbuch
```

HTML-Output:
```
./gradlew asciidoctor
```

PDF-Output:
```
./gradlew asciidoctorPDF
```

## Github pages

https://sogis.github.io/oereb-handbuch/master.html

## Setup Github pages

```
cd /path/to/repo-name
git symbolic-ref HEAD refs/heads/gh-pages
rm .git/index
git clean -fdx
echo "My GitHub Page" > index.html
git add .
git commit -a -m "First pages commit"
git push origin gh-pages
```
