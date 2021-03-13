# spotify_etl

**Extract: Spotify API**

I retrieved data out of the Spotify API to get a maximum of 50 of my most recently played tracks. The result of this is a dictionary which I will then take and create multiple dataframes after cleaning it. 

**Transform: Python and Pandas**

I extracted the Spotify data using Python and then transformed the data with the Pandas library. I also performed some basic checks on the data within the code. I checked for any empty data, NULLS, and made sure that there were no duplicates by creating a unique ID per song played through the UNIX timestamp as I cannot play more than one song at the same time.

**Load: Python and Postgresql**

I created a database located on my computer using Postgresql to store all of the Spotify data that is being ingested with this ETL process. I use the pandas method .to_sql to load the data into Postregsql.
