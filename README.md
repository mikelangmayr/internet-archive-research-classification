# Internet Archive Research Classification

This project builds a machine learning pipeline to classify academic and research-related documents sourced from the [Internet Archive](https://archive.org/). It includes stages for downloading raw data, processing and engineering features, training classifiers, and analyzing model results using advanced statistical tools.

## 📂 Project Structure

The core of the project is organized into four Jupyter notebooks:

1. **Download_and_Organize_files.ipynb**
   - Downloads HTML and PDF documents from sources like FatCat and GWB
   - Extracts and stores structured metadata
   - Handles encoding issues, language detection, and multiprocessing

2. **Pipeline_and_Feature_Engineering.ipynb**
   - Parses text from documents
   - Extracts lexical, structural, and contextual features
   - Supports tokenization, translation, and domain extraction

3. **Modelling_and_Evaluation.ipynb**
   - Trains classifiers (e.g., SVM, Random Forest, XGBoost, LDA/QDA)
   - Performs hyperparameter tuning with GridSearchCV
   - Evaluates models using confusion matrices, accuracy, and cross-validation

4. **BMA_Analysis.ipynb**
   - Applies Bayesian Model Averaging (using PyMC3) for deeper evaluation
   - Visualizes uncertainty and feature contributions
   - Summarizes statistical insights with ArviZ

## 🛠️ Setup Instructions

### Install Dependencies

#### Create a virtual environment and install dependencies using:

```bash
pip install -r requirements.txt
```

#### Launch the Notebooks:
```bash
jupyter notebook
```

### Run the notebooks in the following order for full functionality:

    - Download_and_Organize_files.ipynb

    - Pipeline_and_Feature_Engineering.ipynb

    - Modelling_and_Evaluation.ipynb

    - BMA_Analysis.ipynb

## 📌 Dependencies

    - pandas, numpy, matplotlib, seaborn

    - scikit-learn, xgboost, statsmodels

    - nltk, langdetect, tldextract

    - pymc3, arviz, theano
    
    - bs4, pdfminer.six, requests, ftfy, selectolax
    
    - google_trans_new, mtranslate

See requirements.txt for details.

## 👥 Authors
   - John McNulty
   - Sarai Alvarez
   - Michael Langmayr

## 📊 Features Used

    - Text structure and formatting patterns (e.g., word count, punctuation)
      Language detection and translation

    - Metadata such as URL domains

    - Statistical modeling with PyMC3 and Bayesian averaging

## 📘 License

This project is licensed under the MIT License.

