# Title

# Abstract
The OpenSubtitles2018 database contains subtitles from more than 150 thousand movies released between the late 19th century and today. The aim of this project is to analyse the language and vocabulary used in movies.

The language used in a movie is one of its most important parts. People usually remember the best line or dialogues from their favorite movies. In our project we will rigorously analyze the movie language's properties: its simplicity or complexity, its mildness or strongness. We will also check how these properties change over time. The films are usually classified into genres, so we will also check how does language differ across genres.

Analysis of these properties will give as a fuller picture of movie history and the connection between the two medias - the textual and the visual. And after all, the language used in movies is similar to the language used in real life, so this analysis might give us some insight into language in general.


# Research questions
__Generally, we are focusing on language used in films.__
* _How did language evolve in films over time?_ 
    * Are films using more violent and strong language?
    * Are films becoming more less "intelectual" and use more simple dialogues?
* _What are the differences in language across genres?_
    * Are some genres using more or less sophisticated language?
    * Are some genres catering to a specific audience/age group? 


# Dataset
The primary dataset we are using is the _OpenSubtitles2018_ dataset. The dataset has film subtitles for three languages: English, French and Chinese. We are going to use only the English part. It has 25 GB of data and offers film subtitles from the late 19th century to 2018. 

The format of the dataset is easy to use. For each year we have a folder of the films that were released that year. Then for every film we have an XML file for its subtitles. Here is an example of one subtitle:

```xml
  <s id="14">
    <time id="T1S" value="00:01:24,000" />
    <w id="14.1">With</w>
    <w id="14.2">a</w>
    <w id="14.3">good</w>
    <w id="14.4">heart</w>
    <w id="14.5">.</w>
    <time id="T1E" value="00:01:26,000" />
  </s>
```
In addition to the subtitles, some information is given about the film: duration, date genre, number of sentences, etc.

The id of the film is given, which is an IMDB identifier. We can use this id for connecting our dataset to the IMDB datasets. The IMDB offers datasets for film average score and other information for every film. So by connecting our dataset with the IMDB dataset we can get more interesting data for each movie, thus enriching our dataset.  

# A list of internal milestones up until project milestone 2
1. convert the data from XML to a more appropriate format
2. clean the data and deal with missing/inconsistent values
3. merge our dataset with the IMDB dataset to get more features
4. do some descriptive statistics
5. explore how to quantify language complexity and strongness.

# Questions for TA
