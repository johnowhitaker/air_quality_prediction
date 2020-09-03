# air_quality_prediction
Predicting historical air quality based on satellite data

Report: https://docs.google.com/document/d/1e1y-hwduVXcDYs8KxxoGSrK_LI5mCOpe-7WY_QkcdoI/edit?usp=sharing

Dashboard to view results: http://www.datasciencecastnet.com/airq/

### Accessing Predictions

The predictions can be found in the Data/results folder.
- za_cities_predictions contains the predictions for cities across South Africa
- pcs_predictions contains predictions for some additional population centers in South Africa
- af_cities_predicitons contains the predictions for major cities across Africa

### Replicating the project:

- Download the historical air quality measurements from https://aqicn.org/data-platform/covid19/ and store the files in Data/waqi_downloads 
- Run '1. WAQI Data Prep.ipynb' to merge the relevant data into a single csv file, which is stored in Data/intermediate/citypm25.csv
- Run '2. Fetch GEE Data.ipynb'. You can optionally downlaod the same input data for new locations as well, to make predicitons for later.
- Run '3. Modelling and Evaluation.ipynb'. This loads the training data, trains and evaluates a model and saves predictions.

If you'd rather just use the trained model, you can do this by following '4. Making Predictions for New Locations' which shows how to use the trained model to make predictions given a set of locations you're interested in. It goes through all the steps needed, from downloading the data from GEE to saving and displaying your predictions.


