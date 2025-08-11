# Text Classification for Life Sciences Applications




## Introduction

In this case study, we develop a classification pipeline to automatically determine whether SAP Fiori apps are relevant to the life sciences domain.

**Problem Statement**  
We are working with a catalog of 14,145 SAP Fiori apps, each described by 25 metadata fields (e.g. titles, descriptions, roles). The dataset is ***entirely unlabeled***, so we must manually annotate a small subset to train a classifier. Operating under ***low-resource conditions*** with only a few hundred labeled examples; we aim to build a model that can generalize effectively across the full catalog.


## Objectives
1. **Manual annotation**: Create a labeled dataset by manually tagging a representative sample of SAP Fiori apps as Relevant or Irrelevant to the life sciences domain.

2. **Model development**: Train interpretable classifiers, such as logistic regression and embedding-based models, to predict relevance based on app metadata.

3. **Evaluation & insights**: Assess model performance using metrics like accuracy, precision, recall, and F1-score. Analyze feature importances and embedding spaces to gain insights into model behavior and decision boundaries.

## Notebook structure
<div style="display: flex; align-items: center; gap: 10px;">
  <a href="https://github.com/alikhalajii/text-classification-life-sciences/blob/master/notebooks/01-data-cleaning.ipynb" target="_blank">1. Data cleaning</a>
  
  <a target="_blank" href="https://colab.research.google.com/github/alikhalajii/text-classification-life-sciences/blob/master/notebooks/01-data-cleaning.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
</div>


<div style="display: flex; align-items: center; gap: 10px;">
  <a href="https://github.com/alikhalajii/text-classification-life-sciences/blob/master/notebooks/02-exploratory-data-analysis-data-labeling.ipynb" target="_blank">2. Exploratory Data Analysis & Data Labeling</a>
  
  <a target="_blank" href="https://colab.research.google.com/github/alikhalajii/text-classification-life-sciences/blob/master/notebooks/02-exploratory-data-analysis-data-labeling.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
</div>

<div style="display: flex; align-items: center; gap: 10px;">
  <a href="https://github.com/alikhalajii/text-classification-life-sciences/blob/master/notebooks/03-feature-engineering.ipynb" target="_blank">3. Feature Engineering</a>
  
  <a target="_blank" href="https://colab.research.google.com/github/alikhalajii/text-classification-life-sciences/blob/master/notebooks/03-feature-engineering.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
</div>

<div style="display: flex; align-items: center; gap: 10px;">
  <a href="https://github.com/alikhalajii/text-classification-life-sciences/blob/master/notebooks/04-traning-baseline-models.ipynb" target="_blank">4. Baseline Models (LR-RF) Trainig & Evaluation</a>
  
  <a target="_blank" href="https://colab.research.google.com/github/alikhalajii/text-classification-life-sciences/blob/master/notebooks/05-training-embedding-models.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
</div>

<div style="display: flex; align-items: center; gap: 10px;">
  <a href="https://github.com/alikhalajii/text-classification-life-sciences/blob/master/notebooks/05-training-embedding-models.ipynb" target="_blank">5. Embedding-based Classification (Word2vec, fastText, SBERT)  
  </a>
  
  <a target="_blank" href="https://colab.research.google.com/github/alikhalajii/text-classification-life-sciences/blob/master/notebooks/05-training-embedding-models.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
</div>

<div style="display: flex; align-items: center; gap: 10px;">
  <a href="https://github.com/alikhalajii/text-classification-life-sciences/blob/master/notebooks/06-ensemble-full-dataset-prediction.ipynb" target="_blank">6. Ensemble & Full-Dataset Prediction)  
  </a>
  
  <a target="_blank" href="https://colab.research.google.com/github/alikhalajii/text-classification-life-sciences/blob/master/notebooks/06-ensemble-full-dataset-prediction.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
</div>

---

## Environment Setup

Follow these steps to recreate the full analysis from scratch:


**Create and activate a clean virtual environment**

```bash
python3.12 -m venv .venv_gxp
source .venv_gxp/bin/activate
pip install -U pip && pip install -r requirements.txt
```


**Note:**
You may safely delete any previously generated sub-directories and still reproduce every result.


## LICENSE

This project is licensed under the [MIT License](./LICENSE).