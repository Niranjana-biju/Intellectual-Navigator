# Intellectual Navigator

A semantic knowledge exploration and topic recommendation system that helps users discover related topics based on their current interests and previous exploration.

## Features

- Fetches topic summaries and related links from Wikipedia
- Uses Sentence-BERT embeddings for semantic understanding
- Recommends relevant and diverse next topics using cosine similarity
- Maintains a session-based curiosity trail
- Personalizes recommendations using the user's exploration history
- Visualizes the exploration path as a directed graph
- Interactive interface built with Streamlit

## Tech Stack

- Python
- Wikipedia API
- Sentence Transformers (`all-MiniLM-L6-v2`)
- Scikit-learn
- NumPy
- NetworkX
- Streamlit

## How It Works

1. User enters a topic.
2. Wikipedia content and related links are retrieved.
3. The text is cleaned and converted into 384-dimensional embeddings.
4. A candidate pool is created from predefined topics and Wikipedia links.
5. Cosine similarity is used to rank relevant topics.
6. Repetitive and previously explored topics are filtered.
7. The user's exploration history is represented as a curiosity vector.
8. The top recommendations are displayed through the Streamlit interface.



