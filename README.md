# 💊 Drug–Target Interaction Predictor

A machine learning web app that predicts whether a drug molecule
will bind to a protein target — built for drug discovery applications.

## 🔗 Live Demo
👉 https://dti-predictor-hff4f9lx9ae6g6xac6sfgd.streamlit.app

## 🧠 How it works
1. Enter any drug molecule as a SMILES string
2. Select a protein target (EGFR, BRAF, CDK2, HDAC1, VEGFR2, BCL2, DRD2)
3. Get an instant binding probability prediction with 2D molecule visualization

## 📊 Model Performance
- Algorithm  : XGBoost Classifier
- ROC-AUC    : 0.993
- Accuracy   : 96.8%
- Training data : 10,000+ ChEMBL bioactivity records

## 🛠️ Tech Stack
- Data      : ChEMBL API, UniProt API
- Features  : RDKit Morgan Fingerprints (2048 bits) + Amino Acid Composition
- Model     : XGBoost
- Dashboard : Streamlit
- Deployment: Streamlit Community Cloud

## 🧪 Example drugs to try
| Drug | SMILES | Expected target |
|------|--------|----------------|
| Erlotinib | COCCOC1=CC2=C(C=C1OCCOC)C(=NC=N2)NC3=CC=CC(=C3)C#C | EGFR |
| Vemurafenib | CCCS(=O)(=O)NC1=CC=C(F)C(C(=O)C2=CNC3=NC=C(Cl)C=C23)=C1 | BRAF |
| Aspirin | CC(=O)OC1=CC=CC=C1C(=O)O | None (low binding) |