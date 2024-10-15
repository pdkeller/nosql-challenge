# nosql-challenge
# Author: Paul Keller
# Due Date: October 15, 2024

# The purpose of this project was to create a NoSQL database and perform ETL actions on it. The data set was
# extracted through GitBash and the command to do so is located within the code file. Next, a database variable was
# created, as was one for the only collection within that database. The find_one() function was used to verify the
# success of download. The data set was then transformed by adding a new document using the insert_one() function.
# This document had a field updated using the update_one() function. All local Authorities with the value 'Dover'
# were deleted from the database using the delete_many() function, which only deletes documents. Finally, a query 
# was used to change the fields longitude and latitude to Doubles and the field RatingValue to Int.

# During the next part, a query was used for each of the four tasks. The first two tasks used the queries to 
# create dataframes for the respective data collected. The third query searched for documents whose latitude and 
# longitude fields fell with a small range of values and that matched a RatingValue. This list of results was 
# sorted by Hygiene score in descending order and was limited to five results. This data was too saved to a dataframe.
# The final task used three queries to create a pipeline. These queries were a match query, a group query, and a sort
# query. This aggregated data pipeline returned a list of data that matched Hygiene scores, grouped LocalAuthorityName
# and sorted by count in descending order. This result was then saved to a dataframe.