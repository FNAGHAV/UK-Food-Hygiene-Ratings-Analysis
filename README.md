# UK Food Hygiene Ratings Analysis
Background
The UK Food Standards Agency evaluates various establishments across the United Kingdom and assigns them a food hygiene rating. This project involves analyzing the ratings data to help the editors and journalists of the food magazine "Eat Safe, Love" decide where to focus their future articles.

Project Overview
This project is divided into three main parts:

Database and Jupyter Notebook Setup
Updating the Database
Exploratory Analysis
Part 1: Database and Jupyter Notebook Setup
In this part, the data provided in the establishments.json file was imported into a MongoDB database. The database was named uk_food and the collection establishments.

Steps:
Imported data from establishments.json into MongoDB.
Confirmed the creation of the database and data import.
Displayed one document from the establishments collection to verify the import.
Part 2: Update the Database
This part involved making several updates to the establishments collection based on the magazine editors' requests.

Updates Made:
Added a New Restaurant:
Added information about a new halal restaurant in Greenwich that hadn't been rated yet.
Found and updated the BusinessTypeID for the new restaurant.
Removed Establishments in Dover:
Checked and removed all establishments within the Dover Local Authority.
Converted Data Types:
Converted latitude and longitude from strings to decimal numbers.
Converted RatingValue from strings to integer numbers.

Part 3: Exploratory Analysis
This part involved answering specific questions from "Eat Safe, Love" using the data in the establishments collection.

Questions Answered:
Found and listed establishments with a hygiene score of 20.
Identified establishments in London with a rating value of 4 or higher.
Listed the top 5 establishments with a rating value of 5, sorted by the lowest hygiene score, near the newly added restaurant "Penang Flavours".
Counted the number of establishments in each Local Authority area with a hygiene score of 0.
Sorted and displayed the top ten Local Authority areas with the highest counts.

