[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/H9e3WTsM)


------------------------------------------------------------------------------

## London House Price Prediction
=========================

### Executive Summary
Housing properties have many attributes that can greatly influence their price such as location, number of rooms and more. This project aims to leverage the patterns presented by these attributes using machine learning methods to accurately predict London house prices. Accurate predictions are important for helping buyers, sellers, and investors better understand property values in a dynamic market.

### Impact of Solution
The final model’s predictions can serve as useful heuristics for property pricing, offering quick, data-driven estimates to support decision-making. This will assist people working in the real estate industry, such as agents, developers, and financial advisors, by providing an additional tool for assessing property values. It will also help potential buyers and sellers better understand market trends and set more informed price expectations.

### Proposed Solution
- Linear modelling:
    - Linear regression
    - Ridge regression
- Non-linear modelling:
    - Decision Tree regressor
    - Random forest regressor

After implementing each model, analysis and evaluation will be carried out to assess its effectiveness. This will provide insights into which model should be used next and what adjustments to the process may be needed to improve results.

### Dataset description
Refer to '01-data-loading-cleaning' notebook for further details on the dataset.

Link for access to original dataset:
https://www.kaggle.com/datasets/jakewright/house-price-data

### Organization

#### Repository 

* `data` 
    Link: https://drive.google.com/drive/folders/1fV7q2s92QuqNteQTlNvH_qrSzXcF6NrC

* `model`
    - final_model.pkl
    (Saved in notebook folder)

* `notebooks`
    - 01-data-loading-cleaning
    - 02-eda
    - 03-pre-processing
    - 04-linear-modelling
    - 05-non-linear-modelling

* `docs`
    - Contains Sprint presentation PDFs

* `src`
    - Contains the project source code (refactored from the notebooks)

* `.gitignore`
    - Part of Git, includes files and folders to be ignored by Git version control

* `conda.yml`
    - Conda environment specification

* `Makefile`
    - Automation script for the project

* `README.md`
    - Project landing page (this page)

* `LICENSE`
    - Project license

#### Final Conclusion
The best performing model was the Decision Tree Regressor achieving the highest accuracy and the best generalisation to the data. Refer to '05-non-linear-modelling' notebook for further details. 

------------------------------------------------------------------------------