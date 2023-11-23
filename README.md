# -nosql-challenge

This project centers around leveraging the UK Food Standards Agency's restaurant evaluations to assist Eat Safe, Love magazine editors in deciding their future article focus. 

The initial steps involved setting up a MongoDB database named "uk_food," importing data from a provided JSON file, and establishing a MongoClient instance. 

Key imports included MongoClient, pprint, pandas, and matplotlib for creating images of DataFrames. The project encompassed tasks such as adding a new restaurant, Penang Flavors, updating restaurant information, excluding Dover locations as per the magazine's preference, and adjusting data types for numeric values in the dataset.

Jupyter notebook analysis in 


Utilizing the count_documents method, I displayed the number of documents in the result. The first document was presented using pprint and subsequently converted the result into a Pandas DataFrame. The analysis involved identifying establishments with a hygiene score of 20, establishments in London with a RatingValue greater than or equal to 4 (using the $regex method), and the top 5 establishments with a RatingValue of '5' sorted by the lowest hygiene score, closest to the recently added restaurant "Penang Flavours." This proximity search was performed within 0.01 degrees on either side of latitude and longitude.

Additionally, an examination was conducted to determine the number of establishments in each Local Authority area with a hygiene score of 0. The results were sorted from highest to lowest, and the top ten Local Authority areas were printed out using an aggregation method.
