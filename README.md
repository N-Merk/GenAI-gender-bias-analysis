# Auditing Gender Bias in AI-Generated Content

This project investigates how gender is represented across occupations in AI-generated text and images. It combines data preparation, AI-assisted translation, rule-based gender classification, and statistical analysis to compare representations across datasets and verb categories.

## Project Overview

The project uses U.S. employment data from the [Bureau of Labor Statistics](https://www.bls.gov/cps/cps_aa2023.htm#charemp) as a reference for occupational gender distributions. It generates and analyzes text and image datasets involving a range of occupations, then compares the gender representations found in the generated content.

Google Gemini was used to translate text datasets and generate images. The analysis includes gender classification based on German articles and occupation-name endings, as well as visual comparisons using histograms and heatmaps.

## Repository Structure

- `data/` — Raw, processed, and AI-generated datasets, including generated images.
- `notebooks/` — Jupyter notebooks for data generation, preparation, and statistical analysis.
- `src/` — Python functions for data preparation, translation, gender classification, and visualization.
- `plots/` — Generated charts and figures.
- `tests/` — Project tests.
- `main.py` — Main Python entry point.

## Methods

The analysis workflow includes:

1. Preparing occupation and verb datasets.
2. Generating and translating text with the Google Gemini API.
3. Classifying the grammatical gender of occupation references in translated text.
4. Comparing gender patterns across datasets, occupations, and verb categories.
5. Visualizing results with histograms and heatmaps.
6. Comparing AI-generated image datasets with reference employment data.

## ---- German Version ---------------------------------------------------------------------------

# Untersuchung von Geschlechterverzerrungen in KI-generierten Inhalten

Dieses Projekt untersucht, wie Geschlecht in KI-generierten Texten und Bildern zu verschiedenen Berufen dargestellt wird. Es verbindet Datenaufbereitung, KI-gestützte Übersetzung, regelbasierte Geschlechtsklassifikation und statistische Analysen, um Darstellungen in unterschiedlichen Datensätzen und Verbkategorien zu vergleichen.

## Projektüberblick

Als Referenz für die Geschlechterverteilung in verschiedenen Berufen dienen US-amerikanische Beschäftigungsdaten des [Bureau of Labor Statistics](https://www.bls.gov/cps/cps_aa2023.htm#charemp). Das Projekt erstellt und analysiert Text- und Bilddatensätze zu verschiedenen Berufen und vergleicht anschließend die darin vorkommenden Geschlechterdarstellungen.

Google Gemini wurde verwendet, um Textdatensätze zu übersetzen und Bilder zu generieren. Die Analyse umfasst eine Geschlechtsklassifikation anhand deutscher Artikel und typischer Berufsbezeichnungen sowie visuelle Vergleiche mit Histogrammen und Heatmaps.

## Repository-Struktur

- `data/` — Rohdaten, aufbereitete und KI-generierte Datensätze einschließlich generierter Bilder.
- `notebooks/` — Jupyter-Notebooks zur Datengenerierung, Datenaufbereitung und statistischen Analyse.
- `src/` — Python-Funktionen zur Datenaufbereitung, Übersetzung, Geschlechtsklassifikation und Visualisierung.
- `plots/` — Erstellte Diagramme und Grafiken.
- `tests/` — Tests für das Projekt.
- `main.py` — Einstiegspunkt für die Ausführung des Python-Codes
  
## Methoden

Der Analyseablauf umfasst:

1. Aufbereitung der Berufs- und Verbdatensätze.
2. Generierung und Übersetzung von Texten mit der Google Gemini API.
3. Klassifikation des grammatischen Geschlechts von Berufsbezeichnungen in den übersetzten Texten.
4. Vergleich der Geschlechterdarstellungen zwischen Datensätzen, Berufen und Verbkategorien.
5. Visualisierung der Ergebnisse mit Histogrammen und Heatmaps.
6. Vergleich der KI-generierten Bilddatensätze mit den Referenzdaten zur Beschäftigung.



Um den gesamten Code inklusive der Übersetzungen via der Gemini-API auszuführen ist eine personal.env Datei im Hauptordner zu erstellen in welcher der Gemini API Key zu speichern ist indem mit "GEMINI_API_KEY = <Personal Gemini API-KEY>". 
