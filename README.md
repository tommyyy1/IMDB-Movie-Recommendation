# IMDB-Movie-Recommendation

## Problem Statement
This project focuses on extracting movie data from IMDb for 2024, specifically focusing on the movie name and storyline. Using Selenium, the program will scrape IMDb to collect movie names and their associated storylines. The storylines will then be pre-processed and analyzed using Natural Language Processing (NLP) techniques, such as TF-IDF (Term Frequency-Inverse Document Frequency) or Count Vectorizer. Using these methods, the project will calculate Cosine Similarity or other Machine Learning algorithms to recommend similar movies based on a given storyline. The project will provide an interactive user interface built with Streamlit where users can input a movie storyline and receive the top 5 recommended movies.

## Approach

### Data Scraping and Storage
- **Data Source**: IMDb Movies page for 2024.
- **Scraping Method**: Use Selenium to extract the following data:
  - Movie Name
  - Storyline (Plot Summary)
- **Data Storage**: Save the extracted movie data into a CSV file for further analysis.
- **Columns**:
  - Movie Name
  - Storyline
- **CSV Storage**: Save the data in a CSV format for easy data manipulation.

### Data Preprocessing and Analysis
1. **Text Cleaning (NLP)**:
   - Preprocess the storyline text by removing stop words, punctuation, and unnecessary characters.
   - Tokenize the story text for further analysis.
2. **Text Representation**:
   - Use TF-IDF Vectorizer to convert the movie storylines into numerical vectors.
3. **Cosine Similarity**:
   - Calculate the Cosine Similarity between the movie storylines to find the most similar movies.
   - Rank the movies based on similarity scores.

### Recommendation System
- **Algorithm**: Use Cosine Similarity or other ML algorithms to find the top 5 most similar movies based on a user’s input.
- **User Input**: Users will be able to input a movie storyline into the Streamlit app, and the system will output the top 5 recommended movies based on storyline similarity.

### Streamlit Interface
1. **Streamlit Application**:
   - Create an interactive user interface using Streamlit.
   - Allow users to input a movie storyline (a short description or plot).
   - The app will process the input and display the top 5 recommended movies with their names and storylines.
2. **Visualization**:
   - Show the top 5 recommended movies as a list with their names and storylines.
   - Provide a dynamic interface that allows users to explore different movie recommendations based on storyline input.

## Dataset
- **Scraped IMDb Data for 2024 Movies**.
- **Columns**:
  - Movie Name: The title of the movie.
  - Storyline: The movie's plot summary or storyline.
- **Format**: CSV file containing the scraped data for all 2024 movies.

## Technical Tags
- **Languages**: Python
- **Libraries/Tools**:
  - Web Scraping: Selenium
  - NLP: NLTK, SpaCy, Scikit-learn (TF-IDF, Count Vectorizer)
  - Recommendation Algorithms: Cosine Similarity, Machine Learning
  - Web Framework: Streamlit
  - Data Manipulation: Pandas
  - Visualization: Streamlit, Matplotlib, Seaborn
- **Environment**: VS Code or Python Environment

## Project Deliverables
- **CSV File**: Containing the scraped IMDb 2024 movie data (Movie Name, Storyline).
- **Python Scripts**:
  - Scraping Script: For extracting the movie data using Selenium.
  - NLP and Recommendation Script: For processing the storyline and calculating recommendations using TF-IDF and Cosine Similarity.
  - Streamlit App Script: For building the interactive user interface.
- **Streamlit Application**: A live application where users can input a storyline and receive movie recommendations.
- **Project Documentation**: A detailed project report explaining the methodology, code, and insights.

## Approach Breakdown
1. **Data Scraping**:
   - Use Selenium to scrape IMDb for movie names and storylines from the 2024 movie list.
   - Store the data in a CSV file.
2. **Data Preprocessing**:
   - Clean and tokenize the storylines using NLP techniques (removing stop words, punctuation, etc.).
   - Vectorize the text using TF-IDF Vectorizer or Count Vectorizer to convert text into numerical form.
3. **Cosine Similarity**:
   - Calculate the similarity between each movie's storyline using Cosine Similarity.
   - Use the similarity scores to rank movies and make recommendations.
4. **Streamlit Interface**:
   - Create an interactive interface where users can input a movie storyline and receive the top 5 recommended movies based on the cosine similarity score.
   - Generated two

## Example Use Case:
- **Input**: A user inputs the storyline: “A young wizard begins his journey at a magical school where he makes friends and enemies, facing dark forces along the way.”
- **Output**: The Streamlit app displays the top 5 movies with similar storylines, such as:
  - **Movie Name**: The Wizard’s Journey (Storyline: A boy discovers his magical abilities and faces a powerful sorcerer.)
  - **Movie Name**: The Magic Academy (Storyline: A young student navigates life at a school for magic, facing powerful challenges.)
  - **Movie Name**: The Dark Sorcerer (Storyline: A young hero confronts an ancient sorcerer threatening the magical world.)




