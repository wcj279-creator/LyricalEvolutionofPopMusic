# LyricalEvolutionofPopMusic
# Lyrical Evolution: A Quantitative Analysis of Pop Music

**Student ID:** WILJEN0825
**Date:** August 17, 2025

---

## Project Overview

This project analyzes a dataset of over 1.6 million English-language pop songs from 1965 to 2015 to explore the evolution of lyrical trends. The primary research question is: **How have the length and sentiment of pop song lyrics changed over time?** A secondary analysis seeks to determine if these features can be used to predict the sentiment of a song.

---

## Summary of Findings

* **Exploratory Data Analysis (EDA):** The number of songs in the dataset trends upwards, peaking in the 2010s. Lyric length shows a wide distribution, with most songs containing between 150 and 350 words.
* **Sentiment Analysis:** Bivariate analysis revealed a slight negative correlation (-0.09) between the year of release and lyrical sentiment, suggesting that lyrics have, on average, become slightly more negative over time.
* **Predictive Modeling:**
    * A baseline **Logistic Regression** model achieved an accuracy of 60.4%, primarily by predicting the majority class (positive sentiment).
    * A **Neural Network** was implemented, also achieving an accuracy of 60.4%. While not outperforming the baseline on accuracy, the model's training curves showed it learned patterns before plateauing. This indicates that `year` and `lyric_length` alone are not strong predictors of sentiment.
* **Scenario Analysis:** Hypothetical scenarios showed that the model predicts a slight increase in negative sentiment for songs with longer lyrics ("Verbose Poet" era) and a very slight increase in positive sentiment for songs from the 1980s ("Nostalgic Revival" era).

---

## Dependencies

To run this project, you will need Python 3 and the following libraries:
* pandas
* numpy
* seaborn
* matplotlib
* pandarallel
* nltk
* vaderSentiment
* tensorflow
* scikit-learn

You can install them using pip:
`pip install pandas numpy seaborn matplotlib pandarallel nltk vaderSentiment tensorflow scikit-learn`

---

## How to Run

1.  Clone this repository.
2.  Ensure all dependencies are installed.
3.  Open and run the `SDC486L_3.2_Project_Jennette.ipynb` Jupyter Notebook. The notebook is structured to load, process, analyze, and model the data sequentially. Note that some cells for data processing may take time to run. Pre-computed CSV files are included to speed up the process.
