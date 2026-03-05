# CS 4412 Data Mining Project  
**Discovery of Linguistic Patterns in Japanese News Articles**

## Project Description
This project explores hidden patterns in Japanese news articles using data mining techniques.  
Rather than focusing on prediction, the goal is **unsupervised discovery**, including:

- Identifying natural clusters of news articles based on linguistic similarity
- Discovering frequently co-occurring Japanese words and phrases to reveal semantic associations

Because Japanese text does not contain whitespace between words, morphological analysis is used to tokenize articles before applying clustering and association rule mining techniques.

## Dataset
**Japanese Newspapers (2005–2021)**  
- Source: Kaggle  
- Link: [https://www.kaggle.com/datasets/vyhuholl/japanese-newspapers-20052021](https://www.kaggle.com/datasets/vyhuholl/japanese-newspapers-20052021?select=japanese_news.csv)  
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
├── notebooks/ # Analysis notebooks (preprocessing, EDA, clustering)
├── README.md
├── docs/ # Contains project proposal
```

## Current Status (Milestone 2)
- Implemented Japanese tokenization with fugashi/MeCab and custom stopword filtering.
- Performed exploratory analysis with histograms of article lengths, source counts, and top tokens.
- Built TF IDF document vectors and applied K-Means clustering to discover high-level themes (e.g., politics, finance, local/disaster news, crime, and sports) in the news corpus.

## Needed installs
 - You must run the notebook in a venv
### Installs
 - pip install pandas numpy
 - pip install "fugashi[unidic-lite]"      
 - pip install scikit-learn               
 - pip install matplotlib  
 - pip install jupyter                     
 - pip install mlxtend  