# 🚀 End‑to‑End ML Pipeline with DVC & AWS S3

**This repository demonstrates an end‑to‑end machine learning workflow using DVC for data and model versioning and AWS S3 for remote storage.**  
Build reproducible, traceable, and scalable ML pipelines — from raw data → preprocessing → training → evaluation → model artifacts — all versioned and stored in the cloud.

---

## 🔧 Key Features

- **Data & Model Versioning:** Manage datasets and models efficiently using **DVC**  
- **Cloud Storage:** Store large files safely on **AWS S3**  
- **Reproducible Pipelines:** Define workflow stages in `dvc.yaml` and run with `dvc repro`  
- **Metrics & Logs Tracking:** Monitor experiments with **dvclive**  
- **Lightweight & Collaborative:** Keep Git repos clean while enabling team collaboration  

---

## 🧠 How It Works

1. **Initialize DVC** and link to an AWS S3 bucket for remote storage  
2. Add datasets and models to DVC → stored as lightweight pointer files  
3. Define your **pipeline stages** (`ingest`, `preprocess`, `train`, `evaluate`) in `dvc.yaml`  
4. Run `dvc repro` → automatically executes all stages and rebuilds only what changed  
5. Push datasets & models to S3 using `dvc push`  
6. Collaborate easily and track everything without bloating your Git repository  

> *Reproducible pipelines + cloud storage = smooth ML workflow for teams and individuals.* 🔁

---

## 🚀 Quick Start Commands

```bash
git clone <this-repo>
dvc pull             # Fetch datasets & models from S3
dvc repro            # Reproduce the full pipeline
dvc push             # Push outputs back to S3
```

| Component   | Purpose                                |
| ----------- | -------------------------------------- |
| **Git**     | Version control for code               |
| **DVC**     | Data & model versioning                |
| **AWS S3**  | Remote storage for datasets and models |
| **Python**  | Pipeline scripts and ML logic          |
| **dvclive** | Track metrics, logs & plots            |


## 🧠 Project Overview

This repository is a modern MLOps template demonstrating:
 -DVC for Version Control: Keep large files out of Git, track changes efficiently
 -AWS S3 Remote Storage: Store heavy datasets and models while Git tracks only pointers
 -Automated Pipelines: Rebuild only what changed for reproducible experiments
 -Metrics & Reporting: Use dvclive, logs, and reports to monitor experiments
 -A fully end-to-end, reproducible, and scalable ML workflow ready for real-world projects.
