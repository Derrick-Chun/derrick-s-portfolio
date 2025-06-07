# Derrick Chun’s GitHub Portfolio

Hi, I’m Derrick. Welcome to my portfolio! Below are selected projects showcasing my skills in data analysis, software engineering, and machine learning.

🔗 **Connect with me:** [LinkedIn](https://www.linkedin.com/in/derrick-chun/) | [Email](mailto:derrickchun107@gmail.com)

---

## 🚀 Selected Projects

### 🪙 Crypto Trust Network Analysis

🔗 **GitHub Repository:** [Derrick-Chun/DS210_FinalProject](https://github.com/Derrick-Chun/DS210_FinalProject)

- **Course**: DS 210: Programming for Data Science (Boston University)  
- **Language**: Rust  
- **Description**: Built a Rust-based analytics engine to examine whether **trust between users** in a decentralized crypto network (Bitcoin Alpha) leads to **more transaction activity**.

**Research Question:** Does greater trust correlate with higher interaction in a decentralized network?

#### 🛠️ Tools & Techniques
- Programming: Rust  
- Analysis: BFS-based graph analysis & adjacency maps  
- Visualization: Histograms & scatter plots via `Plotters`  
- Core Logic: Weighted directed graph from CSV → BFS → degree & trust-score metrics

#### 🧠 Key Findings
- High-trust users form **fewer but stronger ties**  
- Highly connected users show moderate trust—broad vs. deep relationships  
- More connections ≠ more trust

#### 💻 How to Run the Code
```bash
git clone https://github.com/Derrick-Chun/DS210_FinalProject.git
cd DS210_FinalProject
cargo test
cargo run
cargo run --release
```

---

### 🏀 NBA MVP Prediction (2023–2024)

🔗 **GitHub Repository:** [derrick-chun/nba-mvp-prediction](https://github.com/derrick-chun/nba-mvp-prediction)

- **Course**: CDS DS 110: Intro to Data Science (Boston University)  
- **Language**: Python  
- **Team**: Derrick Chun, Pavan Kumar, Cole Ouyang, Kelsey Keate  

**Description:**  
Built and compared Decision Tree & K-Nearest Neighbors models to predict the Top 5 NBA MVP candidates for the 2023–2024 season using historic player stats (2019–2023) and MVP voting data.

**Research Question:**  
Can stat-only models accurately flag Top 5 MVP candidates?

#### 🛠️ Tools & Techniques
- Data wrangling: Pandas, NumPy  
- Machine learning: Scikit-learn (DecisionTreeClassifier, KNeighborsClassifier)  
- Statistical testing: SciPy (T-test, ANOVA)  
- Visualization: Seaborn, Matplotlib (heatmaps, bar charts, scatter plots)

#### 🧠 Key Findings
- Accurately flagged MVP candidates like **Giannis Antetokounmpo**  
- T-tests & ANOVA confirmed that PPG, RPG, APG, SPG, and BPG differ significantly for MVPs  
- Some “near-MVP” players were misclassified, highlighting the limits of stat-only approaches

#### 💻 How to Run the Code
```bash
git clone https://github.com/derrick-chun/nba-mvp-prediction.git
cd nba-mvp-prediction
pip install -r requirements.txt
jupyter notebook Chun_CDSDS110_FinalProject_Coding.ipynb
```

---

### 📄 MA214 Final Project: Social Media Habits Analysis

🔗 **GitHub Repository:** [derrick-chun/ma214-final-project](https://github.com/derrick-chun/ma214-final-project)  
📄 **Paper (PDF):** [MA214_Final_Project_Paper.pdf](https://github.com/derrick-chun/ma214-final-project/blob/main/MA214_Final_Project_Paper.pdf)  
🌐 **Dataset:** https://www.kaggle.com/datasets/zeesolver/dark-web

- **Course**: MA 214: Statistical Methods (Boston University)  
- **Language**: R  
- **Team**: Derrick Chun, Andrew Gibson, Linh Lai, Jiakai Lin, Emily Zhao  

**Description:**  
A comprehensive statistical analysis examining whether user demographics and engagement metrics can predict daily social-media usage. We applied t-tests, ANOVA, linear regression (with confidence & prediction intervals), chi-square tests, stepwise selection, and generalized linear models.

**Research Question:**  
Can demographics (age, income) and usage behaviors (video time, session count, scroll rate) accurately predict total time spent on social media?

#### 🛠️ Methods
- **Data Wrangling:** `readr` for CSV import and cleaning  
- **Statistical Tests:**  
  - T-test comparing life expectancy by TV density  
  - Chi-square tests on gender, profession, platform, and watch‐reason distributions  
- **Modeling:**  
  - Linear regression (Total_Time_Spent ~ Video_Time)  
  - Confidence & prediction intervals via `predict()`  
  - Stepwise model selection (`step()`)  
  - Generalized linear model for categorical predictors  

#### 🧠 Key Findings
- **Video time** is the only marginally significant predictor (β ≈ 0.55, p ≈ 0.04).  
- “Habitual watch reason” shows significance in the GLM (p < 0.05).  
- Overall, **no strong univariate predictors** beyond those two variables.

#### 💾 How to View

- **Read the PDF file:**  
  [MA214_Final_Project_Paper.pdf](https://github.com/derrick-chun/ma214-final-project/blob/main/MA214_Final_Project_Paper.pdf)


