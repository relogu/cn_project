# Data directory

This directory should contain the data for the project.
Some of these data will be created and saved here using the scripts in the repo, others have to be downloaded before starting to use the repo.

# Media Cloud dataset

Media Cloud is an open source and open data platform for storing, retrieving, visualizing, and analyzing online news.

You can find out how much the media have been talking about your subject of interest over time, which were the key events that drove coverage about it, which are the words most frequently used around the keywords you searched for, and which media sources have covered the issue. Exploiting this features is possible to extract data to build the world matrix applying the gensim model using Google News Word2Vec.

To extract efficiently the data one has to tructure queries using the Media Cloud tools of Explorer and Topic Mapper.


### Query construction

Building a query consists of choosing the words or phrases to search for and entering them into the *search for*  field. Media Clouds tools now search at the story level for the keywords you enter. 

The key words should be connected using logic connector as AND, OR and NOT.

> (Boris AND Johnson)

To run a search query for stories written in a specific language the same concept holds.

> (Boris AND Johnson AND language:es)

The time range of interest is set using the Publishing time and even the Media source of the stories can be specified using the specific ID.

Further information at https://mediacloud.org/support/query-guide

# Gensim World2Vec

To check the similarity between two article a word matrix has been created from the occurencies of the words inside the article itself, from this point two articles can be compared computing the World2Vec.

The underlying assumption of Word2Vec is that two words sharing similar contexts also share a similar meaning and consequently a similar vector representation from the model. For instance: "dog", "puppy" and "pup" are often used in similar situations, with similar surrounding words like "good", "fluffy" or "cute", and according to Word2Vec they will therefore share a similar vector representation.
