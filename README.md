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

With the use of Python, Pandas, ETL process and code refactoring we wanted to write functions that will read the files and gives 3 seperate dataframes.
Wikipedia Data

![image](https://user-images.githubusercontent.com/94253815/150708002-5cffabad-692b-4f29-8d88-c92169f01c5f.png)

Kaggle Metadata 

![image](https://user-images.githubusercontent.com/94253815/150708065-c42f6dd6-33f7-4a84-83b5-231b7c184888.png)

ratings Data frame

![image](https://user-images.githubusercontent.com/94253815/150708117-d7bfc7ba-385d-4b62-9000-923a26b2bfb1.png)

## Extract and Transform the Wikipedia Data
This will continue our use of Python, Pandas, the ETL process and code refactoring, we'll merge the Wikipedia data with Kaggle data. We'll also use the "try- except" block to catch any errors.

Wiki_movies_df
![image](https://user-images.githubusercontent.com/94253815/150708603-23ff911c-eda1-4304-938c-a0fc3901ce1c.png)

Data Frame List

![image](https://user-images.githubusercontent.com/94253815/150708754-0f02732a-4298-4793-999f-4992bf680240.png)


## Extract and Transform the Kaggle Data

Here we extracted and transformed Kaggle Metadata and Movielens rating data, converted into dataframes.  We'll create 2 data frames.  the 1st will consist of Kaggle metadata Dataframe and the Wikipedia movies DataFrame and will create a DataFrame called "movies_df".  Finally, we'll combine the movies_df with MovieLens rating DataFrame to create "movies_with_ratings_df

movies_with_ratings_df

![image](https://user-images.githubusercontent.com/94253815/150709423-43a6782f-0920-4e79-abaa-8b00325fef42.png)


movies_df

![image](https://user-images.githubusercontent.com/94253815/150709347-2e6f5c26-f79d-42a4-90fa-92499ac64fc0.png)

## Final Deliverable - To create the Movie data base
Once we have created the movies_df, we'll use that, along with MovieLens CSV data, and load into a SQL data base.  Once we quered the information, we came back with two results. We created two tables, a movie table and a ratings table.  While the files are too large to view, we were able to get the number of rows per table  We confirmed the total rows in the movie table was 6052 and the ratings table returned 37,024,289.

Movie Table:

![image](https://user-images.githubusercontent.com/94253815/150709983-5c44900c-7d76-423c-b1ed-e5a47a673ac6.png)

Ratings table:

![image](https://user-images.githubusercontent.com/94253815/150710032-7e563e83-9615-401e-9c85-f0b9ec333e05.png)

