# NumPy Repository Analysis
**RQ2 - Which parts of the codebase evolve the most, and how does 
file-level activity vary across the project structure?**

This project performs an empirical analysis of the NumPy GitHub 
repository using PyDriller. It extracts 23 years of commit history, 
computes code churn at the file and component level, and produces 
four visualizations to answer RQ2.

---

## How to reproduce

### 1. Clone this repository
git clone <https://github.com/hafsaSaih/numpy-analysis.git>
cd numpy-analysis

### 2. Clone the NumPy repository into the same folder
git clone https://github.com/numpy/numpy.git

Your folder should look like this:
numpy-analysis/
├── analysis.ipynb
├── numpy/          ← cloned here
├── data/
├── plots/
└── ...

### 3. Create a virtual environment and install dependencies
python -m venv venv
venv\Scripts\activate        # Windows
pip install -r requirements.txt

### 4. Register the kernel
python -m ipykernel install --user --name=numpy-analysis 
                             --display-name "Python (numpy-analysis)"

### 5. Launch Jupyter and run the notebook
python -m jupyter notebook

Open analysis.ipynb and run all cells in order.
Note: Cell 4 (full extraction) takes approximately 20-45 minutes.

---

## Repository structure
analysis.ipynb              main analysis notebook
requirements.txt            pinned library versions
data/                       cleaned datasets (CSV)
plots/                      all four visualizations (PNG)
docs/reflection.pdf         written reflection document
docs/ai_session.pdf         full AI assistance session

---

## Environment
Python 3.11
pandas 3.0.3
pydriller 2.10
seaborn 0.13.2
