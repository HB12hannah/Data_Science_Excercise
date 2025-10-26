# Copilot Instructions for This Codebase

## Überblick
Dieses Projekt enthält vor allem Jupyter-Notebooks und wissenschaftliche Python-Skripte für Datenanalyse und Visualisierung im Bereich Meteorologie oder Geowissenschaften. Die wichtigsten Arbeitsdateien liegen im Verzeichnis `Python_kurs/`.

## Wichtige Verzeichnisse und Dateien
- `Python_kurs/` – Hauptarbeitsverzeichnis für Notebooks und CSV-Daten
- `requirements_esdsrs.txt` – Enthält alle Python-Abhängigkeiten für die Umgebung

## Entwicklungs- und Arbeitsweise
- Notebooks werden für interaktive Analysen und Visualisierungen genutzt (z.B. mit matplotlib, numpy).
- Externe Daten werden als CSV eingebunden (z.B. `projections.csv`).
- Die Python-Umgebung wird mit `pip install -r requirements_esdsrs.txt` eingerichtet. Fehlende Systembibliotheken (z.B. PROJ für pyproj) müssen ggf. separat installiert werden (z.B. mit Homebrew: `brew install proj`).

## Typische Workflows
- Notebooks direkt ausführen, um Code und Visualisierungen zu testen.
- Für Skripte außerhalb von Notebooks: Code als `.py` speichern und im Terminal mit `python <dateiname>.py` ausführen.
- Bei Import- oder Installationsproblemen: Prüfen, ob alle Abhängigkeiten aus der requirements-Datei installiert sind und ob Systembibliotheken vorhanden sind.

## Besonderheiten und Konventionen
- Es gibt keine speziellen Build- oder Testskripte, keine automatisierten Tests und keine CI/CD-Konfigurationen.
- Die Umgebung ist für wissenschaftliches Arbeiten ausgelegt, nicht für produktive Softwareentwicklung.
- Die requirements-Datei enthält viele Pakete für Datenanalyse, Geodaten und Visualisierung.

## Beispiele
- Ein typisches Notebook importiert numpy, matplotlib, liest Daten aus CSV und erstellt Plots.
- Beispiel für einen Plot:
  ```python
  import matplotlib.pyplot as plt
  import numpy as np
  x = np.linspace(0, 10, 100)
  y = np.sin(x)
  plt.plot(x, y)
  plt.title("Mein erster Plot")
  plt.show()
  ```

## Hinweise für AI Agents
- Fokus auf Datenanalyse, Visualisierung und wissenschaftliche Workflows.
- Prüfe immer, ob Systemabhängigkeiten (wie PROJ) installiert sind, wenn ein Import fehlschlägt.
- Es gibt keine projektspezifischen Test- oder Buildkonventionen.
