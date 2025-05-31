# Kepler - Exoplanets Disposition Machine Learning Prediction

The goal of this project is to determine weather a Kepler Objects of Interest (KOI) discovered by the Kepler Space Telescope can be predicted as confirmed, false positive, and candidate by using various features taken at the time.

## Data Collection
This dataset was produced from the NASA Exoplanet Archive. Which is an open-source API for various Exoplanet related science.
http://exoplanetarchive.ipac.caltech.edu
A data frame with 49 columns was created.

## Data Analysis and Feature Engineering
Label encoding was used for the remaining categorical features and correlation between the features and target be to predict (koi_disposition) were found.

## Machine Learning
The first model used was Random Forest Classification with all numerical features. This produced a respectable accuracy of 93%.
An SMV Model was then used which produced an accuracy of 87%.
Finally, a second Random Forest Classification with only the top features was used which produced a resulting accuracy of 90%.

## Predictions
Due to the quantity of features needed for a prediction with the original data frame, the decision was made to use the Random Forest Classification model with less features as a predictor. The model successfully predicted koi_disposition using selected data.
