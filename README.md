# Phishing Website Detection Using Machine Learning

## Project description
This cybersecurity project trains a Random Forest model to classify records from the UCI Phishing Websites dataset as phishing or legitimate. It demonstrates data preparation, model training, evaluation, feature importance, and model saving.

**Important:** This project uses pre-extracted dataset features. It does not visit URLs or guarantee that a website is safe.

## Dataset
- Name: UCI Machine Learning Repository — Phishing Websites
- Link: https://archive.ics.uci.edu/dataset/327/phishing+websites
- Download the dataset from the UCI page. Place the downloaded data file in the project folder and update `DATA_PATH` in the notebook to match the filename.

## Technologies used
- Python 3
- Jupyter Notebook
- pandas and NumPy
- scikit-learn
- Matplotlib
- joblib

## Project files
- `Yazir_PhishingWebsiteDetection.ipynb` — complete source code and explanations
- `requirements.txt` — Python dependencies
- `Yazir_ProjectReport.docx` — project report
- `README.md` — setup and project overview

## Setup and run
1. Install Python 3.10 or later.
2. (Recommended) Create and activate a virtual environment.
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Download the dataset from the UCI link above.
5. Put the data file in the same folder as the notebook. In the notebook, change `DATA_PATH = Path("phishing.csv")` to the actual filename.
6. Start Jupyter:
   ```bash
   jupyter notebook
   ```
7. Open `Yazir_PhishingWebsiteDetection.ipynb` and run the cells from top to bottom.

## Output
The notebook prints classification metrics and a classification report, displays a confusion matrix and feature-importance chart, and saves `phishing_detection_model.joblib`.

## Target-label note
The notebook supports the common UCI encoding `-1 = phishing`, `1 = legitimate`, and binary exports using `1 = phishing`, `0 = legitimate`. Verify the labels in the exact dataset version you download before interpreting results.

## Ethical and safety note
Use this project for education and defensive security research. Predictions can be wrong. Do not use the output as the only basis for deciding whether to trust a website.
