# sqlalchemy-challenge    
## Part 1: Analyzing and Exploring the Climate Data <br />       
In this section, I used Python and SQLAlchemy to do a basic climate analysis and data exploration of your climate database. Specifically, I used SQLAlchemy ORM queries, Pandas, and Matplotlib. To do so, I completed the following steps:

1. Use the SQLAlchemy create_engine() function to connect to your SQLite database. 

2. Use the SQLAlchemy automap_base() function to reflect your tables into classes, and then save references to the classes named station and measurement.

3. Link Python to the database by creating a SQLAlchemy session.
 
![image](https://github.com/dclaxto1/sqlalchemy-challenge/assets/128431134/d3427b3f-a1db-4156-826d-c883565ecddf)
 

Perform a precipitation analysis and then a station analysis by completing the steps in the following two subsections.  

### Precipitation Analysis
Find the most recent date in the dataset.

Using that date, get the previous 12 months of precipitation data by querying the previous 12 months of data.
![image](https://github.com/dclaxto1/sqlalchemy-challenge/assets/128431134/db5bb81e-a624-4220-ad3c-428f5d297e49)

Loaded the query results into a Pandas DataFrame. Explicitly set the column names.

Sort the DataFrame values by "date".

Use Pandas to print the summary statistics for the precipitation data.
![image](https://github.com/dclaxto1/sqlalchemy-challenge/assets/128431134/13f51128-c648-4f7a-a295-b1b773309575)

![image](https://github.com/dclaxto1/sqlalchemy-challenge/assets/128431134/7ec0e1aa-33b7-4c14-b08c-f7a6c77466e4)


### Station Analysis
Design a query to calculate the total number of stations in the dataset.
![image](https://github.com/dclaxto1/sqlalchemy-challenge/assets/128431134/775571c6-26dc-4a46-9776-81d561bb311e)  

Design a query to find the most-active stations (that is, the stations that have the most rows). List the stations and observation counts in descending order. <br />
![image](https://github.com/dclaxto1/sqlalchemy-challenge/assets/128431134/8b2fd16e-9ab5-4d9b-802a-271a79d5a0cb)



Design a query that calculates the lowest, highest, and average temperatures that filters on the most-active station id found in the previous query.<br />

![image](https://github.com/dclaxto1/sqlalchemy-challenge/assets/128431134/d1b69d07-cd99-49cc-9453-0dbcf525c62d)

Design a query to get the previous 12 months of temperature observation (TOBS) data. To do so, complete the following steps:

Filter by the station that has the greatest number of observations.

Query the previous 12 months of TOBS data for that station.
![image](https://github.com/dclaxto1/sqlalchemy-challenge/assets/128431134/6925131f-2126-415f-b19c-c12120df136a)
