# deep-learning-challenge

Report on the Neural Network Model

Overview : The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. From Alphabet Soup’s business team, we have CSV files containing more than 34,000 organizations that have received funding from Alphabet Soup. Within this dataset are a number of columns that capture metadata about each organization, such as:
•	EIN and NAME—Identification columns
•	APPLICATION_TYPE—Alphabet Soup application type
•	AFFILIATION—Affiliated sector of industry
•	CLASSIFICATION—Government organization classification
•	USE_CASE—Use case for funding
•	ORGANIZATION—Organization type
•	STATUS—Active status
•	INCOME_AMT—Income classification
•	SPECIAL_CONSIDERATIONS—Special considerations for application
•	ASK_AMT—Funding amount requested
•	IS_SUCCESSFUL—Was the money used effectively

Data Preprocessing: Data is preprocessed by:
•	Dropping columns not beneficial.
•	Cutoff values is chosen and list is created.
•	Categorial data to numeric with pd.get_dummies.
•	Splitting preprocessed data into features and target arrays.
•	Get training and testing dataset.
•	Scale the data using StandardScaler.
•	Deep neural net- the number of input features and hidden nodes for each layer.
•	Model is compiled and trained.
•	Evaluate the model using test data.
•	Export model as HDF5 file.

Compiling, Training, and Evaluating the Model: The model is designed and accuracy of model is adjusted from 72% to more than 75%. Model is compiled with parameter of loss, optimizer and metrics. After compiling model, it is trained with epochs value. Lastly, model is evaluated using test data and accuracy is found.

In first Model Design:
	EIN and NAME is dropped. 2 hidden input layers are made with values 10 and 5 and activation unit is “relu” and output layer is “sigmoid”. Epochs value as 100. Accuracy of this model is around 72%.

In Second Model Design:
	EIN and NAME is dropped. 2 hidden input layers are made with values 30 and 10 and activation unit is “relu” and output layer is “sigmoid”. Epochs value as 200. Accuracy of this model is around 73%.

In Final Model Design:
	EIN column is dropped. 3 hidden input layers are made with values 10, 8 and 6 and activation unit is “relu” and “sigmoid” and activation output layer is “sigmoid”. Epochs value as 30. Accuracy of this model is around 76%.

Summary: In 3 designs, the model accuracy increased from 72% to 76%. Total layers used in these models is from 2 to 3 hidden input layers with activation units as relu and sigmoid. 

3 code:

First model design - Starter_Code.ipynb
Second model design - AlphabetSoupCharity_Optimization.ipynb
Third model design - AlphabetSoupCharity_Optimization_final.ipynb
