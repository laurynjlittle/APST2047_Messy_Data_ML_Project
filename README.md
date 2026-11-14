## Messy Data Machine Learning: Group Project

Fraud, Scams, and their reporting in the Age of AI

---

### Project Workflow & Setup
1. Open the target notebook in Google Colab (`File > Open notebook > GitHub`) or Open directly from GitHub.
2. Run **Section 0 (Setup)** at the top of the notebook to mount Google Drive (`/content/drive/MyDrive/Messy_Data_ML_Group_Project`) and clone/pull the latest repository code.
3. Save progress back to GitHub using **File > Save a copy in GitHub** (or via `git_push()` after saving the active notebook to Drive).

--- 

### Notebook Pipeline

#### `NB0_Messy_Data_Dataset_Assembly.ipynb` — Data Assembly & Ingestion
* **Environment & Storage Initialization:** Mounts shared Google Drive directories (`Data/`, `models/`, `outputs/`) and clones the GitHub repository into the Colab runtime.
* **Raw Data Acquisition:** Pulls and consolidates raw fraud and scam reporting datasets into a unified ingestion pipeline.
* **Master Dataset Export:** Saves the assembled baseline dataset to `Data/` on Google Drive for downstream preprocessing and modeling.

#### `NB1_Messy_Data_Dataset_Preprocessing.ipynb` — Data Cleaning, Feature Engineering, EDA
* **Data Loading & Preprocessing:** Loads the assembled dataset from `Data/` and resolves messy data artifacts (text normalization, missing value imputation, outlier handling, and type standardization). Preliminary visualizations saved to `outputs/`.
* **Exploratory Data Analysis (EDA):** Examines reporting trends, scam categories, temporal shifts, and key predictive signals.
* **Feature Engineering:** Constructs domain-specific and text/tabular features tailored to fraud detection and reporting patterns.

#### `NB2_Messy_Data_Models.ipynb` — Model Training & Evaluation
* **Model Training & Evaluation:** Trains baseline and candidate ML models, evaluates performance metrics, and exports trained artifacts to `models/` and `outputs/`.


