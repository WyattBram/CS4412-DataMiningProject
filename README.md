# CS 4412 Data Mining Project  
**Pattern Discovery in Japanese News Articles**

## Project Description
This project explores hidden patterns in Japanese news articles using data mining techniques.  
Rather than focusing on prediction, the goal is **unsupervised discovery**, including:

- Identifying natural clusters of news articles based on linguistic similarity
- Discovering frequently co-occurring Japanese words and phrases to reveal semantic associations

Because Japanese text does not contain whitespace between words, morphological analysis is used to tokenize articles before applying clustering and association rule mining techniques.

## Dataset
**Japanese Newspapers (2005–2021)**  
- Source: Kaggle  
- Link: https://www.kaggle.com/datasets/vyhuholl/japanese-newspapers-20052021  
- Subset used: `japanese_news.csv`

The dataset contains Japanese news articles with the following fields:
- `source`: News outlet
- `date`: Publication date
- `text`: Full article text

## Planned Techniques
- Text preprocessing with Japanese morphological analysis
- TF-IDF vectorization
- Document clustering (K-Means / Hierarchical Clustering)
- Association rule mining (Apriori / FP-Growth)

## Repository Structure
```
cs4412-project/
├── data/ # Dataset files (or placeholders if large)
├── notebooks/ # Analysis notebooks (future milestones)
├── README.md
```
