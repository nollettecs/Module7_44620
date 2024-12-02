# Final Project: Article Summarizer

# Article Sentiment Analysis and Summary Generation
## Overview
This project focuses on analyzing the sentiment of a real-world article, extracting meaningful information, and generating summaries based on sentiment scores. The article's sentiment is evaluated at the sentence level using spaCy and TextBlob, with the goal of creating summaries that highlight the most emotionally charged content.

# Project Workflow
1. Article Acquisition:

The article is fetched from the web (using the URL: https://www.bankrate.com/real-estate/case-shiller/).
The raw HTML content is saved to a file for further processing.

2. Text Extraction:

Using BeautifulSoup, the HTML content is parsed to extract the plain text of the article.

3. Sentiment Analysis:

TextBlob is used to analyze the sentiment of each sentence, generating a polarity score (ranging from -1 for negative sentiment to 1 for positive sentiment).
The text is processed both at the token level (individual words) and the lemma level (base forms of words).

4. Summary Generation:

Sentences with sentiment scores above a predefined cutoff are selected to generate summaries that focus on emotionally stronger content.
Separate summaries are generated based on token and lemma scores.

5. Comparison of Results:

Polarity scores for the full article, token-based summary, and lemma-based summary are calculated and compared.
Differences in sentiment are explained, emphasizing how summary generation based on sentiment scores affects the final polarity.

# Key Outputs
- Polarity Score: Displays the overall sentiment of the article and its summaries (based on token and lemma scores).
- Number of Sentences: Provides insight into the brevity and focus of the summaries.
- Summary Text: The most sentimentally charged sentences are presented in a clean, readable format.

# Conclusion
The sentiment analysis and summary generation process provides an automated way to distill an article's emotional tone. By focusing on sentences with higher sentiment scores, the resulting summaries are more positive, reflecting the key points and ideas with the strongest emotional impact.