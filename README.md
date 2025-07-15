# 🧠 Disease Prediction using Symptom-Based Heterogeneous Network and Network Analysis

This project models relationships between diseases and symptoms as a **heterogeneous network** and applies **Social Network Analysis (SNA)** techniques to predict diseases, uncover symptom relationships, detect communities, and rank clinically important nodes.

---

## 📌 Project Objectives

1. **Model Data as a Network:**
   - Nodes:
     - 🔴 **Disease Nodes** (e.g., *Pneumonia*, *Diabetes Mellitus*)
     - 🟡 **Symptom Nodes** (e.g., *Fever*, *Cough*, *Blurred Vision*)
   - Edges:
     - **Disease–Symptom Edge**: Links a disease to its symptoms.
     - **Symptom–Symptom Edge**: Co-occurrence of symptoms in diseases.
     - **Disease–Disease Edge**: Based on symptom overlap.

2. **Key Research Questions:**
   - Can we predict diseases from a given symptom set?
   - Which symptoms co-occur most often?
   - What diseases are similar based on shared symptoms?
   - Which symptoms or diseases are most central or influential?

---

## 🧪 Social Network Analysis (SNA) Techniques

- **Centrality Measures**:
  - `Degree`, `Betweenness`, `Closeness`, `Eigenvector`
- **Community Detection**:
  - `Louvain Algorithm`, `Spectral Clustering`
- **Similarity Measures**:
  - `Jaccard`, `Cosine` similarity
- **Network Metrics**:
  - Degree Distribution, Density, Components, Clustering Coefficient
- **Visualization**:
  - Node-link diagrams for intuitive insights

---

## 🧮 Algorithms Implemented

### 🔍 Disease Prediction:
- Compute similarity between input symptom set and disease profiles using:
  - `Jaccard Similarity`
  - `Cosine Similarity`

### 🤝 Symptom Relationship Analysis:
- Symptom co-occurrence frequency using edge weights
- Symptom-symptom subgraph analysis

### 🔗 Disease Similarity Analysis:
- Compare diseases using shared symptom profiles

### ⭐ Node Importance:
- Rank symptoms/diseases using centrality measures

### 🧬 Community Detection:
- Louvain for modularity-based partitioning
- Spectral Clustering using graph Laplacian decomposition

---

## 📊 Dataset and Experimental Design

- **Dataset Source**: Disease–Symptom Knowledge Base (Columbia University)
- **Steps:**
  1. Load and clean dataset
  2. Construct heterogeneous graph
  3. Analyze network metrics and centralities
  4. Apply clustering algorithms
  5. Predict diseases using symptom similarity
  6. Visualize results

---

## 📈 Results Summary

- **Network Created**: Nodes (Diseases + Symptoms), weighted edges for co-occurrence/similarity
- **Communities Detected**:
  - Logical clusters (e.g., Respiratory, Neurological, Psychiatric)
- **High-Centrality Symptoms**:
  - *Pain*, *Fever*, *Shortness of Breath*
- **High-Centrality Diseases**:
  - *Pneumonia*, *Chronic Kidney Failure*, *Bipolar Disorder*
- **Prediction Accuracy**:
  - Methods returned relevant predictions (e.g., *Chronic Obstructive Airway Disease*, *Heart Failure Congestive*)

---

## 🔍 Key Observations

- **General vs Specific Symptoms**:
  - General symptoms (e.g., fever) have high centrality but low specificity
- **Disease Overlap**:
  - Many diseases share symptoms → strong interconnectivity
- **Community Structure**:
  - SNA reveals modular and clinically relevant groupings

---

## 🚀 Future Work

- Use **Graph Neural Networks (GNNs)** for disease prediction
- Incorporate **patient demographic and history data**
- Extend network with **temporal data** to model disease progression

---

