# 🚀 Startup Growth and Funding Trends Analysis

## 📊 Projektübersicht

Dieses Projekt analysiert Wachstums- und Finanzierungsdaten von Startups, um datenbasierte Erkenntnisse über Erfolgsfaktoren, Finanzierungsmuster und Branchentrends zu gewinnen. Im Rahmen einer Gruppenarbeit werden Python-Bibliotheken wie Pandas, NumPy, Matplotlib und Seaborn eingesetzt, um explorative Datenanalysen durchzuführen und aussagekräftige Visualisierungen zu erstellen.

## 🎯 Projektziel

Identifikation von Erfolgsmustern und Entwicklung von Erkenntnissen für:
- Verständnis von Finanzierungstrends im Startup-Ökosystem
- Analyse von Wachstumsmustern erfolgreicher Startups
- Identifikation von Branchentrends und Investitionsschwerpunkten
- Faktoren für erfolgreiche Funding-Runden

## 📁 Projektstruktur

```
DS-Projekt-Online-Retail/
│
├── project.ipynb          # Hauptanalyse-Notebook
├── README.md              # Projektdokumentation
└── data/                  # Datensatz (optional lokal)
```

## 📈 Datensatz

**Quelle:** [Kaggle - Startup Growth and Funding Trends](https://www.kaggle.com/datasets/samayashar/startup-growth-and-funding-trends)

**Beschreibung:**  
Umfassende Daten über Startups, ihre Finanzierungsrunden, Wachstumsmetriken und Unternehmensentwicklung. Der Datensatz enthält Informationen zu:

- **Unternehmensdetails:** Name, Gründungsjahr, Branche, Standort
- **Finanzierung:** Funding-Runden, Investitionsvolumen, Investoren
- **Wachstum:** Mitarbeiterentwicklung, Umsatzwachstum, Bewertung
- **Performance:** Erfolgsmetriken, Exit-Status, Entwicklungsstadium

**Zentrale Variablen:**

| Variable | Typ | Beschreibung |
|----------|-----|--------------||
| Company Name | Text | Name des Startups |
| Founded Year | Numerisch | Gründungsjahr |
| Industry | Kategorial | Branche/Sektor |
| Location | Text | Standort/Region |
| Funding Amount | Numerisch | Erhaltene Finanzierung |
| Number of Employees | Numerisch | Mitarbeiteranzahl |
| Funding Stage | Kategorial | Finanzierungsphase (Seed, Series A/B/C, etc.) |
| Valuation | Numerisch | Unternehmensbewertung |
| Status | Kategorial | Aktueller Status (Operating, Acquired, IPO, Closed) |

## 🔍 Analyseschwerpunkte

### 1. Datenimport & Vorbereitung
- Laden und Inspektion der Startup-Daten
- Data Cleaning (fehlende Werte, Duplikate, Ausreißer)
- Datentyp-Konvertierung und Formatierung

### 2. Explorative Datenanalyse (EDA)
- Deskriptive Statistiken zu Finanzierung und Wachstum
- Finanzierungsanalyse nach Branchen und Regionen
- Zeitreihenanalyse (Gründungstrends, Funding-Wellen)
- Erfolgsanalyse (Exits, IPOs, Bewertungsentwicklung)

### 3. Visualisierungen
- Finanzierungstrends über Zeit
- Top-Branchen und Investitionsschwerpunkte
- Geografische Verteilung von Startups und Funding
- Erfolgsquoten nach Funding-Stage

### 4. Erkenntnisse & Handlungsempfehlungen
- Wichtigste Erfolgsfaktoren
- Branchentrends und Investitionsmuster
- Limitationen der Analyse

## 🛠️ Verwendete Technologien

- **Python 3.x**
- **Jupyter Notebook**
- **Pandas** - Datenmanipulation und -analyse
- **NumPy** - Numerische Berechnungen
- **Matplotlib** - Datenvisualisierung
- **Seaborn** - Statistische Visualisierungen

## 🚀 Installation & Ausführung

### Voraussetzungen
```bash
Python 3.8 oder höher
pip (Python Package Manager)
```

### Setup
1. Repository klonen oder herunterladen
```bash
git clone <repository-url>
cd DS-Projekt-Online-Retail
```

2. Benötigte Packages installieren
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

3. Jupyter Notebook starten
```bash
jupyter notebook project.ipynb
```

## 📊 Analysestruktur im Notebook

1. **Einführung & Datensatz**
   - Problemstellung
   - Datensatzbeschreibung
   - Fragestellungen

2. **Datenimport & Vorbereitung**
   - Daten laden
   - Erste Inspektion
   - Data Cleaning

3. **Explorative Datenanalyse**
   - Finanzierungsanalyse
   - Zeitreihenanalyse
   - Branchenanalyse
   - Erfolgsanalyse

4. **Visualisierungen**
   - Trends und Muster
   - Vergleiche und Rankings

5. **Erkenntnisse & Fazit**
   - Key Findings
   - Handlungsempfehlungen

## 👥 Team

Projektarbeit im Rahmen des Kurses "Introduction to Data Science"

---

**Hinweis:** Der Datensatz stammt von Kaggle und sollte gemäß der Kaggle-Nutzungsbedingungen verwendet werden.