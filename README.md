

## Research Paper - https://arxiv.org/abs/2310.11520
## Website - https://newstextsummarisation.onrender.com
## Google Scholar - 

# News-Text-Summarisation

In today’s rapidly evolving and interconnected world, the importance of news cannot be overstated. It serves as a critical catalyst for societal development, enabling informed decision-making and active citizen participation in civic affairs. However, the sheer volume and complexity of news articles often pose a challenge for individuals striving to stay updated. The application of Natural Language Processing's text summarization models to news articles emerges as a viable solution. By condensing extensive news pieces into concise formats, this approach presents the main points effectively, saving time and encouraging diverse news consumption.

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

## References

- [1] Information about Natural Language Processing's text summarization models.
- [21] Graph-based model reference for extractive text summarization utilizing cosine similarity.
- [22] Google’s PageRank algorithm reference for text summarization.

This graph-based approach, integrating cosine similarity and PageRank, demonstrates promising results in the field of extractive text summarization.

