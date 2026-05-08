# 🛡️ Misinformation Detection for African News Contexts
### NLP-based text classification pipeline for information integrity monitoring

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/misinformation-detection-africa/blob/main/misinformation_detection_africa.ipynb)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)

---

## Overview

Misinformation is one of the most pressing challenges facing African digital spaces — spreading through WhatsApp chains, social media, and informal news channels faster than fact-checkers can respond. This project builds a **reproducible NLP pipeline** that classifies text statements as *reliable* or *potentially misleading*, using the LIAR benchmark dataset as a foundation.

The work is grounded in a civic tech context: rather than treating misinformation detection as a purely technical problem, this notebook frames it as a **governance and digital rights challenge**, examining both the capabilities and the limits of automated detection in African information ecosystems.

---

## What this project demonstrates

| Skill | Detail |
|-------|--------|
| **NLP fundamentals** | TF-IDF vectorisation, text preprocessing, n-gram features |
| **ML classification** | Logistic Regression baseline with cross-validation |
| **Model evaluation** | Precision, recall, F1-score, ROC-AUC, confusion matrix |
| **Interpretability** | Top predictive features visualised per class |
| **Civic framing** | Explicit discussion of African context, language gaps, and ethical limits |

---

## Key results

- **ROC-AUC: ~0.74** on LIAR test set using TF-IDF + Logistic Regression
- **5-fold CV F1** consistently above 0.65 — solid baseline for an interpretable model
- **Confusion matrix** and **top feature analysis** included for full transparency

---

## Visualisations

The notebook produces 4 publication-quality charts:
1. Label distribution (original 6-class + binary)
2. Statement length by class
3. Confusion matrix + ROC curve
4. Top 15 predictive words for each class (Fake vs Real)

---

## Limitations & next steps

This baseline intentionally uses an interpretable model over a black-box transformer — in civic contexts, **explainability matters as much as accuracy**.

Planned extensions:
- Fine-tune `xlm-roberta-base` for multilingual transfer to French/Camfranglais
- Build a French-language dataset from AfricaCheck and Désinfox Afrique fact-checks
- Deploy as a lightweight REST API for integration into civic monitoring dashboards

---

## Quick start

```bash
# Run directly in Google Colab — no local setup required
# Click the "Open in Colab" badge above

# Or locally:
pip install scikit-learn pandas matplotlib seaborn datasets
jupyter notebook misinformation_detection_africa.ipynb
```

---

## References

- Wang, W. Y. (2017). Liar, Liar Pants on Fire: A New Benchmark Dataset for Fake News Detection. *ACL 2017*
- AfricaCheck — https://africacheck.org
- AfricTivistes — https://africTivistes.org

---

**Author:** Pantouin Adjinsala · University Lecturer & Civic Tech Contributor, AfricTivistes CitizenLab Cameroon  
**Part of:** [AI for Social Good portfolio](https://github.com/YOUR_USERNAME)
