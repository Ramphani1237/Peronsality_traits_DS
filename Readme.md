# Personality Traits Prediction using Machine Learning

## Project Overview
This project predicts the **Big Five Personality Traits** from written text using **Natural Language Processing (NLP)** and **Machine Learning**. Essays are analyzed to determine the presence or absence of each personality trait. Since multiple traits can apply to a single essay, this is a **multi-label classification problem**.

**Personality Traits Predicted:**
- Openness (cOPN)
- Conscientiousness (cCON)
- Extraversion (cEXT)
- Agreeableness (cAGR)
- Neuroticism (cNEU)

---

## Objectives
- Perform exploratory data analysis on textual data
- Convert text into numerical features using TF-IDF
- Train and evaluate multiple machine learning models
- Compare model performance using F1-score
- Store predictions and evaluation results in a structured format

---

## Dataset
- Input: Essays written by individuals
- Output: Binary labels (0 or 1) for each personality trait
- Problem Type: Multi-label text classification

---

## Methodology
1. **Exploratory Data Analysis**
   - Trait distribution analysis
   - Word count statistics
   - Trait correlation analysis

2. **Text Preprocessing**
   - Lowercasing and cleaning
   - Stopword removal
   - TF-IDF vectorization

3. **Model Training**
   - One-vs-Rest multi-label strategy
   - Logistic Regression
   - Linear Support Vector Machine
   - Multinomial Naive Bayes

4. **Evaluation**
   - Metric used: F1-score (per trait)
   - Model-wise performance comparison
   - Results stored as CSV files

---

## Results
Logistic Regression showed the most consistent and balanced performance across all personality traits. Linear SVM performed competitively on high-dimensional TF-IDF features, while Naive Bayes served as a fast baseline model.

---

## Limitations
- Personality labels are subjective
- Class imbalance across traits
- TF-IDF does not capture semantic context
- Traits are predicted independently despite correlations

---

## Project Structure
```
Personality_traits_DS/

assets/
    raw/
        essaytrain.csv
    processed/
        predictions_step5.csv
    plots/
        cAGR_bar_counts.png
        cAGR_pie_percent.png
        cCON_bar_counts.png
        cCON_pie_percent.png
        cEXT_bar_counts.png
        cEXT_pie_percent.png
        cNEU_bar_counts.png
        cNEU_pie_percent.png
        cOPN_bar_counts.png
        cOPN_pie_percent.png
        traits_correlation_heatmap.png
    results/
        confusion_matrix_cAGR.png
        confusion_matrix_cCON.png
        confusion_matrix_cEXT.png
        confusion_matrix_cNEU.png
        confusion_matrix_cOPN.png
        f1_scores_per_trait.png
        f1_scores_summary.csv
        model_comparison_f1_scores.csv

notebooks/
    00_project_overview.ipynb
    01_data_overview.ipynb
    02_EDA.ipynb
    03_feature_engineering_and_data_preparation.ipynb
    04_Model_building.ipynb
    05_results_analysis_and_visualization.ipynb
    06_multiple_models_analysis.ipynb
    07_project_finalisation.ipynb
```
---

## Tools and Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## Conclusion
This project demonstrates an end-to-end data science workflow, including NLP preprocessing, multi-label classification, model evaluation, and result management. It serves as a strong foundational project for applied machine learning and text analytics.

---

## Author
Ramphani 

---
