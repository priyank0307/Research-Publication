# Automated Ticket Categorization Using BERT and Azure ML

[![PDF Document](https://img.shields.io/badge/Document-PDF-red.svg)](./conference_paper.pdf)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Official repository hosting the conference paper titled **"Automated Ticket Categorization Using BERT and Azure ML"**, authored by Priyank Raj, Raj Aryan, and Dr. Andhe Pallavi from RNSIT, Bangalore.

---

## 📋 Abstract
The project focuses on automating the categorization of queries received by Service Desks using advanced machine learning techniques to eliminate manual routing effort, reduce delays, and prevent misclassifications[cite: 1]. By replacing traditional logistic regression with BERT-based classification methods, the system ensures continuous learning, quick adaptation to new data, and a reduction in ticket misclassification rates[cite: 1]. The primary objectives are:
1. Creating an automatic Service Desk Ticket Issue Categorizer Model[cite: 1].
2. Deploying this model as a web service[cite: 1].

---

## 🤖 AI Architectures & Models
* **BERT (Bidirectional Encoder Representations from Transformers):** Used for detecting customer sentiment and enabling the prioritization of negative or urgent cases[cite: 1].
* **DistilBERT & TinyBERT:** Lightweight variants implemented to address standard BERT's high GPU requirements and slow training phases[cite: 1].
* **GPT-4:** Utilized for generating accurate, contextually appropriate responses to customer queries[cite: 1].

---

## 📊 Dataset & Query Distribution
The system utilizes the `Customer_Support_Training_Dataset.csv` dataset containing customer queries organized by issue type, priority level, sentiment, sample responses, resolution times, and feedback scores[cite: 1]. 

Key category frequencies in the dataset include:
* **ACCOUNT:** 5,986 entries (most frequent)[cite: 1]
* **ORDER:** 3,988 entries[cite: 1]
* **REFUND:** 2,992 entries[cite: 1]
* **INVOICE, CONTACT, PAYMENT, FEEDBACK, DELIVERY, & SHIPPING:** 2,000 entries each[cite: 1]
* **SUBSCRIPTION & CANCEL:** Least frequent categories[cite: 1]

---

## ⚙️ Methodology & Implementation
* **Azure ML Workspace Setup:** Configures data storage, compute resources, and environments for scalable model training and deployment[cite: 1].
* **Data Preprocessing:** Handles missing values, standardizes text, and removes noisy data[cite: 1].
* **Sentiment Analysis & Classification:** Assesses customer sentiment (positive, neutral, negative) and categorizes tickets by type[cite: 1].
* **Response Generation & UI:** Implements a Streamlit user interface where support agents can view prioritized/categorized tickets, choose responses, and review recommended actions[cite: 1].

---

## 📈 Evaluation & Results
* **Classification Performance:** Evaluated using standard classification metrics including Accuracy, Precision, and Recall[cite: 1].
* **Response Quality:** Evaluated using the BLEU score, achieving a score of **0.6177** for structured response workflows[cite: 1].

---

## 📄 Accessing the Paper
The full conference paper PDF is available directly in this repository: [`conference_paper.pdf`](./conference_paper.pdf)[cite: 1].

---

## 📖 Citation
If you reference or use this work in your research, please cite it as follows:

```bibtex
@inproceedings{raj2026automated,
  title={Automated Ticket Categorization Using BERT and Azure ML},
  author={Raj, Priyank and Aryan, Raj and Pallavi, Andhe},
  booktitle={Conference Proceedings},
  year={2026}
}
