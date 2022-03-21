# Analyse der Bordkarten-kontrolldaten des BERs
Ein Studentenprojekt an der<br>
<img src="https://upload.wikimedia.org/wikipedia/de/thumb/9/90/Hochschule_f%C3%BCr_Wirtschaft_und_Recht_Berlin_logo.svg/500px-Hochschule_f%C3%BCr_Wirtschaft_und_Recht_Berlin_logo.svg.png?20090401201013" width="240" align="left" style="display:block;clear:both;"/>
<br><br><br>
Hochschule für Wirtschaft und Recht Berlin<br>
Fachbereich II - Duales Studium Wirtschaft / Technik<br>
<i>Modul: Business Intelligence (WI-201)</i><br><br>


#### Table of Contents
- [Voraussetzungen](#Voraussetzungen)
- [Installationsanleitung](#Installationsanleitung)
- [Struktur des Repositories](#Struktur-des-Repositories)
- [Datenquellen](#Datenquellen)


<a name="Voraussetzungen" /><br>
## Voraussetzungen
- Anaconda mit Python3 (https://www.youtube.com/watch?v=jS4VQx56khc)
- MySQL community server & workbench (https://dev.mysql.com/downloads/)
- Jupyter Notebook (über Anaconda)

<a name="Installationsanleitung" /><br>
## Installationsanleitung
1. Starte MySQL community server
2. Starte Jupyter Notebook über Anaconda (oder alternativ über die Eingabeaufforderung)
3. Clone dieses Repository über Git oder lade es alternativ herunter
4. Erstelle eine Datenbank-Konfigurationsdatei in dem Hauptverzeichnis namens 'dbCredentials.py' mit dem folgenden Inhalt:
   ```
   host = 'localhost'
   username = 'root'
   password = 'myPassword'
   ```
   WICHTIG: Ersetze localhost, root und myPassword mit deinen Zugangsdaten zum MySQL community server.
5. Öffne anschließend das im Hauptverzeichnis enthaltende Jupyter Notebook namens 'BKK-Analyse.ipynb'.
6. Du bist nun bereit, das Jupyter Notebook zu nutzen.

<a name="Struktur-des-Repositories" /><br>
## Struktur des Repositories
- Verzeichnisse
     - data : Enthält die zur Analyse verwendeten Datengrundlagen
     - zwischenstände : Enthält Exporte der Zwischenstände des Jupyter Notebooks als HTML-Dateien
- Dateien
     - BKK-Analyse.ipynb (Jupyter Notebook-Datei) : Das eigentliche Jupyter Notebook und somit der Kern dieses Repositories
     - hilfsfunktionen.py (Python-Datei) : Ein Python-Skript mit Hilfsfunktionen, welche im Jupyter Notebook 'BKK-Analyse.ipynb' verwendet werden
     - readme.md (Readme-Datei) : Diese Datei

<a name="Datenquellen" /><br>
## Datenquellen
- bkk-data.csv : Anonymisierter Auszug aus einem System des BERs
- GDP.csv : https://www.kaggle.com/darknez/gdp-among-world
- airports.csv : https://ourairports.com/data/
- covid19_cases.csv : https://www.kaggle.com/sangeethachinnasamy/corona-new-cases-dataset-for-regression
