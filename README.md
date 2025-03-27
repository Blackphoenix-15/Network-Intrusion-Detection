# Network Intrusion Detection System

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Machine learning pipeline for detecting network intrusions using the UNSW-NB15 dataset.

## Features
- Data preprocessing (cleaning, encoding, scaling)
- Feature importance analysis
- Four ML models: Random Forest, SVM, XGBoost, LightGBM
- Threshold optimization for security-critical scenarios
- Comprehensive evaluation (accuracy, precision, recall, AUC)

## Dataset
[UNSW-NB15 Dataset](https://www.kaggle.com/datasets/mrwellsdavid/unsw-nb15)  
- Training set: 175,341 samples
- Testing set: 82,332 samples  
- 45 features including:
  - Network flow statistics (`dur`, `sbytes`, `dbytes`)
  - Protocol/service information (`proto`, `service`)

## Installation
```bash
git clone https://github.com/Blackphoenix-15/network-intrusion-detection.git
cd network-intrusion-detection
pip install -r requirements.txt

Usage
Preprocessing data:

python

python preprocess.py --input data/UNSW_NB15_training-set.csv
Train models:

python

python train.py --model xgboost
Evaluate performance:

python

python evaluate.py --threshold 0.1234
Results Summary
Model	Accuracy	Precision	Recall	AUC
XGBoost	90.0%	99.0%	86.0%	0.985
Random Forest	90.0%	99.0%	86.0%	0.982
LightGBM	90.0%	99.0%	86.0%	0.986
SVM	91.3%	90.5%	91.0%	0.962
Directory Structure

├── data/                   # Raw dataset files
├── notebooks/              # Jupyter notebooks for analysis
├── src/
│   ├── preprocess.py       # Data cleaning pipeline
│   ├── train.py            # Model training
│   └── evaluate.py         # Performance evaluation
├── reports/                # Generated visualizations
├── requirements.txt        # Python dependencies
└── README.md
License
MIT License - See LICENSE for details.



---

### Key Features of This Setup:
1. **Concise Metadata**: Badges for Python version and license
2. **Modular Structure**: Clear separation of preprocessing/training/evaluation
3. **Reproducibility**: `requirements.txt` for dependencies
4. **Visual Results**: Table summarizing key metrics
5. **Actionable Commands**: Ready-to-run example scripts

To implement:
1. Create a new GitHub repository
2. Add this README.md
3. Structure your code files according to the directory layout
4. Include a `requirements.txt` with your Python packages
5. Add your Jupyter notebooks and report PDF (from Overleaf)

?


