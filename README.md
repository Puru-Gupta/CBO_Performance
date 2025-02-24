# Abnormal CBOs Affinity Group detection
Maped SHGs to a vector space using key repayment features (loan amount, overdue days, repayment frequency, past borrowing history) and loan repayment similarity as a continuous function of Euclidean distance in the feature space.
In Clustering Step, Applied a clustering algorithm on the SHG feature vectors which segregates the SHGs into different clusters based on repayment behavior.
and finally in selection step Clusters is identified where SHGs consistent on-time payments (high-performing), irregular repayments (medium risk), significant overdue loans (low-performing, high risk).

# **Abnormal CBOs Affinity Group Detection**

## **Overview**
This repository contains an implementation of **Abnormal CBOs Affinity Group Detection**, which identifies **Self-Help Groups (SHGs)** with abnormal repayment behavior using **vector space representation and clustering algorithms**. This approach helps financial institutions assess loan repayment risks and make informed credit decisions.

---

## **🛠️ Methodology**

### **1️⃣ Mapping SHGs to a Vector Space**
Each SHG is represented as a **numerical vector** using key repayment features:
- **Loan Amount** – Total amount borrowed.
- **Overdue Days** – Number of days a loan is overdue.
- **Repayment Frequency** – Weekly, monthly, etc.
- **Past Borrowing History** – Previous loan patterns.
- **Loan Repayment Similarity** – Measured using **Euclidean distance**.

# **Why Euclidean Distance?**
- SHGs with **similar repayment behaviors** are closer in space.
- SHGs with **different repayment behaviors** are farther apart.

---

### **2️⃣ Clustering Step (Grouping Based on Similarity)**
Once SHGs are mapped to a feature space, a **clustering algorithm** is applied to identify distinct repayment behavior groups.

#### **Clustering Algorithms Used**
- **K-Means Clustering** – Segments SHGs into predefined groups based on repayment patterns.
- **DBSCAN** – Identifies outliers and groups SHGs with dense repayment similarities.
- **Hierarchical Clustering** – Builds a tree-like structure to visualize SHG repayment behavior.

# **What Happens Here?**
- SHGs with **similar repayment behavior** are grouped together.
- The algorithm **automatically detects patterns** in SHG repayment.

---

### **3️⃣ Selection Step (Identifying Risk Groups)**
After clustering, SHGs are categorized into three risk groups:

#### **✅ High-Performing SHGs (On-Time Payments)**
- Consistently repaying loans on time.
- Low-risk and eligible for better credit opportunities.

#### ** Medium-Risk SHGs (Irregular Repayments)**
- Occasionally delayed payments.
- Require monitoring to prevent risk escalation.

#### ** High-Risk SHGs (Frequent Overdue Loans)**
- Regular loan defaults or overdue payments.
- Higher financial instability and require intervention.

**Why is This Important?**
- Helps **microfinance institutions** identify SHGs needing intervention.
- Enables **risk-based credit decision-making**.
- Prevents **loan defaults** through proactive management.
  
---

## ** Results & Visualization**
- **Heatmaps** of repayment patterns.
- **Clustering visualizations** using PCA.
- **Risk group distribution charts**.

---


**This project enables smarter financial decision-making by detecting abnormal repayment patterns in SHGs.!**
