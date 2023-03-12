# student-project
## Overview
>This repo helps to explore relationships between budget, genre, TMDB average vote score, and profits.The best movies for optimizing vote score and total profit are long, high budget, Action/SciFi or Action/Adventure movies. These still have  much higher than average movie, but may require expensive IP. Short, high budget, Animation/Adventure/Comedy movie.
>## Business Problem
Microsoft sees all the big companies creating original video content, and they want to get in on the fun. They have decided to create a new movie studio, but the problem is they don’t know anything about creating movies. They have hired you to help them better understand the movie industry. Your team is charged with exploring what type of films are currently doing the best at the box office. You must then translate those findings into actionable insights that the head of Mi
# Questions to consider:
1. What is the best / worst performing movies in terms of profits?
2. What is the release month vs. average revenue?
3. What is the  average rating vs. revenue?
4. What is the average rating vs. revenue?
# Description of data
>#numpy for high level mathematical functions and working with Arrays
>import numpy as np
>#pandas data manipulation and analysis for tablular data
>import pandas as pd
>#seaborn and matplotlib for data visualization
>import seaborn as sns
>import matplotlib.pyplot as plt
>%matplotlib inline

# Loading data
>data=pd.read_csv("bom.movie_gross.csv.gz",index_col=0)
>data
>data_1 =pd.read_csv("tmdb.movies.csv.gz",index_col=0)
>data_1
>data_2=pd.read_csv("tn.movie_budgets.csv.gz",index_col=0)
>data_2
# cleaning data
>cleaned(data)
>cleaned(data_1)
>cleaned(data_2)
# merging of dataframes
>#merged_data = data_merge.merge(data_2, on='movie')
>#merged_df
>#data_gp_movie = data_merge.groupby('movie')
>#data_gp_movie.first()
# reassign back to a dataframe object
>#data_merged_movie = data_gp_movie.first()
>data_merged_movie
# Visualizations
# Conclusion
> Project will consider these datasets: 'tn.movie_budgets.csv.gz' and 'tmdb.movies.csv.gz' and 'imdb.title.basics.csv.gz'
> The bottom line for the "success" of a film is the money it makes (profits). Variables that may influence the "success" of a film:
1. Worldwide Gross Revenue
2. Vote Count
3. Popularity
4. Release Date
5. Movie
6. Genre_ids
> The merged_data contains information about movies including their budget, revenue, release dates, genres, and production companies.Some of the variables in the dataset include id, original_title, genres, release_date, production_budget, worldwide_gross, vote_count, vote_average, popularity, production_companies, release_year, release_month, and profits.
 # Findings
 Movies with high quantities of high ratings fetch big profits! So, produce quality movies catering to the largest majority of people, to garner a larger volume of high ratings.
Make more movies about “adventure.” The “adventure” genre makes the most money. Otherwise, “animation” and “horror” are the next best options.
Generally, during the summer is good. If a movie must be released to make a last-minute buck, November is your best bet.
