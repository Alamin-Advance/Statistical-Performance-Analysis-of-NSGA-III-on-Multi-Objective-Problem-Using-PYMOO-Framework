# Statistical-Performance-Analysis-of-NSGA-III-on-Multi-Objective-Problem-Using-PYMOO-Framework

📌 Overview
This repository presents a comprehensive statistical performance analysis of NSGA-III (Non-dominated Sorting Genetic Algorithm III) on standard multi-objective optimization problems (MOPs) from the ZDT and DTLZ benchmark suites. The study evaluates NSGA-III using multiple performance metrics, including:

Hypervolume (HV)

Generational Distance (GD)

Spacing

Inverted Generational Distance (IGD)

R2 Indicator

Epsilon (ϵ)

The implementation and testing were conducted using the PyMOO framework, ensuring reproducibility and scalability.

🔍 Key Findings
✅ NSGA-III performs robustly on ZDT problems, excelling in convergence (GD, IGD) and distribution (HV, Epsilon).
✅ Strong diversity maintenance in complex DTLZ problems, though differences in HV and R2 were less pronounced.
✅ Statistical significance tests (Wilcoxon, Friedman) confirm NSGA-III's superior performance in most cases.
✅ MOEA/D comparison highlights NSGA-III's advantages in maintaining diversity, while MOEA/D may be preferable for decomposition-friendly problems.

📊 Benchmark Problems Evaluated
Problem Suite	Test Problems
ZDT	ZDT1, ZDT2, ZDT3, ZDT4, ZDT6
DTLZ	DTLZ1, DTLZ2, DTLZ3, DTLZ4
📈 Performance Metrics
Six key metrics were used to assess solution quality:

Hypervolume (HV) → Measures volume dominated by Pareto front. (Higher = Better)

Generational Distance (GD) → Average distance to true Pareto front. (Lower = Better)

Spacing → Uniformity of solution distribution. (Lower = Better)

Inverted Generational Distance (IGD) → Convergence + Diversity. (Lower = Better)

R2 Indicator → Convergence using reference points. (Lower = Better)

Epsilon (ϵ) → Worst-case deviation from true Pareto front. (Lower = Better)

📂 Repository Structure
text
├── /notebooks/       # Jupyter notebooks with analysis  
├── /data/            # Benchmark results (CSV/JSON)  
├── /figures/         # Boxplots, convergence plots  
├── /src/             # PyMOO implementation scripts  
├── requirements.txt  # Python dependencies  
└── README.md  
🛠️ Installation & Usage
Clone the repository

bash
git clone https://github.com/yourusername/nsga3-statistical-analysis.git
cd nsga3-statistical-analysis
Install dependencies

bash
pip install -r requirements.txt
Run the analysis

Execute notebooks in /notebooks/ to reproduce experiments.

Modify /src/nsga3_pymoo.py for custom benchmarks.

📜 Citation
If this work aids your research, please cite:

bibtex
@misc{citationkey,
  author = {},
  title = {Statistical Performance Analysis of NSGA-III on Multi-Objective Benchmark Problems},
  year = {2025},
  publisher = {},
  journal = {},
  howpublished = {\url{}}
}
🤝 Contributing
Contributions are welcome! Open an Issue or Pull Request for improvements.

📧 Contact
For questions, contact: alaminh1411@example.com

🔹 Built with PyMOO | Open-source Multi-Objective Optimization 🔹
