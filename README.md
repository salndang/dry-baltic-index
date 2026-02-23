# ⚓ The Ship Index

**Can the cost of shipping predict economic growth before official data does?**

During the Cold War, analysts reportedly monitored pizza deliveries to the Pentagon. When orders spiked late at night, it signalled a crisis was unfolding — often before any public announcement. The data was hiding in plain sight.

This project applies the same principle to the global economy. Instead of pizza boxes, we look at **shipping containers**. The [Baltic Dry Index](https://en.wikipedia.org/wiki/Baltic_Dry_Index) (BDI) tracks the cost of moving raw materials — iron ore, coal, grain — by sea. Because these materials are the physical inputs of industrial production, changes in shipping demand should logically precede changes in economic output.

**The question: does 25 years of data confirm this? And if so, how far ahead does the ocean tell us what the economy is about to do?**

---

## 📊 Key Findings

*Coming soon — currently in Phase 1 (data collection).*

---

## 🔬 Methodology

| Step | Description |
|------|-------------|
| Data Collection | BDI daily data (2000–2025) + UK/US/Eurozone GDP from FRED |
| Exploratory Analysis | Time-series overlays, annotated economic events |
| Lead-Lag Analysis | Cross-correlation at 0–4 quarter lags |
| Granger Causality | Does the BDI statistically "predict" GDP changes? |
| Regression Modelling | Baseline (AR) vs Ship Index augmented model |
| The Pentagon Pizza Test | Did the BDI call each major turning point first? |

---

## 🛠️ Tech Stack

- **Python 3.11+** — pandas, numpy, scipy, statsmodels
- **Visualisation** — matplotlib, plotly
- **Data Sources** — FRED API (GDP), Trading Economics (BDI)
- **Environment** — Jupyter Notebook

---

## 📁 Project Structure

```
dry-baltic-index/
├── README.md
├── requirements.txt
├── notebooks/
│   ├── 01_data_collection.ipynb
│   ├── 02_cleaning_eda.ipynb
│   └── 03_analysis.ipynb
├── data/
│   ├── raw/
│   └── processed/
├── outputs/
└── src/
```

---

## 🚀 How to Run

```bash
git clone https://github.com/salndang/dry-baltic-index.git
cd dry-baltic-index
python -m venv venv
venv\Scripts\activate        # Windows
pip install -r requirements.txt
jupyter notebook
```

You'll need a free [FRED API key](https://fred.stlouisfed.org/docs/api/api_key.html) for GDP data.

---

## 👤 Author

**Salim** — MSc Economics (King's College London), Commercial Reporting & Analytics Lead

*This project is part of an analytics portfolio exploring unconventional economic indicators.*

---

## 📜 License

MIT
