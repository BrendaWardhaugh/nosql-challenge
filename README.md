# nosql-challenge

## Part 1: Database and Jupyter Notebook Set Up
Import the data provided in the `establishments.json` file from your Terminal. Name the database `uk_food` and the collection `establishments`.
Data import:
* mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json

## Part 2: Update the Database
An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis. Add the following restaurant "Penang Flavours" to the database.

![new establishment](https://user-images.githubusercontent.com/120147552/228339074-39c0c3c8-b3d2-4da4-81af-fc8db59f8210.png)

## Part 3: Exploratory Analysis
Unless otherwise stated, for each question: 
* Use `count_documents` to display the number of documents contained in the result.
* Display the first document in the results using `pprint`.
* Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.

### 1. Which establishments have a hygiene score equal to 20?

![hygiene 20](https://user-images.githubusercontent.com/120147552/228339871-14c4c0c6-2792-4352-8460-9d0cf935130c.png)

![df hygiene 20](https://user-images.githubusercontent.com/120147552/228340204-2e0b2730-097d-4450-b8d3-d5976f1b06a4.png)

### 2. Which establishments in London have a `RatingValue` greater than or equal to 4?

![london](https://user-images.githubusercontent.com/120147552/228340479-39a9f971-108e-4692-b42c-d4ef0dc47c14.png)

![df 2](https://user-images.githubusercontent.com/120147552/228340713-b97576e0-ce6d-45aa-a2fa-3aee0b8a2e6e.png)

### 3. What are the top 5 establishments with a `RatingValue` rating value of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

![top 5](https://user-images.githubusercontent.com/120147552/228340922-10c628f3-9955-4463-b791-fffb2b8ec72a.png)

### 4. How many establishments in each Local Authority area have a hygiene score of 0?

![Untitled](https://user-images.githubusercontent.com/120147552/228343687-709a513f-acd6-4c35-96bf-702fb023d869.png)

