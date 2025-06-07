# Derrick Chun's Portfolio

Welcome! Below are selected data science and analytics projects I’ve completed as part of my academic and independent work.

---

## 🪙 Crypto Trust Network Analysis

🔗 [View GitHub Repo](https://github.com/Derrick-Chun/DS210_FinalProject)

**Course**: DS 210: Programming for Data Science (Boston University)  
**Instructor**: Prof. Chator  
**Language**: Rust

In this final project, I built a Rust-based analytics engine to examine whether **trust between users** in a decentralized crypto network (Bitcoin Alpha) leads to **more transaction activity**.

---

### 🔍 Focus
**Research Question**: Does greater trust correlate with higher interaction in a decentralized network?

Motivated by an interest in blockchain and social-financial dynamics, this project explores how trust shapes engagement in the Bitcoin Alpha trust graph.

---

### 📊 Dataset
- **Bitcoin Alpha Trust Network** from [Stanford SNAP](https://snap.stanford.edu/data/soc-sign-bitcoin-alpha.html)  
- 3,783 nodes (users), edge weights from -10 to +10  
- 93% of edges represent positive trust

---

### 🛠️ Tools & Techniques
- Rust programming  
- Graph analysis using BFS and adjacency maps  
- Histogram and scatter plot visualizations (`Plotters` crate)  
- Unit-tested trust/distance metrics

---

### 📈 Key Methods
- Constructed a **weighted directed graph** from CSV  
- Ran BFS to estimate shortest paths between sampled user pairs  
- Visualized degree distribution and trust-score correlation  
- Analyzed trust vs. connectivity to understand network behavior

---

### 🧠 Findings
- Users with high trust scores tend to have **fewer but stronger ties**  
- Highly connected users show moderate trust — possibly due to broad, shallow connections  
- Trust facilitates interaction, but **more connections ≠ more trust**

---

### 💻 How to Run the Code
```bash
git clone https://github.com/derrickchun/crypto-trust-analysis  
cd crypto-trust-analysis/src  
cargo test               # Run unit tests  
cargo run                # Run analysis  
cargo run --release      # Optimized version

## 🏀 NBA MVP Prediction (2023–2024)

🔗 [View GitHub Repo](https://github.com/derrick-chun/nba-mvp-prediction)

**Course**: CDS DS 110 (Boston University)  
**Language**: Python  
**Team**: Derrick Chun, Pavan Kumar, Cole Ouyang, Kelsey Keate

This group project predicts the **Top 5 NBA MVP candidates** for the 2023–2024 season using machine learning models trained on player stats and MVP voting data from 2019–2023.

---

### 📊 Methods
- **Machine Learning**:  
  - Decision Tree Classifier  
  - K-Nearest Neighbors (k = 1–10)  
- **Statistical Analysis**:  
  - T-Test (PPG significance by MVP rank)  
  - ANOVA (comparing average stats for MVPs)  
- **Visualizations**:  
  - Heatmaps, bar charts, scatter plots of player performance by season

---

### 🧠 Key Findings
- Both ML models accurately predicted MVP candidates like **Giannis Antetokounmpo**  
- Statistical tests confirmed **PPG and other stats significantly differ** for MVPs  
- Some players were misclassified, suggesting limitations in stat-only models

---

### 🎯 Personal Contributions
- Full code implementation for:  
  - Decision Tree Classifier  
  - K-Nearest Neighbors  
  - T-Test and ANOVA  
  - Heatmap visualizations  
- Data cleaning, integration, and feature engineering  
- Slide deck content, coding, and analysis writing

---

### 📂 Project Materials
- 📘 [Jupyter Notebook](https://github.com/derrick-chun/nba-mvp-prediction/blob/main/Chun_CDSDS110_FinalProject_Coding.ipynb)  
- 🖥️ [Presentation Slides (PDF)](https://github.com/derrick-chun/nba-mvp-prediction/blob/main/Chun_Kumar_Ouyang_Keate_DS110_FinalProject_Presentation.pdf)  
- 📄 [Final Research Paper (PDF)](https://github.com/derrick-chun/nba-mvp-prediction/blob/main/Chun,%20Keate,%20Kumar,%20Ouyang_DS110%20Paper.pdf)
