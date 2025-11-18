# 🚀 Startup Growth & Funding Trends Analysis

## 📊 Projektübersicht

Dieses Data-Science-Projekt analysiert Wachstums- und Finanzierungsdaten von 500 Startups, um **profitable Investments für Investoren zu identifizieren**. Durch Machine Learning und explorative Datenanalyse werden Erfolgsmuster erkannt und ein **Empfehlungsmodell** entwickelt, das datenbasierte Investitionsentscheidungen unterstützt und psychologische Verzerrungen (Biases) reduziert.

## 👥 Gruppenmitglieder

- Engel, Silas
- Nolepa, Mark
- Schneider, Tom
- Trölenberg, Lukas

## 🎯 Geschäftsziel

**Hauptziel:** Große Mengen an Startups ressourceneffizient bewerten und profitable Investments identifizieren.

**Kernfragen:**
- Welche Kennzahlen beeinflussen die Profitabilität für Investoren?
- Wie gut kann ein datenbasiertes Modell die Profitabilität von Startups vorhersagen?
- In welche Startups mit hohem Wachstumspotenzial sollte investiert werden?

**Nutzen:**
- Objektive Bewertung statt Bauchgefühl
- Risikominimierung durch datenbasierte Analyse
- Effiziente Filterung vielversprechender Startups
- Reduktion von Confirmation Bias, Halo-Effekt und Recency Bias

## 📁 Projektstruktur

```
DS-Projekt-Startup-Growth-final/
│
├── Startup.ipynb          # Hauptanalyse-Notebook
├── startup_data.csv       # Datensatz (500 Startups)
├── requirements.txt       # Python-Abhängigkeiten
├── Dockerfile             # Container-Setup
└── README.md              # Projektdokumentation
```

## 📈 Datensatz

**Quelle:** [Kaggle - Startup Growth and Funding Trends](https://www.kaggle.com/datasets/samayashar/startup-growth-and-funding-trends)

**Beschreibung:**  
Umfassende Daten über Startups, ihre Finanzierungsrunden, Wachstumsmetriken und Unternehmensentwicklung. Der Datensatz enthält Informationen zu:

- **Unternehmensdetails:** Name, Gründungsjahr, Branche, Standort
- **Finanzierung:** Funding-Runden, Investitionsvolumen, Investoren
- **Wachstum:** Mitarbeiterentwicklung, Umsatzwachstum, Bewertung
- **Performance:** Erfolgsmetriken, Exit-Status, Entwicklungsstadium

**Zentrale Variablen (500 Startups):**

| Variable | Typ | Beschreibung |
|----------|-----|--------------|
| Startup Name | Text | Name des Startups |
| Industry | Kategorial | Branche (EdTech, FinTech, HealthTech, E-Commerce, CleanTech) |
| Region | Kategorial | Region (North America, Europe, Asia) |
| Funding Amount (M USD) | Numerisch | Investitionssumme in Mio. USD |
| Valuation (M USD) | Numerisch | Unternehmensbewertung in Mio. USD |
| Revenue (M USD) | Numerisch | Umsatz in Mio. USD |
| Number of Employees | Numerisch | Mitarbeiteranzahl |
| Years in Operation | Numerisch | Betriebsjahre |
| Market Share (%) | Numerisch | Marktanteil in Prozent |
| Customer Growth Rate (%) | Numerisch | Kundenwachstumsrate |
| Profitable | Binär | Profitabilität (1 = profitabel, 0 = unprofitabel) |

## 🔍 Analyseschwerpunkte

### Teil 1: Business Understanding & Datenexploration
- **Business Kontext:** Zielsetzung, Geschäftsfragen, Warum Data Science?
- **Explorative Datenanalyse (EDA):** 
  - Vergleich profitabler vs. unprofitabler Startups (Umsatz, Bewertung, Mitarbeiter)
  - Branchenverteilung und regionale Analyse
  - Korrelationsanalyse (Pearson, Spearman)
  - Identifikation von Verzerrungen (Bias-Analyse)
  - Kapitaleffizienz-Analyse (Revenue per Invested Dollar)
  - Marktanteil und Erfolgsfaktoren

### Teil 2: Datenaufbereitung
- **Fehlende Werte:** Identifikation und Behandlung
- **Ausreißer-Behandlung:** IQR-Methode, Clipping-Strategien
- **Feature Engineering:**
  - Neue Metriken: Kapitaleffizienz, Branchenmarktanteil
  - Binäre Features: High Valuation, High Revenue Growth
  - Interaktionseffekte zwischen Features

### Teil 3: Modellierung & Evaluation
- **Modellauswahl:** Logistische Regression für binäre Klassifikation (Profitabel/Unprofitabel)
- **Train-Test-Split:** 80/20-Aufteilung
- **Feature Selection:** Relevante Prädiktoren identifizieren
- **Evaluation:**
  - Confusion Matrix (TP, FP, TN, FN)
  - Accuracy, Precision, Recall, F1-Score
  - Fokus auf Risikominimierung (False Positives reduzieren)
- **Hyperparameter-Tuning:** Threshold-Optimierung

### Teil 4: Erkenntnisse & Handlungsempfehlungen
- **Konkrete Investitionsempfehlungen**
- **Modellgrenzen und Limitationen**
- **Kritische Fragen:** Datenqualität, Repräsentativität, Kausalität
- **Nächste Schritte:** Erweiterungsmöglichkeiten (größere Datensätze, Ensemble-Methoden, Survival Analysis)

## 🛠️ Verwendete Technologien

### Core Libraries
- **Python 3.13**
- **Jupyter Notebook / VS Code**

### Data Processing & Analysis
- **Pandas** - Datenmanipulation und -analyse
- **NumPy** - Numerische Berechnungen
- **SciPy** - Statistische Tests und wissenschaftliche Berechnungen

### Visualization
- **Matplotlib** - Basis-Visualisierungen
- **Seaborn** - Statistische Plots und Heatmaps
- **Plotly Express** - Interaktive Visualisierungen (Bubble Charts, 3D-Plots)

### Machine Learning
- **Scikit-learn** - Logistische Regression, Train-Test-Split, Metriken
- **IPython.display** - Notebook-Darstellung

## 🚀 Installation & Ausführung

### Voraussetzungen
- **Python 3.8+** (empfohlen: 3.13)
- **pip** (Python Package Manager)
- **Jupyter Notebook** oder **VS Code mit Python Extension**

### Setup

#### Option 1: Automatische Installation (empfohlen)
Das Notebook installiert automatisch alle benötigten Module beim ersten Ausführen der Installationszelle.

1. **Repository klonen oder herunterladen**
```bash
git clone <repository-url>
cd DS-Projekt-Startup-Growth-final
```

2. **Notebook öffnen**
```bash
jupyter notebook StartUp.ipynb
# oder mit VS Code
code StartUp.ipynb
```

3. **Erste Zellen ausführen** - Die Installation läuft automatisch

#### Option 2: Manuelle Installation
```bash
pip install -r requirements.txt
```

Oder einzeln:
```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn scipy ipython
```

### Docker Setup (Optional)
```bash
docker build -t startup-analysis .
docker run -p 8888:8888 startup-analysis
```

## 📊 Notebook-Struktur (StartUp.ipynb)

### Teil 0: Setup
- Automatische Modulinstallation
- Import aller benötigten Libraries
- Laden des Datensatzes (`startup_data.csv`)

### Teil 1: Business Understanding & Datenexploration
1. **Business Kontext**
   - Geschäftsproblem und Zielsetzung
   - Warum Data Science für Startup-Investments?
   
2. **Explorative Datenanalyse (EDA)**
   - **Graph V1:** Umsatzvergleich profitabel vs. unprofitabel
   - **Graph V2:** Verteilung der Startups nach Industrie
   - **Graph V3:** Regionale Verteilung
   - **Graph V4:** Bewertung vs. Investitionssumme (Bubble Chart)
   - **Graph V5:** 3D-Visualisierung (Marktanteil, Umsatz, Bewertung)
   - **Graph V6:** Kapitaleffizienz-Analyse (Top 30 nach Revenue/Investment)
   - **Korrelationsmatrix:** Pearson & Spearman
   - **Bias-Analyse:** Identifikation systematischer Verzerrungen
   - **Marktanteil-Analyse:** Korrelation mit Erfolgsmetriken

### Teil 2: Datenaufbereitung
1. **Fehlende Werte behandeln**
2. **Ausreißer-Erkennung und -Behandlung** (IQR-Methode)
3. **Feature Engineering:**
   - Kapitaleffizienz berechnen
   - Branchenmarktanteil
   - Binäre High-Performance-Features

### Teil 3: Modellierung
1. **Modellauswahl:** Logistische Regression
2. **Train-Test-Split** (80/20)
3. **Feature Selection**
4. **Model Training**
5. **Evaluation:**
   - Confusion Matrix
   - Precision, Recall, F1-Score
   - Threshold-Optimierung
6. **Top-Startup-Empfehlungen** (nach Wahrscheinlichkeit sortiert)

### Teil 4: Insights & Next Steps
1. **Konkrete Investitionsempfehlungen**
2. **Modellgrenzen und Limitationen**
3. **Kritische Reflexion:**
   - Datenqualität
   - Repräsentativität
   - Kausalität vs. Korrelation
4. **Weiterführende Analysemöglichkeiten:**
   - Größere Datensätze
   - Ensemble-Methoden
   - Survival Analysis
   - Kausalinferenz

## 📈 Wichtigste Erkenntnisse

### Datenanalyse-Insights
- **Branchenverteilung:** EdTech und FinTech dominieren den Datensatz
- **Regionale Unterschiede:** North America führt bei Investitionsvolumen
- **Korrelationen:** Starker Zusammenhang zwischen Funding Amount und Valuation (r=0.8)
- **Kapitaleffizienz:** Große Varianz zwischen Branchen und Startups
- **Marktanteil:** Positiver, aber schwacher Zusammenhang mit Profitabilität

### Modell-Performance
- **Accuracy:** ~60%
- **Precision:** Fokus auf Risikominimierung (False Positives reduzieren)
- **Recall:** ~35% (Trade-off zugunsten höherer Precision)
- **Ergebnis:** Modell schlägt Zufallsrate (50%) und reduziert Investitionsrisiko

### Empfehlungen
1. **Nicht blind investieren** - Top 10-20 Startups genauer prüfen
2. **Portfolio-Diversifikation** - In mehrere vorgeschlagene Startups investieren
3. **Qualitative Faktoren beachten** - Team, Vision, Produkt-Market-Fit
4. **Datenbasiert entscheiden** - Bauchgefühl durch objektive Metriken ergänzen

## 🚧 Limitationen

- **Kleiner Datensatz:** Nur 500 Startups
- **Survivorship Bias:** Gescheiterte Startups möglicherweise unterrepräsentiert
- **Fehlende Features:** Gründerteam-Erfahrung, Netzwerkeffekte, Marktdynamiken
- **Zeitliche Effekte:** Keine Normalisierung nach Unternehmensalter/Gründungsjahr
- **Kausalität unklar:** Korrelation ≠ Kausalität

## 🔮 Zukünftige Erweiterungen

- Größerer Datensatz (5.000-10.000 Startups)
- Ensemble-Methoden (Random Forest, Gradient Boosting)
- Survival Analysis (Zeit bis Profitabilität)
- NLP-Analyse von Pitch Decks und Business Plans
- Einbindung makroökonomischer Variablen
- Real-Time-Daten und API-Integration

## 📝 Lizenz & Datenquelle

**Datensatz:** [Startup Growth & Funding Trends - Kaggle](https://www.kaggle.com/datasets/samayashar/startup-growth-and-funding-trends)

Der Datensatz wird gemäß der Kaggle-Nutzungsbedingungen verwendet. Dieses Projekt dient ausschließlich akademischen und Lernzwecken.

---

**Projektarbeit im Rahmen des Kurses "Introduction to Data Science"**  

© 2025 | Tom Scheider, Mark Nolepa, Lukas Trölenberg, Silas Engel
