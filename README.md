# **Text Clustering with Non-Negative Matrix Factorization**

This project investigates document clustering on a selected subset of the **20 Newsgroups** dataset using **Non-Negative Matrix Factorization (NMF)** and two versions of **K-Means clustering**. The goal is to analyze how well NMF reveals latent topics compared to K-Means implemented both **from scratch** and using **Scikit-Learn**, and to compare their clustering performance.

---

## **Project Overview**

* **Dataset Selection:**
  A subset of five categories from the 20 Newsgroups dataset is used. After text cleaning and preprocessing, the documents are converted into a **TF–IDF weighted Document–Term matrix**.

* **Text Preprocessing:**
  Cleaning, stopword removal, and tokenization are performed using **NLTK**. TF–IDF scaling is then applied to highlight meaningful terms.

* **NMF Clustering:**
  The **NMF algorithm** is applied to the TF–IDF matrix to extract latent topics. Each document is assigned to the topic with the highest activation score.

* **K-Means Clustering (Two Approaches):**

  1. **K-Means implemented from scratch**, following the classic algorithm (initialization, centroid updates, assignment step).
  2. **K-Means using Scikit-Learn**, serving as an optimized and standardized implementation.
     Results from both implementations are compared to assess correctness and performance differences.

* **Method Comparison:**
  The clustering results of:

  * NMF
  * K-Means (from scratch)
  * K-Means (Scikit-Learn)
    are evaluated and compared.

* **Evaluation Metrics:**
  Performance is measured using:

  * **Silhouette Score**
  * **Adjusted Mutual Information (AMI)**
  * **Adjusted Rand Index (ARI)**

This project highlights how matrix factorization and clustering algorithms behave on textual data and provides a clear comparison between manual and library-based implementations.
