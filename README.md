# NeuroDriftOn

Hybrid AI system for early health risk detection using personal baseline modeling and temporal anomaly intelligence.

---

## Overview

NeuroDriftOn is an end-to-end machine learning system designed to identify early signals of neurodevelopmental and autoimmune conditions from behavioral and physiological time-series data.

The system departs from traditional population-based approaches by learning an individual's baseline state and detecting deviations over time. It integrates temporal sequence modeling with drift-aware anomaly detection to surface subtle, progressive changes in health patterns.

---

## Core Approach

NeuroDriftOn combines three complementary signals:

- **Personal Baseline Deviation**  
  Models an individual’s normal physiological state and measures deviation from that baseline.

- **Temporal Sequence Modeling**  
  Uses a transformer-based architecture to learn sequential patterns and detect anomalies via reconstruction error.

- **Drift Trend Analysis**  
  Captures gradual changes in behavior and physiology over time.

These components are fused into a unified risk score for robust anomaly detection.

---

## System Architecture
```

Data Ingestion
↓
Preprocessing (cleaning, alignment, normalization)
↓
Personal Baseline Model
↓
Temporal Transformer
↓
Drift Detection Engine
↓
Hybrid Risk Scoring
↓
API / Dashboard

```
---

## Project Structure
```bash

neurodrifton/
│
├── data/ # synthetic and processed datasets
├── src/
│ ├── preprocessing/ # data cleaning and alignment
│ ├── baseline/ # personal baseline modeling
│ ├── model/ # transformer-based sequence model
│ ├── anomaly/ # drift detection and scoring
│ ├── pipeline/ # end-to-end orchestration
│ ├── api/ # inference service
│ └── dashboard/ # visualization layer
│
├── experiments/ # training and evaluation
├── models/ # trained model artifacts

```
---

## Setup

```bash
git clone https://github.com/yourusername/neurodrifton.git
cd neurodrifton

pip install -r requirements.txt
Execution

Run the full pipeline:

python run_all.py

Launch dashboard:

streamlit run src/dashboard/app.py
Evaluation

The system is evaluated using:

ROC-AUC (anomaly detection performance)
Precision / Recall
Early Detection Lead Time (temporal advantage in identifying onset)
Applications
Early neurodevelopmental signal detection
Autoimmune condition monitoring
Continuous health risk assessment
Personalized digital health systems
