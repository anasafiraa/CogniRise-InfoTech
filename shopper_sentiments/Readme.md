# SHOPPER SENTIMENTS

## Definition and Purpose
Shopper Sentiments is a dataset containing over 250,000 customer reviews on the TeePublic platform. This data includes attributes such as reviewer_id, store_location, date, title, review, and review-label (rating from 1 to 5). The goal was to understand customer sentiment towards fashion products and gain insights into their shopping experience.

## Datasets

This dataset has the unique features of geographic coordinates (latitude, longitude) and temporal data (date, month, year), making it a valuable data source for:
- Sentiment analysis of customer reviews.
- Geographic pattern identification.
- Temporal trends (seasonality).
- Categorization of reviews based on sentiment.

TeePublic's platform, with its diverse fashion collection, provides the context to understand customer preferences and sentiments towards the products offered.

## Analysis Stages
1. Data Processing:
  - Importing the dataset, performing pre-processing such as removing non-ASCII characters and stopwords.
  - Labeling sentiment based on rating (below 4 as 'bad experience', and 4 or above as 'good experience').

2. Data Exploration:
  - Analysis of sentiment distribution based on geographical location and time.
  - Visualization using Word Cloud for each sentiment category.

3. Modeling and Evaluation:
  - Split the data into training and testing.
  - Using LinearSVC model for sentiment classification.
  - Evaluate model performance through classification report and confusion matrix.

## Insight

1. Sentiment Distribution
  - Most of the reviews (around 80%) have a happy label, indicating a positive customer experience with TeePublic's products and services.
  - In contrast, reviews with bad experience labels only account for about 17.6%, indicating a small percentage of dissatisfied customers.

2. Model Performance
  - Confusion Matrix shows:
    - The model successfully classified 45,086 happy reviews correctly, with only 1,329 reviews misclassified as bad experiences.
    - Of the bad experience reviews, 6,680 were correctly classified, while 2,525 were incorrectly classified as happy.
  - Overall Accuracy: 93%.
  - Precision, Recall, and F1-Score for both classes show that the model is quite reliable in distinguishing between positive and negative reviews.

3. Sentiment Polarization
  - The high number of positive reviews reflects that the majority of customers are satisfied with TeePublic products.
  - However, it should be noted that negative reviews provide opportunities for improvement, especially in the areas where customers most frequently complain.

## Conclusion
1. Linear SVC model with TF-IDF approach as a vectorization feature can effectively capture sentiment patterns.
2. The analysis shows that TeePublic's services generally get positive responses from customers, but there are areas that need to be improved based on reviews labeled as bad experiences.
