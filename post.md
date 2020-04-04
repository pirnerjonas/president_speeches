### War and Peace in America


(inaugural address)
On tuesday, november 3, 2020, a president is elected for the 46th time in the history of the United States of America. The election of the president will be followed by the inauguration. After the president has recitated the presidential oath of office he or she will give a speech to the people. This speech is the **inaugural address** which gives the president the chance to inform the people of his or her intentions.  

My fellow citizens:

I stand here today humbled by the task before us, grateful for the trust you have bestowed, mindful of the sacrifices borne by our ancestors. I thank President Bush for his service to our nation, as well as the generosity and cooperation he has shown throughout this transition.

Forty-four Americans have now taken the presidential oath. The words have been spoken during rising tides of prosperity and the still waters of peace. Yet, every so often the oath is taken amidst gathering clouds and raging storms. At these moments, America has carried on not simply because of the skill or vision of those in high office, but because We the People have remained faithful to the ideals of our forbearers, and true to our founding documents.

...

excerpt of Obamas inaugural address in 2009

(dataset)
In this blog post I will analyze the **inaugural address corpus** which contains 55 speeches from the years 1789 till 2009. 
As a european, with only a slight interest in history, it was especially interesting for me to find out which topics are typically discussed in the speeches.


#### What are some common topics in the speeches? 

In order to be able to answer this question adequately, one must first think about what a topic actually is or how it should be defined. 

While there are several research areas that deal intensively with this "topic" (e.g. aspect extraction in the field of sentiment analysis) I have simplified this first step. 

Within this project nouns are topics. Of course this is a simplification because this is not always correct (e.g. xxx). But if we now take a look at which nouns occur most often in the corpus, it becomes clear that it is already a very good approximation. 

> plot1

Many of the extracted nouns actually represent thematic fields which are or were relevant in the history of the USA. The most common noun in the corpus is "people" which makes sense since presidents have always taken into account the interests of voters. I found two of the words here particularly interesting. 

These are war and peace. 

Although the absolute frequencies of these words were not unusually high, these words still have an extremely high relevance. Not only in the USA but all over the world war has led to unspeakable suffering and has therefore been an inevitable topic of conversation in presidential speeches. 

#### How important were war and peace over time?

To examine the importance of the concepts I wanted to move away from absolute frequency counts. Just because a word is frequent doesn't mean that it is important. I therefore computed the **term frequency-inverse document frequency (tf-idf)** for each of the extracted nouns. If a noun has a high tfidf score it means that it has a high relative relevance to the document (speech). 

The following plot shows the tfidf score of the nomen war and peace over time.

> plot2

Looking at the line which represents the "war" noun reveals that there are two documents in which the word has a very high expressivness. After a quick google search - apologies for my bad history knowledge - I refreshed my highschool knowledge of history and once again found out about the wars going on in 1813 and 1865. The spikes for the peace curve are happening at the time of the second world war and the vietnam war.

#### What were important words during war and peace peeks?

Now that we know about these peek times of war and peace it would be nice to get a more detailed view on what the presidents were speaking about during these times. Foreach of the corresponding speeches we are looking at the top 10 words according to their tfidf score.

> plot3

It becomes apparent that for the two war documents nouns like "massacre", "battle", "offense" and "savage" seem to be the most important words. The famous phrase of Abraham Lincoln "malice toward none" when he stated his policy toward the defeated Confederacy in 1865 shows up partly with the noun "malice". 

#### Conclusion


