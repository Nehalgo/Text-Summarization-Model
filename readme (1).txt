TEXT SUMMARIZATION
(Specialized for COVID-19 topic)

In this project, we are creating a text summariser. 
Today, we have excess of information. Due to the great amount of information we are provided with and thanks to the development of Internet technologies, needs of producing summaries have become more and more widespread. 
Summarization is a very interesting and useful task that gives support to many other tasks as well as it takes advantage of the techniques developed for related Natural Language Processing tasks. 

Description-
We used Extractive approach for text summarization.
(We imported the necessary libraries, including pandas(for dataframe), Nltk(tokenization,stopwords), Sklearn(for classiers) etc.)
In this project, we used nltk library of python, which stands for Natural Language ToolKit, for tokenizing text, downloading stopwords,etc.

First we made functions to calculate different feature scores for sentences, such as 
cue_phrases- the words or phrases which can mark the structure of a discourse in a text or connectors.Sentences having these words given higher score.
[NOTE-Here the list of cue-words includes the important words specically related to COVID-19]
upper_case- the sentences having words written in upper_case are given higher score 
numeric_data- sentences with 
sentence_length- too long or too short sentences are less important
sentence_position- sentences in beginning or end are given higher scores

Then we imported the csv dataset using pandas library.
The dataset used is the one shared on lms for elc activity.
https://drive.google.com/file/d/1aKgJowWfgwCD4rWzKRA5KQZA1tdnDGj4/view?usp=sharing


Using pandas library, we formed dataframe, with coloumns as- different feature scores calculated and label(from above dataset).
We used different classifiers and checked their accuracies and finally chose-DecisionTreeClassifier to train our model.
We finally saved the model.
The sentences with class '1' would be included in the summary.

Now large texts can be given to it as inputs and it will give summarized text as output.


Source of Dataset:
https://drive.google.com/file/d/1aKgJowWfgwCD4rWzKRA5KQZA1tdnDGj4/view?usp=sharing
References:
Thapar learning management system and google
Name and roll no.:
Nehal  -  102003396
Aditi – 102003406
