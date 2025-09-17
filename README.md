
MLSE assignment 4
# MLOps Lab 4 — CI/CD with DVC

This project demonstrates a simple **Machine Learning pipeline** (Linear Regression) integrated with **DVC** for data versioning and **GitHub Actions** for CI/CD automation.  


--

# Install dependencies
pip install -r requirements.txt

# Initialize DVC (only first time)
dvc init

# Reproduce pipeline
dvc repro

# Show tracked metrics
dvc metrics show

MLops_Lab-4/
├─ data/
│   └─ raw/                  # Raw dataset (input data)
│
├─ src/
│   ├─ train.py              # Training script
│   └─ evaluate.py           # Evaluation script
│
├─ .dvc/                     # DVC internal files
├─ .dvcignore                # Ignore patterns for DVC
├─ .github/workflows/ci.yml  # GitHub Actions CI/CD pipeline
├─ dvc.yaml                  # DVC pipeline definition
├─ params.yaml               # Model hyperparameters
├─ requirements.txt          # Python dependencies
└─ README.md                 # Project documentation

