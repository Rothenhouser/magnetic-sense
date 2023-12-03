# Schulung 27.11. - 29.11.

Alle Befehle im Anaconda Prompt ausführen - wenn noch nicht vorhanden: https://docs.conda.io/projects/miniconda/en/latest/

## Umgebungsverwaltung

### Umgebung mit Python 3.11 installieren

```cmd
cd [Pfad\zu\diesem\Ordner]
conda env create
```

### Umgebung aktivieren

```cmd
conda activate magsense
```

### Installierte Pakete anzeigen

```
conda list
```

### Zusätzliche Pakete installieren

Namen in `environment.yml` hinzufügen, dann

```
conda env update
```

### Aktivierung in Spyder

Pfad zum Interpreter:

```cmd
where python
```

In Spyder (Version >= 5.5.0):

- Preferences > Python Interpreter > Pfad von oben angeben
- Terminal neu starten

### Python 3.7

Wenn alte Pythonversionen gebraucht werden, muss eventuell eine ältere Version von 
Spyder genutzt werden. In diesem Fall sollte man spyder auch im `environment.yml` 
aufführen und von conda installieren lassen.

Beispiel für Python 3.7:

```
cd spyder-py-37
conda env create  # installert älteres Spyder.exe
conda activate spyder-py-37
```

- Spyder von `...\miniconda3\envs\spyder-py-37\Scripts\spyder.exe` starten
- wie oben Pfad zum Interpreter finden und in Spyder angeben


## Ausführen von Notebooks

```cmd
jupyter notebook
```

## Code Style

### Linting

```
flake8 .
```

### Automatische Formatierung

Jeweils im ganzen Ordner:

```
isort .
black .
```

Die `.flake8` und `.isort.cfg` Konfigurationsdateien stellen sicher, dass die drei Werkzeuge gut zusammenarbeiten.


## Weitere Dokumentation

- Cheatsheets für Pandas und Matplotlib: siehe Ordner
- [Python Tutorial](https://docs.python.org/3/tutorial/index.html)
- [Python Glossar](https://docs.python.org/3/glossary.html#glossary)
- [Pandas Tutorial](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)
- [Pandas Input/Output Reference](https://pandas.pydata.org/pandas-docs/stable/reference/io.html)
- [Matplotlib Gallery](https://matplotlib.org/stable/gallery/index)
- [Seaborn Gallery](https://seaborn.pydata.org/examples/index.html)
- [Codeformatierung]()
- [Plotly (interaktive Visualisierung)](https://plotly.com/python/)
- [Streamlit (Dashboards)](https://streamlit.io/)
- [Jupyter Notebooks](https://jupyter-notebook.readthedocs.io/en/latest/notebook.html)
- [ChatGPT angepasst für Programmierer - geht auch ohne Account](https://www.phind.com/)