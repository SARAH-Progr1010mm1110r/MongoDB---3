# MongoDB-3
## Create an app,functions in MongoDB 

### 1- **In MongoDB Atlas go to the Realm tab**

### 2- **Create a new app (steps):**

  * Create a read/write rule on the chosen dataset
	
  * Enable Authentication provider (API)
	
  * Create an API key
	
  * From the “Link Data Sources tab” activate the MongoDB connection string with the authentication method “API key”. (where your connection string will be URL to connect to your app via Pymongo)
  * On each step, save your draft and deploy it to apply changes to your app.
	
  * Once deployment is done, copy the URL string (don’t forget to paste your API key) and connect to your Realm app through Pymongo MongoClient.

### 3- **Create at least 6 functions from the “Functions” menu in Realm:**

  * Create a function that returns all players’ names from the dataset.
	
  * Create a function that returns a sorted list of all players who are 20 years old or younger. (sort has to be from youngest to oldest)
	
  * Create a function that takes one argument (integer), and returns players’ names, their team name, and the number of goals they scored. The number of goals is greater than or equal to the integer passed to the argument.
	
  * Create a function that returns an average pass success score for each team. Rename field “_id” to “teamName” and round pass success average score to 2 decimal places. (Hint: Use $project keyword)
	
  * Create a function that returns total assists and aerial wins for each team (fields “assistTotal” and “aerialWonPerGame”). Rename field “_id” to “teamName” and round total aerial wins to 2 decimal places. (Hint: Use $proect keyword)
