# Problem Statement

The management at reddit want to improve their ability to perform analysis of text posted to their site. Social media and Tech. companies are increasingly being called upon to be responsible for the content on their site. For instance, they may be asked to prevent hate speech that spreads violence, identify threats, and so on. Reddit management decided to form a team of data scientists to work on this problem, and as a proof-of-concept, have consulted Dr Monday Oshoikpor(a data scientist) to demonstrate the value of machine learning applied to natural language processing.

In response to that challenge, this project specifically attempts to answer the question:
**Given a post is from one of these two subreddits, correctly classify whether or not a post came from the r/LanguageTechnology thread**.

* r/LanguaguageTechnology <=== Target
* r/videos


# Data Overview and Analysis

I defined a function to state the parameters(subreddit in this case), used the requests.get method of the reddit API to obtain the requested data from url and parameters.Used res.json to convert the data to json format.I extracted information from subreddit r/LanguageTechnology and r/videos,combine both to form a dataframe.

Before modeling I looked at the most common words contained in each set to get a sense for the language in the subreddits.I started the modeling process with the intention to create and compare KNN with Tfidf and Random Forestm with Tfidf models to determine which is best model for my predictions.

# Conclusions

This project is a proof-of-concept to explain the power of Natural Language Processing(NLP) and machine learning in identifying and classifying posts based on analysis of the words they contain. Reddit does not want to be caught unprepared and is considering building out a team of data scientists to develop machine learning models that will help them understand and manage content on their site. My task was attempt to show that we could build a model that would identify, with 77% accuracy or better, whether or not a post came from a particular subreddit. We chose to use data from two different subreddits and build a model to identify the post in the dataset that were from r/LanguageTechnology.

It is comfortable to say that we were able to meet the objective by training a model to predict with 77% accuracy those posts belonging to r/LanguageTechnology.

# Recommendation

We recommend the use of different models to score the algorithms.