## ADS 509
# Assignment 1: Data Acquisition with APIs and Scraping

Acquiring data is one of the fundamental steps in any analysis and proficiency at APIs and web scraping unlocks rich data sets for future analyses. In this assignment, you will scrape lyrics from AZlyrics.com.  

Instructions: 

1. Create a repository under your GitHub account from this template: [https://github.com/37chandler/ads-tm-scrape](https://github.com/37chandler/ads-tm-scrape). Instructions can be found [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template). Make your repository public or add your instructor’s Github account as a [collaborator](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository). 
2. Choose two musical artists for your project. Both should have at least twenty songs at their artist page on AZLyrics. Those pages have forms like this: https://www.azlyrics.com/r/robyn.html. 
3. The file “Lyrics Scrape.ipynb” holds your starting code for this assignment. 
    * This file holds starting code for the assignment. Follow the instructions in that notebook, pulling and storing the lyrics for both artists.
    * The final part of the notebook holds the evaluation code. If you’ve completed the assignment correctly, you should be able to just run this section as is. 

**Things to leave out of your repo**
1. Do not include the raw data in the repository. The `.gitignore` file is set up to ignore the `lyrics/` folder. Git attempts to track every character change in every committed file, so committing a large data file and then making any modification to it can result in a repository that is large and hard to work with. 

Assignment Materials:
* [Web Scraping Repository](https://github.com/37chandler/ads-tm-scrape)

Deliverables:
* When you have finished your code, print your notebook as PDFs and upload these documents to Canvas. 
* Commit your code and push the changes to GitHub so your instructor has access to the ipynb notebook files and any other code you create.

# Assignment 2: Tokenization, Normalization, and Descriptive Statistics

This assignment gives you the opportunity to practice the techniques of this module: tokenization, normalization, and calculating descriptive statistics. You will practice these skills here, then use them in every subsequent assignment. 

Instructions: 

1. Create a repository under your GitHub account from this template: [https://github.com/37chandler/ads-tm-token-norm](https://github.com/37chandler/ads-tm-token-norm). Instructions can be found [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template). Make your repository public or add your instructor’s Github account as a [collaborator](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository). 
2. If you did not complete the assignment for Module 1, download “M1 Assignment Data.zip” from Canvas and extract it into your repository. This folder includes not only what you did in the last module, but also information about the followers of the singers on Twitter.  
3. The “Lyrics and Description EDA.ipynb” file within the repository holds the starting code and instructions for the assignment. 
4. Work through the notebook, performing the steps asked of you. Use and extend the code from the chapters of your textbook. 
5. Part of the data in the folder named Twitter is obtained using Twitter API. 

Assignment Materials:
* [Tokenization, Normalization, and Descriptive Statistics Repository](https://github.com/37chandler/ads-tm-token-norm)
* M1 Assignment Data.zip

# Assignment 3: Group Comparison

The task of comparing two groups of text is fundamental to textual analysis. There are innumerable applications: survey respondents from different segments of customers, speeches by different political parties, words used in Tweets by different constituencies, etc. In this assignment you will build code to effect comparisons between groups of text data, using the ideas learned in reading and lecture.   

This assignment asks you to analyze the lyrics and Twitter descriptions for the two artists you selected in Module 1. If the results from that pull were not to your liking, you are welcome to use the zipped data from the “Assignment Materials” section. 

Instructions: 

1. Create a repository under your GitHub account from this template: [https://github.com/37chandler/ads-tm-group-comp](https://github.com/37chandler/ads-tm-group-comp). Instructions can be found [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template). Make your repository public or add your instructor’s Github account as a [collaborator](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository). 
1. If you did not complete the assignment for Module 1, download “M1 Assignment Data.zip” from Canvas and extract it into your repository. If you did complete the assignment for Module 1, then you will use that data in this assignment.  
1. The notebook “Group Comparison.ipynb” holds detailed instructions for the assignment. In that notebook, you are asked to do the following: 
    
    * Read in the data, normalize the text, and tokenize it. When you tokenize your Twitter descriptions, keep hashtags and emojis in your token set.
    * Calculate descriptive statistics on the two sets of lyrics and compare the results.
    * For each of the four corpora, find the words that are unique to that corpus.
    * Build word clouds for all four corpora.

1. Work through the notebook, performing the steps asked of you. Use and extend the code from the chapters of your textbook.

Assignment Materials: 
  
* [Group Comparison Repository](https://github.com/37chandler/ads-tm-group-comp)
* (Optional) M1 Assignment Data.zip

# Assignment 4: Naive Bayes Assignment

In this assignment we use Naive Bayes (NB) for its two greatest strengths: 
1. Exploration of a data set 
1. Classification of new data based on training data

The databases are not small, so I'm going to share them via a Dropbox link.
You should be able to access the file 
[here](https://www.dropbox.com/s/mwhd2ktvtnyapwx/nb-assignment-data.zip?dl=0).

When you get that file, just extract the contents manually into the same
folder as this repository. 

## Part 1: Exploratory Naive Bayes

In this section, you will build a Naïve Bayes classifier on the convention speeches, using the words of the speech text to predict the party (either Republican or Democratic). Your starting notebook walks you through the steps of fitting and using a Naïve Bayes model from the NLTK package. This repo includes some code that would help you limit the number of words you consider in your model, which might improve run-time. We have asked you to fill in some observations from the fitted model.

## Part 2: Classifying Tweets

We have a pretty gigantic database of tweets (and other data) from 
everyone running for Congress in 2018. As an exercise, we'll try to 
use this convention model to classify those tweets. 

The notebook walks you through the steps in broad terms: 
1. Pull data from the congressional DB.
1. Clean, tokenize, and build your feature dictionary for a tweet.
1. Use the classifier from Part 1 to estimate the party of the tweeter.
1. Compare this estimate to their actual party.

# Assignment 5: Topic Modeling

Topic modeling is a fundamental text analysis technique since asking "What are these documents about?" is a fundamental question. In this assignment, you will build an NMF model, an LDA topic model, and an LSA topic model. You will compare the resulting topic allocations. In this assignment, we will work with the Brown University corpus in `nltk`. The documents are in categories already, so you can compare your models to the official classification as well.

## Instructions

1. Create a repository under your GitHub account from this template: https://github.com/37chandler/ads-tm-topic-modeling. Instructions can be found [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template). Make your repository public or add your instructor’s Github account as a [collaborator](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository).   
1. The notebook “Topic Models.ipynb” holds detailed instructions for the assignment. In that notebook, you are asked to do the following: 
    
    *  Run pre-written code exploring the Brown corpus.
    *  Fit a NMF model and interpret it.
    *  Fit an LSA model and interpret it.
    *  Fit an LDA model and interpret it. 

1. Work through the notebook, performing the steps asked of you. Use and extend the code from the chapters of your textbook.

## Assignment Materials
  
* Topic Modeling Repository

Deliverables:

* When you have finished your code, print your notebook as a PDF and upload this document to Canvas. 
* Commit your code and push the changes to GitHub so your instructor has access to the ipynb notebook file and any other code you create.

# Assignment 6: Sentiment Analysis

This assignment gives you the opportunity to practice sentiment analysis in two ways. You will revisit your lyrics and Twitter data or use the pulled data provided for you. You will compare the average sentiment of the songs of your two artists, as well as identify the most positive and negative songs. You will also compare sentiment of the followers of the two artists, by looking at the use of emojis by their followers in their descriptions.

### Instructions: 

1. Create a repository under your GitHub account from this template: https://github.com/37chandler/ads-tm-sentiment. Instructions can be found [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template). Make your repository public or add your instructor’s Github account as a [collaborator](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository). 

2. If you did not complete the assignment for Module 1, download “M1 Assignment Data.zip” from Canvas and extract it into your repository. If you did complete the assignment for Module 1, then you will use that data in this assignment.  

3. The “Sentiment.ipynb” file within the repository holds the starting code and instructions for the assignment. 

4. Work through the notebook, performing the steps asked of you. Use and extend the code from the chapters of your textbook. 

Assignment Materials: 
  
* [Sentiment Repository](https://github.com/37chandler/ads-tm-sentiment)
* (Optional) M1 Assignment Data.zip

Deliverables:

* When you have finished your code, print your notebook as a PDF and upload this document to Canvas. 
* Commit your code and push the changes to GitHub so your instructor has access to the ipynb notebook file and any other code you create. 
