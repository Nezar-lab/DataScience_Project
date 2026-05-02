Data science project for ARTI506

# AI-Driven Phishing Detection

## Project Idea

Phishing emails remain one of the most pervasive cyber threats, tricking users into revealing sensitive information or downloading malware. Traditional email filters rely on static blacklists and rule-based heuristics, making them ineffective against constantly evolving attack tactics (e.g., AI-generated text, lookalike domains).

This project addresses the question: **How can machine learning models trained on historical email data accurately classify phishing emails without relying on static rules?**

We implement and compare three classification models:
- **Logistic Regression** (baseline)
- **Random Forest** (bagging ensemble)
- **Gradient Boosting** (boosting ensemble)

The goal is to evaluate which model achieves the best balance of precision, recall, and F1-score for real-world cybersecurity applications, with special emphasis on **minimizing false negatives** (missed phishing attacks).

## Dataset

**Source:** [Phishing Email Dataset](https://www.kaggle.com/datasets/naserabdallahalam/phishing-email-dataset) by Naser Abdullah Alam (Kaggle)

**Reference:** Al-Subaiey, A., Al-Thani, M., Alam, N. A., et al. (2024). *Novel Interpretable and Robust Web-based AI Platform for Phishing Email Detection*. ArXiv. https://arxiv.org/abs/2405.11619

**Key Characteristics:**
| Property | Details |
|----------|---------|
| Size | ~39,150 labeled emails |
| Classes | 55.8% Phishing (1), 44.2% Legitimate (0) |
| Sources | Enron, CEAS, Nazario, Nigerian Fraud, Ling, SpamAssassin |
| Features | Sender, receiver, date, subject, body, label, URLs |

**Why this dataset?**
- **Diversity:** Six distinct sources reduce source bias and provide linguistic variety across different attack types and eras.
- **Near-balanced classes:** Minimizes the need for aggressive resampling.
- **Rich features:** Raw body text, subject lines, sender metadata, timestamps, and URLs support NLP and feature engineering.
