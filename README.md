# Analyse von Steam-Reviews zu Grand Theft Auto V

Dieses Projekt untersucht englischsprachige Steam-Nutzerrezensionen zum Videospiel Grand Theft Auto V. Ziel ist es, wiederkehrende Themen in einer großen Menge unstrukturierter Texte automatisch zu erkennen.

## Vorgehensweise

Die Analyse umfasst folgende Schritte:

1. Exploration und Prüfung des Datensatzes
2. Entfernung identischer Review-Texte
3. Textvorverarbeitung
4. Vektorisierung mit Bag-of-Words und TF-IDF
5. Topic Modelling mit LDA und NMF
6. Interpretation und Vergleich der ermittelten Themen

## Verwendete Technologien

- Python
- pandas
- NLTK
- scikit-learn
- matplotlib
- Jupyter Notebook

## Projektstruktur

- `notebooks/` – Durchführung und Dokumentation der Analyse
- `results/` – erzeugte Ergebnistabellen
- `src/` – Platz für wiederverwendbaren Python-Code
- `requirements.txt` – benötigte Python-Pakete

Die Rohdaten und vollständigen Review-Texte sind nicht Bestandteil des öffentlichen Repositorys.

## Installation

Virtuelle Umgebung erstellen:

```powershell
python -m venv .venv
```

Virtuelle Umgebung unter Windows aktivieren:

```powershell
.\.venv\Scripts\Activate.ps1
```

Benötigte Pakete installieren:

```powershell
pip install -r requirements.txt
```

## Zentrale Ergebnisse

Das LDA-Modell identifizierte acht interpretierbare Themen. Dazu gehören unter anderem:

- Modding, Cheating und Bann-Risiken
- Geschäftspraktiken und Preisgestaltung
- Ladezeiten und Ladebildschirme
- technische Probleme und Fehlerbehebung
- Story und Einzelspielermodus
- PC-Portierung, Performance und Grafik

Im Vergleich zum NMF-Modell lieferte LDA stärker inhaltlich abgegrenzte Themen.