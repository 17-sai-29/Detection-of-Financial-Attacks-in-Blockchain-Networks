# Detection-of-Financial-Attacks-in-Blockchain-Networks
Studied financial attack patterns in Ethereum transactions by analyzing key behavioral features. Performed statistical analysis to identify anomaly thresholds, used graph visualizations for structural insights, and applied machine learning to detect and classify anomalous activities.

# 🔍 Ethereum Financial Attack Detection using Feature Analysis and Machine Learning

This project focuses on identifying and classifying **financial attack patterns in Ethereum transaction data**. By combining statistical analysis, graph-based modeling, and machine learning, it aims to uncover anomalies and malicious behaviors commonly seen in blockchain activity.

---

## 🧠 Project Overview

- Studied known financial attacks (e.g., Ponzi schemes, phishing contracts, exploit patterns).
- Analyzed **key behavioral features** such as:
  - Gas usage
  - Transfer frequency
  - Contract creation/interaction
  - Transaction volume and timing
- Identified **statistical thresholds** to separate benign and suspicious activity.

---

## 📈 Methodology

### 1. **Data Exploration**
- Parsed Ethereum transaction datasets with fields such as `from`, `to`, `value`, `gasUsed`, `timestamp`, etc.
- Filtered and normalized data to highlight behaviorally significant accounts.

### 2. **Statistical Analysis**
- Computed descriptive statistics per account.
- Identified upper and lower bounds on behavior (e.g., unusually high transaction volume in short time).

### 3. **Graph Visualization**
- Represented transactions as a **directed graph**:
  - Nodes = Accounts (EOAs or Contracts)
  - Edges = Transactions (weighted by frequency, value, or gas)
- Visualized structural anomalies, dense subgraphs, or propagation chains linked to attacks.

### 4. **Machine Learning for Detection**
- Engineered features from both raw data and graph metrics.
- Trained models like Decision Trees, Random Forest, and SVM to detect anomalous accounts.
- Used labeled historical attack data (where available) for supervised learning.

---

## 🔧 Technologies Used

- **Python**: pandas, numpy, matplotlib, scikit-learn, networkx
- **Blockchain Dataset**: Ethereum transactions csv format
- **Visualization**: Matplotlib, Seaborn, Graphviz, NetworkX

---


## 📊 Results

- Models achieved high accuracy in detecting anomalous behavior patterns.
- Statistical thresholds proved effective in early-stage filtering.
- Graph visualizations revealed meaningful clusters of suspicious nodes.

---
