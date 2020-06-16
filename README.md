# maroph.github.io/openhpi-git
GitHub Projekt für den OpenHPI Git Kurs
[Let's Git - Versionsverwaltung und OpenSource](https://open.hpi.de/courses/git2020)

---

## GitHub Pages Site
Für dieses Projekt verwende ich die optionale 
[GitHub Pages](https://pages.github.com/) Funktionalität. Die zum Projekt gehörige
Webseite ist unter der URL

<https://maroph.github.io/openhpi-git>

zu erreichen. Die Quelle für die GitHub Pages ist das Verzeichnis docs im Branch
master.

## Erzeugen des Content mitr Hilfe des Python Moduls mkdocs
Den Content der Webseite erzeuge ich aus 
[Markdown](https://daringfireball.net/projects/markdown/syntax) Dateien mit Hilfe des
Python Moduls [mkdocs](https://www.mkdocs.org/).

## Installation der fehlenden Python Software
Je nach Distribution sind die Module pip und/oder venv nicht installiert. 
Unter Debian kann man die fehlenden Module folgendermaßen installieren:

    sudo apt install python3-pip
    sudo apt install python3-venv

## Python virtuelles Environment für das Modul mkdocs

    python3 -m venv ./venv
    source ./venv/bin/activate
    python -m pip install --upgrade pip
    python -m pip install --upgrade setuptools
    python -m pip install --upgrade wheel
    python -m pip freeze > ./requirements.txt

## Erzeugen der Dokumente im Verzeichnis docs

    source venv/bin/activate
    mkdocs build

## Speichern (Committen) der Dateien im lokalen Git Repository

    git add .
    git commit -m "my commit message"

## Push in das GitHub Repository

    git push

