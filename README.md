# Sprint Performance Analysis

### Project Overview

This project investigates the relationship between variables, currently wind conditions, and sprint performance, focusing on 100m and 200m.
Using Python, I explored sprint performances, applied statistical analysis and built regression models to investigate how wind speed influences race times.

### Objectives

Explore independent variables of sprint performance.

Investigate the relationship between wind speed and race times.

Apply statistical techniques to quantify the impact of wind conditions.

Visualise relationships and identify patterns in the data.

### Dataset

The dataset used in the notebook file uses a synthetic dataset containing 97 sprint performance records. However my initial analysis used my own sprint dataset
based on real data, which found wind to be a significant predictor of 100m and 200m sprint times.

#### The dataset includes:

Date

Event distance

Time

Location (The specific track)

Wind speed

Competition type (ie, County final, open meeting, club competition, ect)

Mean finishing time of other competitors

Position

Note: Synthetic data is used to protect the privacy of my own racing history.

### Methods 

#### Languages and libraries:

Python

Pandas

NumPy

Matplotlib

Seaborn

Statsmodels

#### Analysis techniques:

Basic Data pre-processing, cleaning and transformation

Ordinary Least Squares (OLS) Linear regression

Model assessment (QQ-plot, residuals vs fitted plot, scale-location plot)

Measuring Outliers (Leverage and Cooks distance)

Logistic regression (to be added)

### How to Run

Create a sprint dataset using the same variables seen under 'Dataset'
Clone this repository.
Install the required libraries seen under 'Methods'
Open ipynb file in Jupyter Notebook.
Run the notebook cells sequentially, replacing the file name to your own dataset, changing the cutoffs to times that would only occur due to injury for you, and
changes to the load_data function based on the datatypes in your dataset.

### Results and Conclusions

With my own, self-collected sprinting dataset I found wind to be a statistically significant predictor of 100m sprint time (P < 0.005, R-squared 0.58),
with only one race (after removing times caused by injury) being a significant outlier based on Cooks Distance. All model assessment graphs suggested wind
is a suitable variable for predicting sprint times. For my dataset, position and mean time of other racers were not signiciant predictors of 100m sprint time.


### Future Improvements

Identify more significant variables for predicting sprint times.
Incorporate multivariate prediction models.
Create a logistic regression model.
Investigate differences between sprint distances.
