### Installation ###
Besides using `spacy` there should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.

### Project Motivation ###
In this repository I analyze the **inaugural address corpus**. This textual data source has the uncommon characteristic that it also contains a time component which makes it very interesting for analyzation. In the notebook `president_speeches.ipynb` I try to develop visualizations which help answering the following questions:

- *"What are some common topics in the speeches?"*
- *"How important were war and peace over time?"*
- *"What were important words during war and peace peaks?"*

### Used libraries ###
`spacy`, `pandas`, `matplotlib`, `sklearn`

### General Information ###
All of the relevant code for the project is located in the `president_speeches.ipynb` notebook. I will now try to highlight the most important methods of this notebook.

The following two methods are important to **transform the text** to a suitable representation:

- *extract_topics()*: extracts the topics (for now its simply extracts nouns)
- *create_tfidf()*: creates a term frequency-inverse document frequency representation

After the text has been transformed the following methods **create the visualizations**:

- *plot_most_frequent_nouns()*: plots the most frequent nouns/topics in the corpus
- *plot_war_and_peace_time()*: plots the nouns 'war' and 'peace' over the timeline
- *plot_words_peek_years()*: plots the most important words of some speeches

### Results ###
The main findings of the code can be found at https://pirnerjonas.github.io/2020/04/07/war-and-peace.html

