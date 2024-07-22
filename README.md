#### Problem Statement
The goal of our project is to leverage sentiment analysis to understand public sentiment regarding the transition to clean energy. 
The raw data for this task consists of a multitude of tweets from X(Formerly Twitter), which are rich in textual content and express a wide range of sentiments about the shift towards renewable energy sources
Expected Outcomes: The expected outcome of this project is a sentiment label for each tweet. This involves classifying the sentiment as either positive, negative, or neutral.

#### Data Cleaning and Exploration
As part of cleaning and preprocessing, we will remove stop words, punctuations, special characters and any URL links in the tweets. We will also tokenize the text using word tokenizer, apply precprocessing steps.

#### Model Selection and Development
Since our goal to classify tweets and our data is unlabeled, we will use the ensemble of pretrained models which are trained on vast amount of social media data to classify the tweet sentiments and take the output from ensemble through hard voting of each model for better classification eliminating any biases in one single model.
Pre-trained Models:
1. VADER (Valence Aware Dictionary and Sentiment Reasoner) is a lexicon and rule-based sentiment analysis tool that is specifically attuned to sentiments of social media
2. TextBlob is another sentiment analysis model
3. Pattern has tools for data mining (Google, Twitter, and Wikipedia API, a web crawler, an HTML DOM parser), natural language processing (part-of-speech taggers, n-gram search, sentiment analysis.
4. A BERT model "distilbert-base-uncased-finetuned-sst-2-english" is a model developed by Hugging Face which is pre trained vast amount of social media text.
5. RoBERTa, short for “Robustly Optimized BERT Pretraining Approach”, is a variant of the BERT (Bidirectional Encoder Representations from Transformers) model, developed by researchers at Facebook AI.

#### Summary and Insights
Data Collection: The dataset consists of tweets related to the clean energy transition. This data was sourced from Kaggle, a popular platform for machine learning and data science projects.
Data Preprocessing: The raw tweets were preprocessed to make them suitable for analysis. This involved cleaning the tweets to remove URLs, user mentions, numbers, and stopwords. This step is crucial as it removes unnecessary noise from the data and helps in extracting meaningful insights.
Sentiment Analysis Models: An ensemble of pre-trained models was used for sentiment classification. This ensemble included VADER, TextBlob, BERT, RoBERTa, and Pattern. Each of these models has its own strengths and weaknesses, and using them in combination helps in achieving more robust and reliable results.
Majority Voting: The final sentiment labels were determined by majority voting across the models. This means that for each tweet, the sentiment label that was predicted by the majority of the models was chosen as the final label. This approach helps in mitigating the biases of individual models and ensures more unbiased results.
Results: The sentiment analysis revealed that a significant proportion of the tweets had a positive sentiment towards the clean energy transition. This indicates a generally positive public perception of the clean energy transition, as reflected in the analyzed tweets.







