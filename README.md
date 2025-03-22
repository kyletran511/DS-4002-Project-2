# DS4002 Project 2: Anomaly Detection of Parking Ticket Issuance in Charlottesville Between 1999 and 2025

## Overview:
This project aims to perform an anomaly detectection on a parking ticket dataset issued by the City of Charlottesville between the years 1999 and 2025 in order to identify factors that influence the frequency of parking tickets issued at a given time. 

## Software and Platform Used
Python was used for data processing, analysis, and visualization.
some of the packages we used: 
- pandas – For data manipulation and preprocessing.
- matplotlib & seaborn – For data visualization.
- Isolation Forest (from scikit-learn) – For anomaly detection
- ttest_ind - For statistical analysis (Mann Whitney U test)

The platform used for development was Google Colab via a juptyer notebook

## Documentation Map

📦 DS 4002 Project 2

```
│── 📂 DATA 
    ├── Data Appendix.pdf 
    ├── 📂 analyzed_data 
      ├── cleaned_parking_tickets.zip
      ├── trained_data.zip     
    ├── 📂 initial_data 
      ├── Parking_Tickets_Original.csv.zip 
│── 📂 OUTPUT
   ├── 📂Plots
      ├── Heatmap of tickets issued by location.png
      ├── Heatmap of tickets issued by hour and day of the week.png
      ├── Number of tickets issued over time.png
      ├── Number of tickets issued per year.png
      ├── Percentage of tickets issued by day of week.png
      ├── Percentage of tickets issued by season.png
│── 📂 SCRIPTS
    ├── DS 4002 Project 2.ipynb
│── LICENSE 
│── README.md     
```     
## Section 3: Instructions for Reproducing Results
To reproduce the results of this study, follow the steps below:

### **1. Clone the Repository**
First, clone this repository to your local machine. In order to that, run this command
```
git clone https://github.com/kyletran511/DS-4002-Project-2.git
```
### **2. Run the Script**
- Go to the SCRIPTS directory and find the DS 4002 Project 2.ipynb
- After finding the jupyter notebook, you can simply run it to reproduce all the results of this project
- There are comments throughout the script to describe how the code works
```
│── 📂 SCRIPTS
    ├── DS 4002 Project 2.ipynb
```
