# Derrick Chun's Portfolio

## [Final Project: Crypto Network Analysis](https://github.com/Derrick-Chun/DS210_FinalProject)

This was my final project for the course **DS 210: PROGRAMMING FOR DS** under Professor Chator at Boston University (Fall 2024). I built a Rust-based analytics engine to investigate whether higher **trust** between users in a decentralized crypto network (Bitcoin Alpha) leads to more **transaction activity**.

---

### 🔍 Project Focus
**Main Hypothesis**: *Does higher trust lead to higher transactions in the Bitcoin Alpha network?*

This project explores the social dimension of blockchain: the trust dynamics between pseudonymous users. Motivated by my interest in finance, digital currency, and the impact of decentralized systems, I wanted to understand how trust facilitates—or hinders—user interaction in a trust-scored crypto environment.

---

### 📊 Dataset
- **Name**: Bitcoin Alpha Trust Weighted Signed Network  
- **Source**: [Stanford SNAP](https://snap.stanford.edu/data/soc-sign-bitcoin-alpha.html)  
- **Nodes (Users)**: 3,783  
- **Edge Weights**: -10 (distrust) to +10 (trust)  
- **Positive Trust Edges**: 93%  

**Citation**:  
Kumar et al. (2016). *Edge Weight Prediction in Weighted Signed Networks*. [Link to Paper](https://cs.stanford.edu/~srijan/pubs/wsn-icdm16.pdf)

---

### 🛠️ Tools & Techniques
- **Language**: Rust  
- **Libraries**: `Plotters`, `VecDeque`, `HashMap`, `rand`  
- **Key Methods**:  
  - Breadth-First Search (BFS) for shortest paths  
  - Degree distribution and histogram generation  
  - Trust-Degree correlation (scatter plot visualization)  
  - Unit testing for metric validation

---

### 📈 Methodology
- Parsed CSV of trust ratings to construct a **weighted directed graph**  
- Built adjacency lists using `HashMap<i32, Vec<i32>>`  
- Implemented BFS to compute **average shortest path** across sampled user pairs  
- Calculated **degree distribution** to identify network hubs and isolated users  
- Visualized:  
  - `degree_distribution_histogram.png`  
  - `trust_vs_degree.png`  
- Tested correlation between **average trust scores** and **node degrees**  
- Outlier analysis of users with low/high trust & activity

---

### 🔍 Key Findings
- Most users with **high trust scores** had **low degrees** (selective, strong ties)  
- Users with **many connections** tended to have **moderate trust**  
- Some nodes showed **high connectivity despite low or negative trust**, suggesting complex dynamics  
- Results suggest that **trust does enable transactions**, but high engagement doesn’t always correlate with high trust

---

### 🧪 How to Run the Code

> ⚙️ **Requirements**: Rust 1.77+, Plotters crate  
```bash
git clone https://github.com/derrickchun/crypto-trust-analysis  
cd crypto-trust-analysis/src  
cargo test              # Run unit tests  
cargo run               # Run analysis  
# or for optimized performance
cargo run --release     
