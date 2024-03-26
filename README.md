# Sentiment_Analysis_LLM
Performs sentiment analysis on customer reviews using a balanced dataset from the Amazon Alexa product reviews.


This code performs sentiment analysis on customer reviews using a balanced dataset from the Amazon Alexa product reviews. Here's a brief overview of the code and its components:

Data Handling:It starts by reading the dataset from a CSV file into a pandas DataFrame, balancing the dataset by downsampling the majority class to address class imbalance.
The dataset is cleaned by removing special characters, HTML tags, single characters, and converting text to lowercase.

Train-Test Split:The dataset is split into training and testing sets, where 95% of the data is used for training and 5% for testing.

Text Generation using Gemini API:The code utilizes the Gemini API from Google's generative AI platform to generate content. Specifically, it uses a model named 'gemini-pro' to generate text.
The generated content is used to classify customer reviews into positive or negative sentiments.

Evaluation:After generating predicted labels for the test set, it computes the accuracy score and plots the confusion matrix to evaluate the performance of the sentiment classification.
Main modules used and their purposes:

numpy and pandas: For data manipulation and analysis.
re: For text preprocessing (cleaning).
sklearn.metrics: For computing accuracy score and generating a confusion matrix.
google.generativeai: For accessing the Gemini API and generating text content.
os and pathlib: For environment variables and file/path handling.
markdown: For converting text to Markdown format for better display in Jupyter notebooks.

The code demonstrates a pipeline for sentiment analysis using a balanced dataset, text preprocessing, model integration via API, and evaluation. It showcases the use of various Python libraries for data manipulation, text processing, and model integration to solve a specific task of sentiment classification.
