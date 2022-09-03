# Background
Alphabet Soup wants to develop a tool that can help with selecting  applicants for funding that have the best chance of success in their ventures. In this project data from Alphabet Soup was used to train a  nueral network model that can to help identify funding applicants that have the best chance of succeeding.


To build the model a CSV file containing more than 34,000 organizations that have received funding from Alphabet Soup over the years was used. Within this dataset are a number of columns that capture metadata about each organization, such as:

* **EIN** and **NAME**—Identification columns
* **APPLICATION_TYPE**—Alphabet Soup application type
* **AFFILIATION**—Affiliated sector of industry
* **CLASSIFICATION**—Government organization classification
* **USE_CASE**—Use case for funding
* **ORGANIZATION**—Organization type
* **STATUS**—Active status
* **INCOME_AMT**—Income classification
* **SPECIAL_CONSIDERATIONS**—Special consideration for application
* **ASK_AMT**—Funding amount requested
* **IS_SUCCESSFUL**—Was the money used effectively
* 
# Step 1: Preprocess the Data
The following steps were taken to clean up the data and suitable for analysi
EIN and NAME columns were removed to from the dataset as they where not relevant to the analysis
 ![image](https://github.com/mayooks/Alphabet-Soup-Funding-Success-Prediction-Model/blob/main/Images/Picture%2033.png)

The data had no rows with Null values as confirmed by the  code below.
![image](https://github.com/mayooks/Alphabet-Soup-Funding-Success-Prediction-Model/blob/main/Images/Picture%201-second.png)

The code below indicated that the data had duplicated columns. However on close inspection it appeared that different organisation with similar profiles were flagged as duplicates. Therefore it was decided not to delete the columns that were flagged as duplicates.
![image](https://github.com/mayooks/Alphabet-Soup-Funding-Success-Prediction-Model/blob/main/Images/Picture%202.png)

The number of unique values and data types in each column were determined using the nunique() and dtypes functions.The IS_SUCCESSFUL column has two integers that were unique making it ideal target variable             ![image](https://user-images.githubusercontent.com/103529769/188283720-adf232a9-43fc-48ef-8f5d-972648e93da8.png)

 
