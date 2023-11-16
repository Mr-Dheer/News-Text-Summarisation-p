

## Research Paper - https://arxiv.org/abs/2310.11520
## Website - https://newstextsummarisation.onrender.com
## Google Scholar - 

# News-Text-Summarisation

In today’s rapidly evolving and interconnected world, it
is impossible to overstate the importance of news. It plays
a crucial function as a catalyst for the development of a
society that makes informed decisions. The news is an essential component of democracies because it enables citizens to
participate actively in civic affairs. However, the vast quantity
of information and the overwhelming nature of news articles
can be daunting, posing a challenge for those who want to
keep themselves updated. The application of Natural Language
Processing’s text summarization [1] models to news articles
arises as a potential solution. This method involves condensing
extensive news articles into concise formats, thereby presenting the main points in an effective manner. By summarising
news articles, individuals are able to remain updated of global
events, saving them time and encouraging diverse news consumption

## Overview

This project utilizes Natural Language Processing techniques for extractive text summarization. The core functionality involves retrieving the latest news using News API and generating summaries of articles. As most APIs provide headlines or links to articles rather than the complete content, this project addresses the need for full articles. By leveraging web scraping using BeautifulSoup on the article links obtained from News API, the model summarizes the content, providing summarized articles for consumption.

## Functionality

- **News Retrieval:** Utilizes News API to collect the latest news articles.
- **Web Scraping:** Retrieves full articles by scraping content from the provided article links.
- **Text Summarization:** Implements a graph-based model for extractive text summarization using TF-IDF, cosine similarity, and Google’s PageRank algorithm.
- **Website Integration:** Provides a user-friendly interface to search and access summarized news articles.

## Model Working

The graph-based model for extractive text summarization operates through several steps:

1. **Tokenization and Vectorization:** Text is tokenized into sentences and transformed into numerical representations using TF-IDF.
2. **Cosine Similarity:** Calculates sentence similarity using cosine relationship, generating a similarity matrix.
3. **Graph Construction:** Constructs a graph with sentences as nodes and edge weights reflecting sentence similarity.
4. **PageRank Algorithm:** Applies Google’s PageRank algorithm to score sentence importance within the context of the text.
5. **Summary Generation:** Ranks sentences based on PageRank scores, composing the extractive summary from the top-ranked sentences, effectively capturing the essential content of the original text.


