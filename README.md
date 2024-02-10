# nosql-challenge
In this NOSQL-chalenge we evaluated some of the ratings data to help UK's journalists and food critics decide where to focus future articles.

Part 1.
1. Database and Jupyter Notebook Set Up.
2. Using NoSQL_setup_starter.ipynb for this section.
3. Imported database uk_food and the collection establishments by using Terminal: mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json.
4. Within notebook, imported the libraries: PyMongo and Pretty Print (pprint).
5.Created an instance of the Mongo Client.
6. Confirm that the database loaded the data properly.
7. List the databases I have in MongoDB. Confirmed that uk_food is listed.
8. Listed the collection(s) in the database to ensure that establishments is there.
9. Found and displayed one document in the establishments collection.
10. Assigned the establishments collection to a variable to prepare the collection for use.

Part 2: Update the Database
1. Made the  changes to the establishments collection by adding restaurant "Penang Flavours" to the database.
2. Found the BusinessTypeID for "Restaurant/Cafe/Canteen" and returned only the BusinessTypeID and BusinessType fields.
3. Updated the new restaurant with the BusinessTypeID that found.
4. Checked how many documents contain the 'Dover' Local Authority in order to remove any establishments within the Dover Local Authority from the database, and checked the number of documents to ensure they were deleted.
5. Converted some of the number values from strings, to numbers.
6. Changed the data type from String to Decimal for longitude, latitude using update_many.
7. Change the data type from String to Integer for RatingValu using update_many.

Part 3: Exploratory Analysis
This analysis will help Eat Safe, Love  find the locations they wish to visit ( restaurants with a hygiene score of 20) and avoid (restaurants with a hygiene score of 0).
1. Using NoSQL_analysis_starter.ipynb .
2. Found the establishments with a hygiene score of 20. There is 41 
3.Converted the result to a Pandas DataFrame.
4.Found the establishments with London as the Local Authority and has a RatingValue greater than or equal to 4.
5. Counted results 33.
6.Converted the result to a Pandas DataFrame.
7. Found the top 5 establishments with a RatingValue rating value of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
8.Foud how many establishments in each Local Authority area have a hygiene score of 0. 
9. There are 55 restaurants with hygiene score of 0.
10. Converted the result to a Pandas DataFrame.

This analysis will help Eat Safe, Love  find the locations they wish to visit and avoid.


