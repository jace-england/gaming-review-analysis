# Gaming Review Sentiment & NLP Analysis

This project applies Natural Language Processing (NLP) techniques to analyse Steam player reviews, identifying key drivers of positive and negative sentiment.

It complements a behavioural analytics project by focusing on **player feedback**, using text data to better understand player experience and common issues in games.

## Goals

- Analyse player reviews and uncover the key themes and drivers of sentiment.
- Demonstrate how unstructured text data can be used to inform game design and player experience decisions.

## Key Insights

- Negative sentiment is strongly associated with **server issues, hackers, and monetisation concerns** (e.g. “server”, “hacker”, “money”, “buy”)  
- Positive sentiment is driven by **gameplay experience, social play, and long-term engagement** (e.g. “friend”, “long”, “better”)  
- Bigram analysis highlights common complaints such as **multiplayer and online experience issues**  
- Players with higher playtime tend to leave more polarised feedback, indicating stronger engagement  

## Data Processing & NLP

The project applies a full NLP pipeline to raw review text:

- Text cleaning (lowercasing, punctuation and link removal)  
- Tokenisation and stopword removal (including domain-specific stopwords)  
- Lemmatization using WordNet  
- Filtering of low-quality / short reviews  
- N-gram analysis (bigrams) to capture common phrases

(Data sourced from [here](https://www.kaggle.com/datasets/luthfim/steam-reviews-dataset), not included due to file size limitations)

## Analysis & Visualisation

The analysis includes:

- **Sentiment distribution** of recommended vs not recommended reviews  
- **Review volume by game and sentiment**  
- **Top games by sentiment breakdown**  
- **Word frequency analysis** (positive vs negative reviews)  
- **Bigram analysis** to identify common phrases  
- **Wordcloud visualisations** for sentiment comparison  
- **TF-IDF analysis** to identify high-impact words  
- **Behavioural analysis**:
  - Hours played vs sentiment  
  - Helpful votes vs sentiment  

## TF-IDF Insights

### Positive Drivers
Examples of high-impact positive terms:

- friend, long, better, graphic, free, dlc  

These suggest that **social gameplay, long-term engagement, and perceived value** contribute to positive sentiment.

---

### Negative Drivers
Examples of high-impact negative terms:

- server, hacker, money, buy, dont, fix  

These highlight that **technical issues, cheating, and monetisation frustrations** are key drivers of negative sentiment.


## Tools Used

- Python (pandas, numpy)  
- NLP (NLTK, TF-IDF, n-grams)  
- Data visualisation (matplotlib, seaborn, wordcloud)  
- Visual Studio Code  

## Project Structure

```
gaming-review-analysis/

├── data/              # Raw dataset (not included due to file size) 
├── notebooks/         # NLP pipeline and analysis  
├── outputs/           # Visualisations
└── README.md  

```
## Project Outcome

This project demonstrates:

- Ability to analyse **unstructured player feedback data**  
- Application of NLP techniques to extract meaningful insights  
- Understanding of **player sentiment drivers in multiplayer games**  
- Translating qualitative feedback into **actionable product insights**  

## Ways to Improve

- Topic modelling to identify deeper themes in reviews  
- Linking sentiment to player behaviour and retention  
- Real-time monitoring of player feedback
