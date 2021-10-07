# neuralnet_energydata

A repository on building a neural network to forecast the wholesale electricity prices for Belgian Electricity market by including the generation data from wind and solar energies under the management of Belpex.

This project was done under the guidance of Prof.Geert Deconinck as part of the Smart Distribution Systems(B-KUL-H00P3A) course at KU Leuven, Belgium.

By the end of this project, I intend to finish the following deliverables.

•	Set up a machine learning environment in Google Colab.
•	Implementing and training a 2-layer neural network using tensorflow, keras.
•	Using this neural network to make prediction about the wholesale electricity prices. 



## Project Flow


This project is mainly divided in three different parts. 

1. Data Import & analysis
2. Neural Network development and training
3. Data forecasting and insights

### Data Import & Analysis

We have the necessary data in the form of .csv files. The primary step after importing all the required Python libraries to the environment is uploading these datasets to Google Colab. 

We first import the uploaded into **Pandas Dataframe**. We are only interested in two columns of the whole csv file, the date and the Load factor for the solar, wind datasets and prices for the Belpex dataset. 

Visualizing the dataframes, we understand that the data is in time series format, but the datasets have different time intervals. Apart from this we also observe some missing values in the Belpex and NaN (Not a Number) values in the solar, wind datasets. Before going to the next steps in the project, we must address these issues and visualize the data to check its readiness for the neural network model. 
