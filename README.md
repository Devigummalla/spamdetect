# spamdetect
company: codetech it solutions

name:G.J.V.N.Devi

Intern id:CT08SYG

Domain:python

Duration:4 weeks

Mentor:Neela Santhosh

Spam Detection Using Machine Learning

Spam emails and messages have become a growing concern in today’s digital era, leading to security threats, data breaches, and an overwhelming influx of unwanted content. This project focuses on developing a robust spam detection system using machine learning techniques. Specifically, it employs Natural Language Processing (NLP) methods to classify messages as either spam or ham (non-spam) based on textual content.

The dataset used in this project is a well-known SMS spam dataset containing labeled messages as either “ham” (legitimate messages) or “spam” (unwanted messages). The dataset is loaded using pandas, and only the necessary columns are retained: the label (spam or ham) and the message text. To facilitate machine learning model training, labels are converted into binary values, where ham is assigned 0 and spam is assigned 1. A crucial step in spam detection is text preprocessing, which involves cleaning the message content to improve model performance. The preprocessing steps include converting all text to lowercase to maintain uniformity, removing punctuation and special characters using regular expressions, and eliminating stop words (common words like “the,” “is,” etc.) using the TF-IDF vectorizer.

To convert raw text into a numerical format suitable for machine learning, the Term Frequency-Inverse Document Frequency (TF-IDF) vectorization technique is used. TF-IDF measures the importance of a word in a document relative to a collection (corpus) of documents. This technique helps in emphasizing unique words associated with spam messages while reducing the impact of commonly used words.

For classification, the Multinomial Naïve Bayes (MNB) algorithm is chosen due to its effectiveness in text classification tasks. Naïve Bayes is based on probability theory and is particularly well-suited for problems with categorical data like text classification. The dataset is split into 80% training and 20% testing data, and the model is trained on the TF-IDF-transformed training data. Once trained, the model is tested on unseen data to evaluate its effectiveness. The following performance metrics are used: Accuracy Score, which measures the overall correctness of predictions, and the Classification Report, which provides a detailed analysis of precision, recall, and F1-score for both spam and ham classes. The model achieves a high accuracy score, demonstrating its ability to effectively differentiate between spam and legitimate messages.

To validate real-world performance, an example spam email (e.g., “Congratulations! You have won a free iPhone. Click the link to claim now.”) is tested. The model successfully identifies it as spam, showcasing its practical application. This project effectively utilizes machine learning and NLP techniques to build a spam detection system. The combination of TF-IDF vectorization and the Naïve Bayes classifier provides a simple yet powerful approach for text classification. The model can be further enhanced by incorporating deep learning methods, handling advanced text patterns, and continuously updating with new spam trends to improve accuracy.


