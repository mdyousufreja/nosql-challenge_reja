# nosql-challenge_reja
module 12 challenge


## Files ##

Downloaded the following files to get started:

Module 12 Challenge [files](https://bootcampspot.instructure.com/courses/3819/assignments/56641?module_item_id=999979)

## Instructions ##

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

## Part 1: Database and Jupyter Notebook Set Up ##

Used NoSQL_setup_starter.ipynb for this section of the challenge.

1. Imported the data provided in the **establishments.json** file from my Gitbash Terminal. Named the database **uk_food** and the collection **establishments**. Copied the text I used to import my data from my Terminal to a markdown cell in my notebook.

2. Within my notebook, imported the libraries that I need: **PyMongo** and **Pretty Print** (pprint).

3. Created an instance of the **Mongo Client**.

4. Confirmed that I created the database and loaded the data properly:

    - Listed the databases I have in MongoDB. Confirmed that **uk_food** is listed.
    - Listed the collection(s) in the database to ensure that **establishments** is there.
    - Found and displayed one document in the **establishments** collection using **find_one** and display with **pprint**.
      
5. Assigned the establishments collection to a variable to prepare the collection for use.

## Part 2: Update the Database ##

Used **NoSQL_setup_starter.ipynb** for this section of the challenge.

The magazine editors have some requested modifications for the database before I can perform any queries or analysis for them. Made the following changes to the establishments collection:

1. An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked me to include it in my analysis.
2. Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.

Update the new restaurant with the BusinessTypeID you found.

The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.

Some of the number values are stored as strings, when they should be stored as numbers.

Use update_many to convert latitude and longitude to decimal numbers.
Use update_many to convert RatingValue to integer numbers.
