# Crop-Classification-using-Sentinel-2
# Notebook Workflow
01-Pre-processing-read image file from sentinel 2 and then we put it to code the custom cloud index and we crop the picture from the image by selecting the index that is less than 1.5
02-create-feature-write function to calculate the function called index stack which use to calculate the vegetation indices based on spectral bands. For each vegetation index, we calculate the mean across time. We used 7 different vegetation indices which are NDVI, NDWI, GCI, SAVI, EVI, VARI, and GNDVI.
03-modeling-binary -We use a model with machine learning primary on random forest classification and hyperparameter selection using cross-validation.
4 we have included visualization using matplotlib to show how our machine learning predicts the test data
# Overview
Arv hackathon has given us a satellite image to work on a crop classification in Thailand for the 2 years in 2020 and 2021 our main goal is to improve agricultural growth and improving food security. Collecting accurate data is crucial to training these models.
This project is a stepping stone to more advanced predictions such as crop yield prediction and predicted food security under future climate change scenarios.
# Goals
The objective of this project is to create a classification model to identify crops using sentinel-2 satellite imagery. The result will be a map of classified fields
# Data 
The fields in the training set are in Thailand around the country.
There are 4 crop types present in the fields:
1. Cassava
2. Rice
3. Maize
4. Sugarcane
# Files included in the dataset:
label_description: Lists of all the unique crops and their Crop IDs
Train.zip: shapefile containing all of the fields in the training dataset. This is the dataset that we will use to train model
test.zip: shapefile containing all of the fields in the test dataset.
Result_from_data.csv: the file that will show the prediction of all the test datasets that we will predict the crop
data_all.csv: the file containing the veg index of all the crops and index that can be used to train the model
Satellite image These are Sentinel-2 satellite data captured on the data indicated in the file name. These files are in SENTINEL-SAFE format, including image data in jp2 format
