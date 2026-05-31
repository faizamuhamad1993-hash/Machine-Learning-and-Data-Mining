# Machine-Learning-and-Data-Mining
Mitigating Bias and Data Protection in Ai-Powered Educational Assessment Systems

# How to Run This Project

This repository contains a fairness and privacy-aware Automated Essay Scoring (AES) project implemented using Jupyter Notebook, Orange Data Mining, and MindSpore. Follow the steps below to set up the environment and reproduce the experiments.

## Project Files

├── 202507410_Supervised learning.ipynb      # Main Jupyter Notebook  
├── 202507410_Unsupervised_Orange.ows                     # Orange workflow file  
├── Dataset                                 # ASAP-2 dataset files   
├── README.md                               # Project instructions  

## Requirements

Make sure the following software is installed on your system:

- Python 3.8 or above
- Jupyter Notebook or JupyterLab
- Orange Data Mining (latest version)
- MindSpore (CPU version)

## Required Python Libraries

Install the required dependencies using pip:

```bash
pip install numpy pandas scikit-learn scipy matplotlib textstat nltk
```

For MindSpore (CPU version), follow the official installation guide:

```bash
pip install mindspore
```

## NLTK Setup

Some text preprocessing functions require NLTK resources. Run the following once before executing the notebook:

```python
import nltk


nltk.download('punkt')
nltk.download('stopwords')
```

## Dataset Setup

1. Download the ASAP-2 Automated Essay Scoring dataset.
2. Place the dataset files inside the project directory.
3. Update the dataset path in the notebook if necessary.

## Running the Jupyter Notebook

1. Clone this repository:

```bash
git clone https://github.com/your-username/your-repository-name.git
```

2. Navigate to the project folder:

```bash
cd your-repository-name
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open:

```text
202507410_Supervised learning.ipynb
```

5. Run all cells sequentially from top to bottom.

## Running the Orange Workflow

1. Open Orange Data Mining.
2. Select **Open Workflow**.
3. Load:

```text
202507410_Unsupervised_Orange.ows
```

4. Ensure the dataset path is correctly configured.
5. Execute the workflow to reproduce the clustering, PCA, and bias analysis results.

## Notes

- The project combines supervised learning in Jupyter Notebook with unsupervised learning in Orange Data Mining.
- Gradient Boosting was identified as the best-performing supervised model and was used for fairness auditing and bias mitigation.
- Privacy-preserving techniques such as pseudonymization, feature isolation, and data minimization were applied during preprocessing.
- Results may vary slightly depending on software versions and hardware specifications.

## Author

**Faiza Mohammed**

## Purpose

This project was developed for academic and research purposes to investigate fairness, bias, and privacy considerations in AI-based Automated Essay Scoring systems.
