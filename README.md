# CS3-DS4002
# Documentation Map

DATA Folder:
Includes all required data needed for the case study, with the scripts of each of the first 7 STAR WARS movies. All data is in txt format.

SCRIPTS Folder:
Includes all required scripts notebooks with code needed for case study.

ARTICLES Folder:
Includes all supplemental reading for further information into the case study's code and topic.

Hook Document & Rubric
The hook document includes relevant background information regarding the case study topic and objectives.
The Rubric includes assignment details required to meet specifications.

# Software and Platform

All coding was done in Python in Jupyter Notebooks using Windows 10 software. 
The required packages and add-ons include: vaderSentiment, NRClex, Pandas, Numpy, matplotlib, tdqm notebook, nltk, punkt, wordnet, averaged_perceptron_tagger, stopwords, brown, vader_lexicon, opinion_lexicon, and punkt_tab


# Instructions for reproducing results

Step 1: importing add ons
Start by downloading vaderSentiment and NRClex from the internet and using pip install to use them in Python. 
Import nltk and essential NLP datasets (punkt, wordnet, averaged_perceptron_tagger, stopwords, brown, vader_lexicon, opinion_lexicon, punkt_tab)
Import re, pandas, numpy, and matplotlib

Step 2: import data
Download all txt files under the Data folder
Assign each text file a respective episode variable (episode1 = SW_01.txt, episode2 = SW_02.txt, etc..)
Group the data into trilogies (Prequels = (episode1, episode2, episode3), original = (episode4, episode5, episode6), sequels = (episode7)

Step 3: Cleaning data
For each script use re to clean them, converting all text to lowercase, replace all new lines with a space, replace multiple spaces with a single space, remove numbers, remove punctuation (except spaces), and finally remove all screenplay markers (int, ext, cut, to, cont, continued, fade)

Step 3: Emotional Analysis
Use the “analyzer.polarity_scores()” command to calculate the VADER compound, positive, negative, and neutral scores for each film. Print the scores for each film.
Create a new variable for each script that uses NRCLex ex: (episode1_NRC = NRCLex(episode_clean)). Use the command episode_NRC.raw_emotion_scores to get the count of emotion in each movie. Also use the command episode_NRC.affect_frequencies to get the frequency of the emotion throughout each movie. 
Create a dictionary of the NRC frequencies for each episode and remove the positive and negative emotion. Then set the variable, “max_emotion_episode” to the max emotion frequency from each episode. Print the value.
 
Step 4: Plotting Results
In separate plots, plot the negative, positive, and neutral sentiment scores for the first and second trilogy on a bar graph.
Create a bar plot with the x-axis being each episode and y-axis being the frequency of an emotion. Make a bar plot for each emotion separately.
Create a bar plot with the x-axis being each emotion and y-axis being the frequency of an emotion. Make a bar plot for each episode separately. 



# Other Notes:
1. The articles section contains a review of the book used to comepare sentiment scores across generational differences in demeanr. For a more in depth view, look to borrow the book "Generations: The Real Differences Between Gen Z, Millennials, Gen X, Boomers, and Silents—and What They Mean for America's Future" by Jean Twenge.
