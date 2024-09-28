# Predictive Modeling of E-commerce App User Review Topics from Google Play Store

## Project Overview 
This project aims to perform topic modeling on user reviews collected from various e-commerce applications available on the Google Play Store. The objective is to group the reviews into distinct topics to better understand user opinions, sentiments, and concerns about these applications.

We employ Latent Dirichlet Allocation (LDA) and Latent Semantic Analysis (LSA), alongside Bag of Words (BoW) and TF-IDF as feature extraction techniques, to create models that predict the topics from review data. These models are then compared based on their coherence scores, and the most efficient model is selected for detailed analysis.

## Methodology
1. Data Collection
   - Source: Google Play Store reviews for 8 e-commerce applications: Shopee, Tokopedia, Lazada, Blibli, Zalora, Bukalapak, Tokobagus, and Alibaba.
   - Scraping Tool: Python library google_play_scraper was used to extract review text, ratings, and metadata (dates, usernames).
   - Total Data: 2388 reviews.
2. Data Preprocessing
   - Data Cleaning: Removal of URLs, numbers, symbols, emojis, and extra spaces.
   - Tokenization: Breaking reviews into tokens (words).
   - Lemmatization: Conversion of words to their base form.
   - Stopword Removal: Elimination of common stopwords (e.g., "the", "a", "in") to focus on meaningful content.
3. Feature Extraction
   - Bag of Words (BoW): Converts reviews into a frequency-based numerical format.
   - TF-IDF: Assigns weights to words based on their importance in a specific document relative to the entire dataset.
4. Model Building
   - Latent Dirichlet Allocation (LDA): A generative probabilistic model used to discover latent topics in a collection of reviews.
   - Latent Semantic Analysis (LSA): A matrix decomposition technique to find hidden structures in a collection of text.
5. Hyperparameter Tuning
   - Grid search was used to optimize model parameters (number of topics, alpha, eta) to achieve the highest coherence scores for each model.
6. Model Comparison
   - The models were compared using coherence scores to evaluate the quality of the topics generated. Visualizations such as word clouds and intertopic distance maps were used to interpret the results.

## Results
- The LDA with BoW model produced coherent topics related to customer service, order issues, and application performance.
- The LSA models showed strong semantic relationships between words, identifying sub-themes within broader topics.
- The highest coherence score was achieved by the LDA model using BoW + TF-IDF with a score of 0.512, indicating it captured the most accurate and meaningful topics from the reviews.

## Conclusion
By analyzing e-commerce app reviews through topic modeling, the project highlights key areas of user concern, such as app functionality, customer service, and order-related issues. Developers can use these insights to improve their applications, addressing user complaints more effectively.

## Contributors

2501971742 - Alisha Zahra Saadiya

2501975620 - Diva Nabila Henryka

2540121322 - Lovina Anabelle Citra
