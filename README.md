**Project: UK Food Standards Agency Data Analysis**

**Description:**
The UK Food Standards Agency evaluates various establishments across the United Kingdom, assigning them food hygiene ratings. This project was undertaken to support the editors of the food magazine, *Eat Safe, Love*, in their efforts to identify establishments for future articles. The objective was to analyze and modify the ratings data to provide insights that would assist journalists and food critics in their decision-making process.

**Part 1: Database and Jupyter Notebook Setup**
In this section, the initial setup involved importing the establishments.json data into a MongoDB database named "uk_food" with the collection name "establishments." The Jupyter Notebook utilized PyMongo and Pretty Print (pprint) libraries to connect to the database and confirm the data import. Additionally, the notebook provided the necessary code and queries to prepare the "establishments" collection for further analysis.

**Part 2: Update the Database**
The magazine editors requested specific modifications to the database before any queries or analysis could be performed. The changes included adding a new halal restaurant, "Penang Flavours," which had not been rated yet. The notebook updated the collection with this new restaurant and verified its insertion. Furthermore, it involved finding the BusinessTypeID for "Restaurant/Cafe/Canteen" and updating the "Penang Flavours" restaurant with this information. The notebook also checked the number of documents containing the Dover Local Authority, removed them from the database, and ensured their successful deletion. Finally, number values stored as strings were converted to decimal numbers and integers using update_many queries.

**Part 3: Exploratory Analysis**
The exploratory analysis section addressed specific questions requested by *Eat Safe, Love*, to guide their location choices for articles and reviews. These questions covered various aspects of the establishments, such as hygiene scores, ratings in London, top-rated establishments, and local authority areas with hygiene scores of 0. The notebook provided queries, counts, and visualizations to present the results effectively.

The project aimed to support Eat Safe, Love by providing insightful analyses and modifications to the database, enabling the magazine to make informed decisions about focus areas for future articles.
