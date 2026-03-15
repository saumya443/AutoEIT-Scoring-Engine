# AutoEIT: Automated Scoring Engine for EIT Transcriptions

This repository contains a reproducible Python-based scoring engine designed to evaluate Spanish Elicited Imitation Task (EIT) transcriptions.

## 🚀 Overview
The system automates the scoring process (0-4) using a meaning-based rubric. It employs advanced text normalization (Regex) and sequence alignment algorithms (`difflib.SequenceMatcher`) to compare learner utterances with target prompts.

## 📊 Key Deliverables
* **Reproducible Script:** `AutoEIT_Scoring.ipynb` handles the entire pipeline from cleaning to batch processing.
* **Validation Accuracy:** Achieved ~90% alignment with human-rated benchmarks.
* **Consolidated Output:** `AutoEIT_Submission_Results.csv` contains the final scores for all participants.
* **Data Transparency:** Includes the 3800-series sample files for immediate verification.

## 🔍 Quality Audit
During validation against the `4_vA` dataset, the model identified instances of human rater inconsistency, correctly penalizing transcription errors that were missed by manual rating.

## ⚙️ How to Use
1. Ensure all CSV files and the notebook are in the same directory.
2. Execute all cells in the Jupyter Notebook.
3. The script will generate a final scoring report as a CSV file.
