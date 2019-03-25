# The evolution of language in films

__[Link](https://robertinjac.github.io/The-evolution-of-language-in-films) to the data story.__

## Abstract
The OpenSubtitles2018 database contains subtitles from more than 150 thousand movies released between the late 19th century and today. The language used in a movie is one of its most important parts. People usually remember the best lines or dialogues from their favorite movies. 

In our project we rigorously analyzed a movie's language properties: its simplicity or complexity, its positiveness or negativeness, its mildness or strongness and have explored how these attributes have changed over time. Moreover, films can usually be classified into genres and we therefore analysed how the aforementioned language properties differ across genres.

Another interesting questions is how important the language properties are for a movie's success? Is it possible to find a correlation between the above mentioned language properties and how well perceived the movie was by the public? This is a another question we have answered in our project.

To summarize, the analysis of the language properties of movies gave us a fuller picture of movie history and the connection between the two medias - the textual and the visual. And after all, the language used in movies reflect the language used by ordinary people in everyday life. 

## Research questions
__Generally, we are focusing on the language used in films.__

* _How has the language in films evolved over time?_ 
  * Are films using more violent and strong langauge now compared to before?
  * Is the language used in films more or less complex nowdays compared to the past?
  * Is the language used more positive or negative in films today compared to the past? 
* _What are the differences in language across genres?_
  * Does the language properties mentioned above differ across genres? 
* _How does a movies language properties affect the public's perception of a movie?_
   * Is it possible to find a positive or negative correlation between the above mentioned language properties and the public's opinion about a movie?


## Dataset
The primary dataset we are using is the _OpenSubtitles2018_ dataset. The dataset has film subtitles for three languages: English, French and Chinese. We are going to use only the English part. It has 25 GB of data and offers film subtitles from the late 19th century to 2018. 

The format of the dataset is easy to use. For each year we have a folder of the films that were released that year. Then, for every film we have an XML file with its subtitles. Here is an example of 
a sentence contained in one of the subtitle files:

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
In addition to the subtitles, some meta data is given about the film: duration, date genre, number of sentences, etc.

The OpenSubtitles2018 dataset contains the IMDB id of each movie. We used this id to connect the OpenSubtitles2018 dataset with the IMDB datasets. The IMDB dataset which was used in this project is the ratings dataset which contains the average rating and number of votes for all movies in the IMDB dataset. The ratings dataset is stored in TSV format (tab-seperated-values) and is freely distributed by IMDB (https://datasets.imdbws.com/).


## Contributions of all group members

### Jakob Svenningsson

* Worked on problem formulation and planning in collaboration with Robert 
* Extracting of subtitle data from its original storage format (XML) to spark dataframes. This was done using the provided cluster.
* Did parts of the descriptive statistics and analysis.
* Collection of results. I wrote the spark scripts which were used to calculate our  results and ran the scripts on the cluster.
* Created all the plots for the data story.

### Robert Injac

* Worked on problem formulation and planning in collaboration with Jakob 
* Did parts of descriptive statistics and analysis
* Created and designed the data story website
* Wrote data story descriptions and conclusions.

We will both work on the poster and the final presentation in January.
