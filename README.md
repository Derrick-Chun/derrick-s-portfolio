# Derrick Chun's Data Science Portfolio

Hi, I'm Derrick. Welcome to my portfolio! Below are selected projects showcasing my skills in data analysis, software engineering, and machine learning.

🔗 **Connect with me:** [LinkedIn]([https://www.linkedin.com/in/your-linkedin-url/](https://www.linkedin.com/in/derrick-chun/)) | [Email](derrickchun107@gmail.com)

---

## 🚀 Selected Projects

### 🪙 Crypto Trust Network Analysis

🔗 **GitHub Repository:** [Derrick-Chun/DS210_FinalProject](https://github.com/Derrick-Chun/DS210_FinalProject)

- **Course**: DS 210: Programming for Data Science (Boston University)
- **Language**: `Rust`
- **Description**: In this final project, I built a Rust-based analytics engine to examine whether **trust between users** in a decentralized crypto network (Bitcoin Alpha) leads to **more transaction activity**.

**Research Question**: Does greater trust correlate with higher interaction in a decentralized network?

#### 🛠️ Tools & Techniques
- **Programming**: Rust
- **Analysis**: Graph analysis using Breadth-First Search (BFS) and adjacency maps.
- **Visualization**: Histogram and scatter plot generation using the `Plotters` crate.
- **Core Logic**: Constructed a weighted directed graph from CSV data, ran BFS to analyze paths, and visualized key metrics like degree distribution and trust-score correlation.

#### 🧠 Key Findings
- Users with high trust scores tend to have **fewer but stronger ties**.
- Highly connected users show moderate trust—possibly due to broad, shallow connections.
- Trust facilitates interaction, but **more connections do not necessarily equal more trust**.

#### 💻 How to Run the Code
```bash
# Clone the repository
git clone [https://github.com/Derrick-Chun/DS210_FinalProject.git](https://github.com/Derrick-Chun/DS210_FinalProject.git)

# Navigate to the project directory
cd DS210_FinalProject

# Run unit tests
cargo test

# Run the analysis (debug mode)
cargo run

# Run the analysis (optimized release mode)
cargo run --release
