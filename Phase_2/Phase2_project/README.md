# Kings County Housing Bake-off

In our analysis, we were to examine our data about home sales in the Seattle Washington area. We were to understand what factors impact a price homes and develop a model that would be able to predict the prices of a home sold.

Firstly, we used various statistical tests and linear regression to capture the relationship between price and different features. Secondly, we built a model that was able to predict home prices as precisely as possible.


## Inference Part

After our analysis, we came to the conclusion that there are certain features that explain price about 80%. These features included: Zip-Codes, Bedrooms, Seasons, if there was a waterfront, the amount of views, the grade of the home, and the squarefoot living. We also came to the conclusion that the year a home was sold wasn't statistically significant enough to explain price.

## Holdout predictions

We found a prediction model that best predicted the price by using recursive feature elimination and select K best. A subset of the columns we used in the model was 'sqft_living', 'sqft_lot', 'zipcode', 'season', 'age' and 'num_times_sold'. We were to predict a model with an RMSE of less than $200,000 and that was achieved.

## Data Set Information

This data set contains information about houses that were sold in the Seattle area during the last decade. Below is a description of the column names, to help you understand what the data represents. As with most real world data sets, the column names are not perfectly described, so you'll have to do some research or use your best judgment if you have questions relating to what the data means.

Like every data set, there are some irregularities and quirks. Trust me, there wasn't a house sold with 33 bedrooms, even though the data says there was. *You have to decide how you want to handle that example*. Also, some houses were sold more than once within the time frame of this dataset. Think about how that can be useful information in predicting the selling price.

As you go through this modeling process, think about what determines how much someone will pay for a house.  For example, the larger the house is, the more people will pay for it. If you understand why certain houses cost more than others and represent that in your model, it will be a more accurate model.

Have fun!

# Column Names and descriptions for Kings County Data Set
* **id** - unique ID for a house
* **date** - Date day house was sold
* **price** - Price is prediction target
* **bedrooms** - Number of bedrooms
* **bathrooms** - Number of bathrooms
* **sqft_living** - square footage of the home
* **sqft_lot** - square footage of the lot
* **floors** - Total floors (levels) in house
* **waterfront** - Whether house has a view to a waterfront
* **view** - Number of times house has been viewed
* **condition** - How good the condition is (overall)
* **grade** - overall grade given to the housing unit, based on King County grading system
* **sqft_above** - square footage of house (apart from basement)
* **sqft_basement** - square footage of the basement
* **yr_built** - Year when house was built
* **yr_renovated** - Year when house was renovated
* **zipcode** - zip code in which house is located
* **lat** - Latitude coordinate
* **long** - Longitude coordinate
* **sqft_living15** - The square footage of interior housing living space for the nearest 15 neighbors
* **sqft_lot15** - The square footage of the land lots of the nearest 15 neighbors


## GitHub Repository

	├── README.md                                     	<- The top-level README for reviewers of this project
	├── Kings_County_Housing_Version_2.ipynb		<- Main Analysis Includes: Inference & Prediction Models
	├── Predict_holdout.ipynb				<- Main Notebook for final predictions
	├── housing_preds_jason_arikupurathu.csv		<- CSV for final predictions generated from Predict_holdout
	├── data                                              	<- Both sourced externally
		└ kc_house_data_test_features.csv			<- Test set csv
		└ kc_house_data_train.csv 				<- Train set csv
	├── notes                                             	<- Contains old notebooks and project guidelines
	├── presentation-slides                              	<- Contains presentation slides
		└ Slides-KCH-Analysis-Inference.pdf             	<- Presentation Slides
	└── pickled_files                                     	<- Contains Pickled Files
		└ model.pickle                                  	<- Model pickled
		└ other_info.pickle 					<- Information to be passed pickled
