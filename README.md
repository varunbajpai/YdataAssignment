Files Description

1) DataProcessing.ipynb : Data Preprocessing steps, when executed independtally produces a file data.csv
2) Train.ipynb : File used to train the data.csv file 
3) Test.ipynb : Testing the model trained by Train file
4) requirements.txt : list of requirements for the project


All files are independent of each other: 


Order of execution is as follows

pip install -r requirements.txt : First install all the dependencies using the command
DataPreprocessing.ipynb
Train.ipynb
Test.ipynb

The path for raw data is set to : Data Challenge/California_SO2_Measures.csv


About:
In order to predict the So2 levels across the state of california i took average of S02 levels across all the dates
Dates in this case acts as primary key for data agrregation
Dates are then changed to Day Wise Categorical Variables: Rational behind this step : S02 levels are higher on weekdays as compared tto weekends
Continuous Variables are Mean Normalized

Variables which have same value such as units or name of county and Longitude latitude are ignored
If we want to deal with each county seperately: the underlying architetcture remains same but additional feature of Location Detail can be added on