# Data_Visualization Final Project 



# Data Visualization Final Project –Visualizing Complexity

I wanted to center my final project on the notion that “positivity” and “compassion” are also contagious instead of the negativity and bleakness of the situation and circumstances produced by Covid-19. However, the data tells a different story. I decided to tell a story of the harsh realities and true sentiments brought forth by this deadly pandemic. 
Data Pre-Processing: 
Data Source: 
After extracting a dataset from Kaggle which consisted of tweets of users who have applied the following hashtags: #coronavirus, #coronavirusoutbreak, #coronavirusPandemic, #covid19, #covid_19, #epitwitter, #ihavecorona, #StayHomeStaySafe, #TestTraceIsolate. It contained different variables associated with Twitter including:  the text, the count of retweets, user name, retweet count, country code, language. The hashtag #coronavirus was the most frequently used. The original dataset included 390263 entries and contained 22 different columns. I filtered the tweets based on language and extracted a subset of tweets written in English. I had to reduce the dimensionality of the dataset even further so I started cleaning after extracting positive and negative sentiment scores for each tweet. I removed tweets that had scores of 0 for both positive and negative polarity. 


# Sentiment and Emotion Analysis using VADER (Python) & Syuzhet ( R ) 

An integral part of my approach and project was gaining more insight into the force and sentiment behind the tweets. Sentiment analysis is a technique used to organize opinions expressed in textual context to determine the attitude of the author. Tweets and emotions expressed on social media can be viewed as a sensor or transducer of cultural and social information. Social media platforms like twitter can be seen as conduits for opinion proliferation, further elevating their importance during global crises. 

For my dynamic and interactive visualization (Tableau), I used VADER (Valence Aware Dictionary and sEntiment Reasoner) to extract positive and negative scores.  VADER adopts a rules-based approach and works at sentence level. VADER combines set of five heuristics including punctuation, capitalization, degree modifiers, conjunctions, and preceding tri-grams and a list of lexical features (e.g., words, phrases) which are generally labelled according to their semantic orientation as either positive or negative.  VADER was specifically created for social media platforms so it was well suited for my project given that it performs very well with emojis, emoticons, slang, and acronyms. 

These sentiments may be expanded into categories of emotions. So for my static visualization, I wanted to incorporate emotion analysis methods and techniques which identify 8 kinds of emotions expressed in texts — e.g. joy, sadness, anger, fear, trust, disgust, surprise, anticipation. For the static visualization, I cleaned the tweets for further analysis in R by removing pieces of extraneous information such as hashtags, junk characters, other twitter handles and URLs from the tweets. Using the NRC sentiment dictionary and get_sentiment_function within R’s Syuzhet package, I extracted a sentiment score for each tweet. The NRC categorizes each word in a tokenized tweet in a binary fashion (“yes”/“no”) for each emotion.  I wanted to take a preliminary look into the distribution of emotion with all the words and look what emotions were more dominant. The bar plot and the word cloud (generated in R) guided my design process.

At a broad level, this project made me practice how to to strike a balance between simplicity and complexity when it comes to data visualization. It is a balancing act to take into consideration - readability and also “reach of the message”. What I mean by “reach” of the message is the extent to which the visualization pushes the viewer to ask more questions and connect the dots. Negativity, when fear and anticipation are far more prevalent, seems to spread faster than positivity.  I wanted to use my visualizations as tools to highlight the extent to which social media can be a breeding ground for negativity and associated negative emotions such as fear and anticipation but it can also be a very important tool for us to peek into the minds of the general public and guage sentiment when wielded meticulously. More importantly, I hope my visualizations push people to reflect and react- as the crisis deepens, may we all lean into more positivity and stop the spread of corona and negativity. 



# Resources 

Desai, Mithun. “Sentiment Analysis Using R and Twitter.” Tabvizexplorer.com, 19 May 2018, www.tabvizexplorer.com/sentiment-analysis-using-r-and-twitter/.

Smith, Shane. “Coronavirus (covid19) Tweets.” Kaggle, www.kaggle.com/smid80/coronavirus-covid19-tweets. 

P. Pandey, “Simplifying Sentiment Analysis using VADER in Python (on Social Media Text),” Medium, 08-Nov-2019. [Online]. Available: https://medium.com/analytics-vidhya/simplifying-social-media-sentiment-analysis-using-vader-in-python-f9e6ec6fc52f.

