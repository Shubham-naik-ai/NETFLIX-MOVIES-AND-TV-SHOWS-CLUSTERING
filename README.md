# NETFLIX MOVIES AND TV SHOWS CLUSTERING

![enter image description here](https://miro.medium.com/max/1400/0*vbVDEEzmh0yMFBeY)


# Project Files Description

This Project includes 1 colab notebook, 1 technical documentation as well as 1 presentation:

#### [](https://github.com/Shubham-naik-ai/NETFLIX-MOVIES-AND-TV-SHOWS-CLUSTERING#executable-files)Executable Files:

-   **NETFLIX_MOVIES_AND_TV_SHOWS_CLUSTERING.ipynb**  - Includes all functions required for classification operations.

#### [](https://github.com/Shubham-naik-ai/NETFLIX-MOVIES-AND-TV-SHOWS-CLUSTERING#output)Output:

-   **Google Colab**  - All the outputs are visible in the provided colab notebook.

#### [](https://github.com/Shubham-naik-ai/NETFLIX-MOVIES-AND-TV-SHOWS-CLUSTERING#input-files)Input Files:

-   **NETFLIX MOVIES AND TV SHOWS CLUSTERING.csv**  - Input dataset having information about different shows/movies available on Netflix.

## Introduction

Netflix, Inc. is an American technology and media services provider and production company headquartered in Los Gatos, California. Netflix
was founded in 1997 by Reed Hastings and Marc Randolph in Scotts Valley,
California. The company’s primary business is its subscription based streaming service, which offers online streaming of a library of films and television series, including those produced in house The dataset consists of details (title, director, cast, duration, rating etc..) of tv shows and movies available on Netflix as of 2019.
## Problem Statement

This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.




## Data Summery

1.  show_id : Unique ID for every Movie / Tv Show
    
2.  type : Identifier - A Movie or TV Show
    
3.  title : Title of the Movie / Tv Show
    
4.  director : Director of the Movie
    
5.  cast : Actors involved in the movie / show
    
6.  country : Country where the movie / show was produced
    
7.  date_added : Date it was added on Netflix
    
8.  release_year : Actual Releaseyear of the movie / show
    
9.  rating : TV Rating of the movie / show
    
10.  duration : Total Duration - in minutes or number of seasons
    
11.  listed_in : Genere
    
12.  description: The Summary description

## Steps involved

 1. **As first step, we perform Data Profiling, Cleaning and basic exploration. We had 7787 rows and 12 columns.** **In our dataset there were 5 columns which has missing values director, cast, country, date_added and rating. Since date_added and rating have very few null values we can drop their row of total 17 observations. It won’t affect data significantly. In director, cast and country we substitute the null values with the word ‘No Data’ for further analysis**
 2.    **Next, through the exploratory data analysis and visualization, we gained several interesting insights into the Netflix movies and tv shows clustering. The variety of columns that allowed us to do deep data exploration on each significant column presented.**
 3. **Next, we implemented dimensionality reduction in this we set the value to be 90% in sklearn.**
 4. **Next, we implemented k value using Metric: silhouette in this we got the score of 82% for 5 n_clusters.**

##  Conclusion

 1. **Nearly 70 percent are movies and 30 percent are TV Shows**
 2.  **After 2016 Movies and Tv Shows added maximum**
 3. **There are two different type of time durations for Movies it's in minutes and for TV Shows it's in season**
 4. **Maximum movies are in the range of 90 to 120 minutes**
 5. **Most of the children, sci-fi & Fantasy movies and documentaries take less amount of time**
 6. **K-Means Clustering with silhouette gives the highest score of 82% for number of clusters 5**
