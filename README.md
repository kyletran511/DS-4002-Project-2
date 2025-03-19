# DS4002 Project 2: Anomaly Detection of Parking Ticket Issuance in Charlottesville Between 1999 and 2025

This project aims to perform an anomaly detectection on a parking ticket dataset issued by the City of Charlottesville between the years 1999 and 2025 in order to identify factors that influence the frequescy of parking tickets issued at a given time. 

## Section 1: 
We used the Isolation Forest Model to identify the anomalies (outliers) in our dataset.


## Section 2

📦 Project_Name
│-- 📂 DATA        
│-- 📂 SCRIPTS    
│-- 📂 OUTPUT      
│-- 📜 README.md    
│-- 📜 LICENSE      

## Section 3: 
1. Preprocess the Data
  a. Download data from City of Charlottesville website
  b. Remove irrelevant columns and null entries
  c. Remove whitespace from string columns & uppercase strings for uniform formatting
  d. Clean entries with multiple street names that are the same
  e. Filter entries to be tickets issued in 2025 or earlier (for date validity)
  f. Remove entries that have the same Ticket Number since this should be unique
  g. Convert the DateIssued and TimeIssued features into datetime objects
  h. Remove entries with invalid state abbreviations 

2. Preparing Features + Feature Engineering
  a. In preparation for model analysis, feature engineering will be done
  b. More specifically:
    i. We plan to normalize the numerical features and autoencode the categorical variables so the model can better interpret those features
    ii. We may also create new features such as the day of the week the ticket was issued so the model can better interpret the data
   
3. Anomaly Detection Analysis
  a. After preparation of features and feature engineering, we will build one model. For the Isolation Forest model, we used the scikit-learn library
  b. After building the model, we will finetune the models based on the hyperparameter:
    i. For Isolation Forest, this includes the contamination parameter, which represents the expected portion of anomalies in the data
    ii. We evaluated the model using metrics of Recall, Precision, and F1-Score
   
4. Hypothesis Testing
  a. After fine tuning the model, we will evaluate whether the model can identify anomalies with a significant difference by performing a two-sample t-test
  More specifically, we will calculate the frequency rate of tickets issued in normal and anomaly periods and compare them using a t-test
  If p-value < 0.05, anomalies are statistically different (reject H₀).
  If p-value > 0.05, no strong evidence of meaningful anomalies (fail to reject H₀).

