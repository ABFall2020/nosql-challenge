# nosql-challenge

# UK Food Standards Agency Data Analysis

## Scenario

Using data obtained from the UK Food Standards Agency, create a NoSQL database in MongoDB, import the data and use the PyMongo module to complete additional tasks.

## Challenge Sections

The challenge is split into three sections:

1. Database and Collection Creation
2. Update Documents and Field Datatypes
3. Exploratory Analysis

### Database and Collection Creation

#### 1. Create the database and import data

- Use the 'mongoimport' function to create a database named 'uk-food' and a collection 'establishments' to import the documents.
```
mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json
```

#### 2. Connection setup and confirmation
Import required libraries in a Jupyter Notebook:
PyMongo
Pretty Print (pprint)
Create an instance of the Mongo Client.
Confirm database creation and data loading:
List the databases and collections.
Display one document from the 'establishments' collection.

#### 3. Prepare collection for use
Assign the 'establishments' collection to a variable for further use.

### Update Documents and Field Datatypes

#### 1. Update documents and fields
Add a new document for a recently opened restaurant.
Find and update the 'BusinessTypeID' for "Restaurant/Cafe/Canteen".
Remove establishments in "Dover" Local Authority.
Convert string number values to integers or decimals.

#### Exploratory Analysis
With the database documents prepared, conduct some exploratory analysis on the database to provide some high-level insights:

For each question, provide the following information:

Count of documents.
Display the first document.
Convert results to a Pandas DataFrame and display.

Questions for Exploratory Analysis:

Which establishments have a hygiene score equal to 20?

Which establishments in "London" have a 'RatingValue' greater than or equal to 4?

What are the top 5 establishments with a 'RatingValue' of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
