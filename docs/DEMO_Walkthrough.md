# Walkthrough Demo: AI‑HRM25 Toolkit v6.0

Questo documento fornisce lo script completo in **Markdown** per la demo del toolkit AI‑HRM25 v6.0, ideale per condividere con il cliente o preparare un PDF.

---

## 1. Introduzione alla Demo

- **Obiettivo**: mostrare l'uso pratico dei template, la generazione automatica del KPI Dashboard e il monitoraggio continuo via tracker.
- **Destinatari**: team HR, IT, Data Science, Sponsor di progetto.

---

## 2. Preparazione dell’Ambiente

1. **Clonazione del repository**
   ```bash
   git clone https://github.com/Spen-Zosky/AI-HRM25.git
   cd AI-HRM25
   ```
2. **Verifica struttura cartelle**
   ```bash
   ls
   ```
   - `docs/` – documentazione metodologica
   - `templates/` – modelli Excel (vuoti, demo e reali)
   - `visuals/` – mock‑up PowerPoint
   - `readme_assets/` – KPI Dashboard in Markdown

---

## 3. Panoramica dei Template Excel Realistici

Aprire ciascun file in Excel e navigare nei fogli:

- **Real_Data_Readiness_Checklist.xlsx**
  - Colonne chiave: `Data Source`, `Variable`, `Quality`, `Owner`, `Notes`.
- **Real_HR_DataMap.xlsx**
  - Campi: `Process`, `Source System`, `Key Fields`, `Refresh Frequency`, `Sensitivity`.
- **Real_KPI_Tracker_Master.xlsx**
  - KPI: `KPI Name`, `Baseline`, `Target`, `Current Value`, `Trend`, `Status`.
- **Real_Insight_to_Action_Tracker.xlsx**
  - Insight Date, Description, Root Cause, Azione proposta, Scadenza, Stato.
- **Real_Adaptive_Governance_Tracker.xlsx**
  - Date, Change, Area, Responsabile, Compliance Impact, Next Review.
- **Real_AI_Retraining_Logbook.xlsx**
  - Versione modello, Data retraining, Accuracy pre/post, Metriche bias, Note.

---

## 4. Generazione Automatica del KPI Dashboard

1. **Modifica** un valore nel file `templates/Real_KPI_Tracker_Master.xlsx` (p.es. `Current Value`).
2. **Salva** e fai:
   ```bash
   git add templates/Real_KPI_Tracker_Master.xlsx
   git commit -m "demo: aggiorna valore KPI"
   git push origin main
   ```
3. Attendere l’esecuzione del workflow **Export KPI Dashboard** su GitHub Actions.
4. Verificare il file `readme_assets/kpi_dashboard.md`: la tabella Markdown con i KPI aggiornati.

---

## 5. Controllo dei Tracker di Governance

1. Aprire `templates/Real_Adaptive_Governance_Tracker.xlsx` per vedere le decisioni di governance.
2. Aprire `templates/Real_AI_Retraining_Logbook.xlsx` per controllare le metriche di performance e bias dei modelli.

---

## 6. Uso della Quick‑Start Guide

1. Aprire `templates/Quick_Start_Guide.docx`.
2. Seguire i passi 1–5 per replicare rapidamente l’ambiente di lavoro.

---

## 7. Conclusione e Prossimi Passi

- **Sintesi**:
  - Setup repo e cartelle.  
  - Esplorazione template realistici.  
  - Generazione automatica del KPI Dashboard.  
  - Verifica dei tracker di insight e governance.
- **Prossimi passi suggeriti**:
  1. Popolare i template con dati aziendali reali.  
  2. Integrare alert su Slack/email per KPI critici.  
  3. Pianificare retraining periodico dei modelli AI.

---

*Fine Walkthrough Demo*

