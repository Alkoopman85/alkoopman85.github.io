## Topic Analysis and Word2Vec Model of the Yelp Dataset

**Project description:** There are four major steps that make up this project. The first was preprocessing the data using spaCy, this included tokenization, lemmatization, punctuation removal and named entity recognition. Next was the phrase modeling step using gensim, creating bigrams and trigrams from the cleaned unigram text. Then we turn to the modeling phase, where we first focused on the funding the optimal number of topics for extraction, the results of which are shown in Figure 1. In this case we landed on 30 topics to use in the gensim LDA model on the full dataset. Figure 2 shows the resulting topics and terms (best seen interactively). Finally A gensim Word2Vec model was trained on the full corpus of 41 million sentences, to find semantic similarity and vector embedding space relationships of terms. This can be seen in Figure 3 (also best seen interactively).

[Preprocessing Code](https://github.com/Alkoopman85/Word2Vec-and-Topic-Analysis-Yelp-Reviews/blob/main/prep_text.py) | [Preprocessing Analysis](https://github.com/Alkoopman85/Word2Vec-and-Topic-Analysis-Yelp-Reviews/blob/main/inspect_prepared_text.ipynb)

### Figure 1: Search Optimal Number of Topics
[Search Code](https://github.com/Alkoopman85/Word2Vec-and-Topic-Analysis-Yelp-Reviews/blob/main/search_for_best_num_topics.py) | [Search Results and Analysis](https://github.com/Alkoopman85/Word2Vec-and-Topic-Analysis-Yelp-Reviews/blob/main/num_topics_search_results.ipynb)
<img src="images/topic_search.png?raw=true">

### Figure 2: Visualization of the Extracted topics using pyLDAvis
[LDA Model Training Code](https://github.com/Alkoopman85/Word2Vec-and-Topic-Analysis-Yelp-Reviews/blob/main/train_lda_model_prep_vis.py) | [LDA Model  Analysis](https://github.com/Alkoopman85/Word2Vec-and-Topic-Analysis-Yelp-Reviews/blob/main/lda_yelp_reviews.ipynb)
<img src="images/static_lda_vis.png?raw=true"/>

[Interactive Version](/images/lda_vis.html)

### Figure 3: Word2Vec Embedding
[Word2Vec Training Code](https://github.com/Alkoopman85/Word2Vec-and-Topic-Analysis-Yelp-Reviews/blob/main/train_word2vec.py) | [Word2Vec Inspection and Analysis](https://github.com/Alkoopman85/Word2Vec-and-Topic-Analysis-Yelp-Reviews/blob/main/Yelp_2_Vec_results.ipynb)
<img src="images/word_vectors_all.png?raw=true"/>

[Interactive Version](/images/word_vectors.html)

