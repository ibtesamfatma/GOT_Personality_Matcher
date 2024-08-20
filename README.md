Project: Game of Thrones Character Personality Matching ⚔️

This project explores the personalities of characters in the popular TV show Game of Thrones using a dataset of character scripts. The goal is to identify potential relationships between characters based on their dialogue. 💬



Data 📊

The data for this project is a JSON file containing character scripts from the Game of Thrones series. The data can be found on Kaggle: [invalid URL removed] والثrones-data


Methodology 🛠️

Data Preprocessing 🧹

- The script data is loaded from a JSON file into a pandas DataFrame. 

- The script for each character is separated into individual lines of dialogue. 🗣️

- A new DataFrame is created for each character, containing their individual lines of dialogue. 📝

- All dialogues for each character are combined into a single string. 🔗

- A new DataFrame is created with a column for each character's name and their combined dialogue. 

- Stop words (common words like "the", "a", "an") are removed from the dialogue text. 🚫
  
Feature Extraction 🔍

A CountVectorizer is used to convert the character dialogue text into a document-term matrix. 📚

This matrix represents the frequency of words in each character's dialogue. 

Dimensionality Reduction 

T-SNE (t-distributed Stochastic Neighbor Embedding) is used to reduce the dimensionality of the document-term matrix. 📉

This reduces the number of features to two, allowing for visualization in a scatter plot. 🗺️

Visualization 🎨

A scatter plot is created using Plotly Express. 📈

Each character is represented as a point in the scatter plot, positioned based on their two-dimensional TSNE coordinates. 

The name of each character is displayed as a label on the scatter plot. 

Results 💡

The scatter plot provides a visual representation of the relationships between characters based on their dialogue. Characters with similar speech patterns may be positioned close together in the plot, suggesting potential personality matches. 🤝

![newplot-2](https://github.com/user-attachments/assets/86f676dd-a0d5-4588-a449-b379ded462f3)

![newplot](https://github.com/user-attachments/assets/05410913-10da-4cac-a0f3-7f343919eaca)

Next Steps ⏩

Analyze the scatter plot to identify potential character relationships. 🕵️‍♀️

Explore different dimensionality reduction techniques. 🧪

Implement clustering algorithms to group characters with similar personalities. 👥

Evaluate the effectiveness of the personality matching approach. ✅
Code 💻

The code for this project is available in a Jupyter Notebook or Python script (replace with the file format you're using). 🐍
