# High Performance Employee Resign Prediction

## Summary

High performance employee resign prediction using graphs (with node embeddings) and supervised learning. This data was taken from Indra Hackday 2024 - People Analytics. The winner from this competiton had 0.5614 F1 score on test data. Applying various techniques such as graph embeddings and Feature Engineering we were able to get 0.6106 F1 score using XGBoost Classifier.

Applying a dimensionality reduction technique named Recursive Feature Extraction with the XGBoost Classifier, the number of features (no node embeddings features included) was reduced from 50+ to only 21, finding that employee's seniority and the interaction between employee and boss gender are the most important features to predict the early resignation of an employee with high performance.

**Key insights:** Employee gender, boss gender, employee performance and seniority were the features that influence the most in the early employee resign.

# Introduction

Employee early resign may have considerable consequences for the business, such as time and money invested in training, make a new for the position which implies time and resources from HHRR, etc. Knowing the motives that make employees to early resing can be a great advantage for business in order to save time, money and resources.

In this project, it's primordial to find those features that influence the most in employee resing, helping the business to take actions to prevent this phenomena.

# Business objectives

**Main objective:** Identify the reasons that make employees to resign in their first 6 months.

**Secondary objectives:** Take actions to prevent early resign from employees.

### Author

William Pabon, Data Scientist

[LinkedIn](https://www.linkedin.com/in/william-ferney-pabon-grimaldi-026846236/)

## Project Organization

    ├── LICENSE
    ├── tasks.py           <- Invoke with commands like `notebook`.
    ├── README.md          <- The top-level README for developers using this project.
    ├── install.md         <- Detailed instructions to set up this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries.
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures         <- Generated graphics and figures to be used in reporting.
    │
    ├── environment.yml    <- The requirements file for reproducing the analysis environment.
    │
    ├── .here              <- File that will stop the search if none of the other criteria
    │                         apply when searching head of project.
    │
    ├── setup.py           <- Makes project pip installable (pip install -e .)
    │                         so high_performance_employee_resign_prediction can be imported.
    │
    └── high_performance_employee_resign_prediction               <- Source code for use in this project.
        ├── __init__.py    <- Makes high_performance_employee_resign_prediction a Python module.
        │
        ├── data           <- Scripts to download or generate data.
        │   └── make_dataset.py
        │
        ├── features       <- Scripts to turn raw data into features for modeling.
        │   └── build_features.py
        │
        ├── models         <- Scripts to train models and then use trained models to make
        │   │                 predictions.
        │   ├── predict_model.py
        │   └── train_model.py
        │
        ├── utils          <- Scripts to help with common tasks.
            └── paths.py   <- Helper functions to relative file referencing across project.
        │
        └── visualization  <- Scripts to create exploratory and results oriented visualizations.
            └── visualize.py

---
Project based on the [cookiecutter conda data science project template](https://github.com/Wiferpagri/cookiecutter-data-science-personal).