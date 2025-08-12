[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/H9e3WTsM)


------------------------------------------------------------------------------

## London House Price Prediction
=========================

### Executive Summary
Housing properties possess numerous attributes that significantly influence their market value, including location, number of rooms, and various other structural and environmental factors. This study seeks to model the relationships among these attributes using machine learning techniques to generate precise and well-calibrated estimates of London house prices. Producing robust predictive models can provide valuable insights for buyers, sellers, and investors, facilitating informed decision-making in a dynamic and volatile real estate market.

### Impact of Solution
The final model’s predictions can serve as useful heuristics for property pricing, offering quick, data-driven estimates to support decision-making. This will assist people working in the real estate industry, such as agents, developers, and financial advisors, by providing an additional tool for assessing property values. It will also help potential buyers and sellers better understand market trends and set more informed price expectations.

### Dataset description
This dataset details information about residential properties in London, including location, property characteristics, and energy efficiency. Allowing for effective real estate analysis and property valuation across different areas. 

Link for access to original dataset:
https://www.kaggle.com/datasets/jakewright/house-price-data

### Data cleaning and pre-processing
The data must be cleaned and pre-processed in order to remove null values and redundant information, and to convert categorical or textual data into numerical formats. As machine learning models require clean, structured, and fully numeric input to function effectively.

### Proposed Solution
- Linear modelling:
    - Linear regression
    - Ridge regression
- Non-linear modelling:
    - Decision Tree regressor
    - Random forest regressor

After implementing each model, analysis and evaluation will be carried out to assess its effectiveness. This will provide insights into which model should be used next and what adjustments to the process may be needed to improve results.

### Interpretation

#### Linear modelling
Exploratory data analysis has revealed linear relationships between key features and price. To meet linear model assumptions, some features were omitted. Ridge regression improved performance by reducing overfitting and stabilizing coefficient values.

**Feature importance**

![Ridge Coeff Plot](./images/Ridge%20Coeff.png)

The Ridge regression model coefficients indicate that the model highlights floor area, tenure, and bathrooms as the most important features which influence the value of a property.

**Performance**

![Ridge Residuals](./images/Ridge%20Residuals.png)

The lack of skewness and the concentration of most residuals around zero indicate a good model fit with minimal bias. R^2 score = 0.62. 

#### Non-linear modelling
The models developed in this stage, will prove more insightful and achieve a better prediction score. This is because latitude and longitude can be included here, location plays a significant role in the pricing of properties so results attained from these models will be more insightful and predictive. 

**Feature importance**

![DTR Feature Importance Plot](./images/Tree%20Feat%20Imp.png)

Results attained from Decision Tree Regressor align well with domain expectations and what was uncovered in the exploratory data analysis. With floor area, latitude, longitude, and bathrooms ranked above leasehold tenure and energy rating. The prominence of location variables highlights that property size and location are the primary drivers of value.

**Performance**

![DTR Residuals](./images/Tree%20Residuals.png)

Shows a normal distribution with minimal skewness, indicating a good fit and low bias. Decision Tree Regressor produces consistent predictions with lower error.

#### Final Conclusion
The best performing model was the Decision Tree Regressor achieving the highest predictive score and the best generalisation to the data. Refer to '05-non-linear-modelling' notebook for further details. 

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

* `images`
    - Contains images of plots shown in README file

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


------------------------------------------------------------------------------