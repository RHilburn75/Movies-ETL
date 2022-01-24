# Movies-ETL
## Overview
Amazing Prime wants to tkeep the dataset updated on a daily basis. We need to create an automated pipleline that will receive data, make the nessesary changes and then loads the data into tables, to make it easier to read.  We'll use 3 files in order to do this:
1. Wikipedia Data
2. Kaggle Data
3. MovieLens data
We'll perform the ETL process and use PostgreSQL database to help with our data analysis.  We'll breakdown each segment into sections:
1. We'll write an ETL Function to read the the three data files
2. Extract and Transform the Wikipedia Data
3. Extract and Transform the Kaggle Data
4. Our final deliverable will be to create the movie base

## The 3 Data files
Wikipedia Data

![image](https://user-images.githubusercontent.com/94253815/150708002-5cffabad-692b-4f29-8d88-c92169f01c5f.png)

Kaggle Metadata 

![image](https://user-images.githubusercontent.com/94253815/150708065-c42f6dd6-33f7-4a84-83b5-231b7c184888.png)

ratings Data frame



