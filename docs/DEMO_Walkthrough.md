# Walkthrough Demo: AI‑HRM25 Toolkit v6.0

Questo documento è la guida completa per condurre una demo efficace del Toolkit **AI‑HRM25 v6.0**. Fornisce lo script in **Markdown**, che può essere convertito in PDF o usato come traccia per la presentazione al cliente.

---

## 1. Obiettivi della Demo

- **Dimostrare** l’intera user journey: dalla configurazione iniziale alla generazione automatica di report.
- **Mostrare** l’integrazione tra i template Excel, il Quick‑Start Guide e la CI GitHub Actions.
- **Evidenziare** la facilità di adattamento per PMI/Startup.

---

## 2. Avvio dell’Ambiente

1. **Clonare il repository**:
   ```bash
   git clone https://github.com/Spen-Zosky/AI-HRM25.git
   cd AI-HRM25
   ```
2. **Controllare la struttura**:
   ```bash
   tree /F
   ```
   - `docs/` – documentazione metodologica
   - `templates/` – modelli Excel (vuoti, demo e reali)
   - `visuals/` – mock‑up PowerPoint
   - `.github/workflows/` – CI per esportare KPI
   - `readme_assets/` – output Markdown del KPI Dashboard

---

## 3. Esplorazione dei Modelli Excel

### 3.1 Data Readiness Checklist
- File: `templates/Real_Data_Readiness_Checklist.xlsx`
- Verificare campi: **Data Source**, **Variable**, **Quality**, **Accessibility**, **Owner**, **Notes**

### 3.2 HR DataMap
- File: `templates/Real_HR_DataMap.xlsx`
- Esaminare: **Process**, **Table/File**, **Key Fields**, **Refresh Frequency**, **Sensitivity**

### 3.3 KPI Tracker Master
- File: `templates/Real_KPI_Tracker_Master.xlsx`
- Controllare: **KPI Name**, **Baseline**, **Target**, **Current Value**, **Trend**, **Status**

### 3.4 Insight‑to‑Action Tracker
- File: `templates/Real_Insight_to_Action_Tracker.xlsx`
- Rivedere: **Insight Date**, **Insight Description**, **Root Cause**, **Action Proposed**, **Owner**, **Due Date**, **Status**

### 3.5 Adaptive Governance Tracker
- File: `templates/Real_Adaptive_Governance_Tracker.xlsx`
- Guardare: **Date**, **Decision/Change**, **Area**, **Responsible**, **Compliance Impact**, **Next Review**

### 3.6 AI Retraining Logbook
- File: `templates/Real_AI_Retraining_Logbook.xlsx`
- Verificare: **Model Name**, **Version**, **Retraining Date**, **Dataset Used**, **Accuracy Pre/Post**, **Bias Metric**, **Validated By**

---

## 4. Generazione Automatica del KPI Dashboard

1. **Modifica di test**: aggiornare `Current Value` in `Real_KPI_Tracker_Master.xlsx`.
2. **Commit & Push**:
   ```bash
   git add templates/Real_KPI_Tracker_Master.xlsx
   git commit -m "demo: update KPI value"
   git push origin main
   ```
3. **Attivazione CI**: il workflow **Export KPI Dashboard** rileva la modifica e avvia l’esportazione.
4. **Verifica output**:
   - Aprire `readme_assets/kpi_dashboard.md` su GitHub.
   - Controllare la tabella Markdown con i nuovi valori.

---

## 5. Consultazione della Quick‑Start Guide

1. Aprire `templates/Quick_Start_Guide.docx`.
2. Seguire i passi descritti per replicare in 5 min la configurazione iniziale.

---

## 6. Domande e Discussione

- Come adattare i template ai vostri dati HR specifici?
- Quali metriche volete aggiungere al tracker?
- Discussione su politiche di governance e frequenza di retraining.

---

*Grazie per l’attenzione!*

