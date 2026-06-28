# STARK: A Machine Learning Framework for Postoperative Acute Kidney Injury Prediction

## Overview
This repository contains the official code implementation for our study on predicting Postoperative Acute Kidney Injury (PO-AKI). We propose the **STARK framework**, an optimized Stacking ensemble learning model designed to deliver highly accurate, well-calibrated, and clinically actionable predictions.

The framework integrates robust feature engineering, state-of-the-art hyperparameter tuning (Optuna/Bayesian Optimization), and rigorous clinical utility validations, including Fairness Audits and Decision Curve Analysis (DCA).

## 🚀 Key Features
- **Comprehensive Benchmarking**: Head-to-head comparison of traditional ML models against state-of-the-art Large Language Models (LLMs) including DistilGPT2, Qwen-2.5 (1.5B), BioMistral (7B), and Medical Llama-3 (8B).
- **Clinical Utility & Fairness**: Evaluates algorithmic fairness across subgroups (Age, Gender) and visualizes clinical utility through Nature-style Heatmap Matrices and DCA curves.
- **Advanced Validation**: Includes Delong test, Continuous Net Reclassification Improvement (Continuous NRI), Integrated Discrimination Improvement (IDI), and Expected Calibration Error (ECE) calculations via 1000-iteration Bootstrap resampling.
- **Unmeasured Confounding Defense**: Implements E-Value analysis to assess the robustness of specific clinical variables (e.g., intraoperative albumin administration).

## 📂 Repository Structure
- `src/`: Contains core scripts for data preprocessing, model tuning, and ensemble training.
- `notebooks/`: Jupyter notebooks demonstrating the generation of baseline tables, LLM benchmarking, and high-quality figures (Figure 3, Figure 4, Figure 7, Figure 8, Figure S6, Figure S7).
- `rebuttal/`: Specific scripts addressing rigorous peer-review audits (e.g., Missingness Pattern Test, Error Mode Audit).

## 🛠️ Installation
To install the required dependencies, please run:
\`\`\`bash
pip install -r requirements.txt
\`\`\`

## 📊 Quick Start
*(Provide brief instructions on how to run the pipeline, e.g., `python src/model_tuning.py`)*

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
