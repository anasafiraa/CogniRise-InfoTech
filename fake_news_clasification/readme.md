## TASK 2
### FAKE NEWS CLASIFICATION

Fake news classification is the process of using machine learning models to distinguish between FAKE and REAL news. By analyzing patterns in text data (such as headlines and news content), models can predict whether an article is fabricated or authentic. This approach is important in today's digital age to help detect and mitigate the spread of misinformation and improve media literacy.

### Objectives
This project aims to:
- Develop a machine learning model capable of classifying news as FAKE or REAL with high accuracy.
- Evaluate the performance of several models, such as XGBoost, SVM, and Naive Bayes, to determine the most effective method in hoax news classification.
- Utilize insights from the evaluation results to build a robust system for detecting misinformation to support digital information integrity.

### Dataset Characteristics:
- Diversity: Contains a mix of real and fake news, providing a balanced perspective for model training.
- Purpose: Designed to train predictive models to distinguish patterns between real and fake news.

### Project Steps
#### Data Preprocessing:
- Cleaning: Cleans text from numbers, capital letters, punctuation, and other irrelevant elements.
- Case Folding: Changing the entire text to lowercase to maintain consistency.
- Tokenization: Breaks the text into individual words for further processing.
- Stopword Removal: Removes common words that have no semantically important value (such as “and”, “or”).
- Vectorization: Converts text into a numerical representation using the CountVectorizer technique, which allows machine learning models to understand patterns in text data.on techniques.

#### Model Selection and Training:
- Divide the dataset into training and test data to evaluate model performance.
- Train several machine learning models, such as:
  - XGBoost: Known for its high accuracy and ability to handle complex patterns.
  - Support Vector Machine (SVM): Effective in handling high-dimensional data.
  - Naive Bayes: Simple and efficient, suitable for text classification tasks.

#### Model Evaluation:
- Uses metrics such as accuracy, precision, recall, and F1-score to evaluate model performance.
- Analyze the confusion matrix to understand the distribution of errors (false positives and false negatives).

#### Analysis:
- Comparing models based on their performance and stability.
- Determining the best model that is most suitable for use in hoax news classification.

### Results and Insights
- XGBoost:
  - Performance: Highest accuracy of 92.78%.
  - Pros: Able to capture complex patterns and produce minimal error distribution.
  - Applications: Suitable for systems that require high accuracy.
- Support Vector Machine (SVM):
  - Performance: 87.00% accuracy.
  - Pros: High precision, making it suitable for situations where false positives should be minimized.
  - Disadvantages: Lower recall indicates the possibility of this model missing some positive examples.
- Naive Bayes:
Performance: 89.06% accuracy.
  - Pros: Fast and lightweight, suitable for situations with limited computing resources.
  - Disadvantages: Generates more false positives than XGBoost.

### Conclusion 
- XGBoost is the best model for this dataset due to its high accuracy and low error distribution.
- SVM is relevant in scenarios where precision is a top priority, especially to reduce the risk of false positives.
- Naive Bayes is a quick choice for situations with limited resources, although it has a higher risk of prediction error.

This project demonstrates that machine learning models can be effectively used to detect fake news, making a positive impact in the fight against misinformation and supporting media literacy.
