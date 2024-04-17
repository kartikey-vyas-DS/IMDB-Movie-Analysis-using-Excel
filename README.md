![logo](download.png)
# IMDB Movie Analysis
 The project focuses on analysing the success of movies based on several factors to derive  actionable insights and trends
# Project Description
With this project my aim is to explore the factors influencing a movie's success on IMDB, focusing on high IMDB ratings as a measure of success. This analysis is vital for stakeholders like producers, directors, and investors seeking to understand the determinants of a movie's success for informed decision-making in future projects. By analyzing a dataset containing movie attributes such as genre, budget, duration, cast, director, and IMDB ratings, I'll uncover patterns, correlations, and key predictors of high IMDB ratings. Insights gained will aid stakeholders in optimizing their strategies for producing successful movies and maximizing returns on investment.
# Approach
In initiating the analysis, I commenced by thoroughly examining the dataset's features and their respective statistics. Upon this initial exploration, I discerned certain columns that appeared to be less relevant to the investigation at hand. Consequently, I made the decision to drop the following columns: "Color," "Face No. in poster," "movie IMDB link," "plot keywords," "Director Facebook likes," "Actor 1 Facebook likes," "Actor 2 Facebook likes," and "Actor 3 Facebook likes."
Following this data refinement step, I proceeded to scrutinize the dataset for any instances of missing or null values. Subsequently, I executed the removal of these null values to ensure data integrity and reliability.
One peculiar observation I made during this phase was the presence of an extraneous character "Â" at the end of each movie name. To rectify this inconsistency, I employed the replace function to systematically eliminate this character across all relevant entries.
With these preliminary data preprocessing steps completed, I was poised to delve into addressing the core problem statement and extracting meaningful insights from the dataset.

# Tech Stack Used
Microsoft Excel 2021 version is used for this project due to its simplicity of use 
and extraordinary analysis and visualization capability.
-Observations
![alt text](picture1.png)

![alt text](picture2.png)

![alt text](picture3.png)

![alt text](picture4.png)

![alt text](picture5.png)

Based on the analysis of the scatter plot depicting the relationship between movie release year and IMDB scores, several noteworthy insights emerge. 

Initially, spanning from 1927 to 1966, a notable consistency is observed in the IMDB scores of movies, which remained relatively stable within a range of 6.8 to 8.9. During this period, the cinematic landscape likely featured a more limited number of releases, potentially allowing for a more discerning audience and stricter quality standards.

However, a discernible shift occurs post-1966, characterized by a substantial increase in the volume of movie releases. This surge in cinematic production coincides with a noticeable broadening of the IMDB score range, expanding from 1.6 to 9.3. 

This widening spectrum of IMDB scores suggests a diversification in cinematic offerings, with films spanning a broader range of genres, themes, and artistic merits. Additionally, it may reflect evolving audience tastes, as well as the democratization of filmmaking tools and platforms, enabling a greater diversity of voices and narratives to enter the cinematic landscape.

Overall, these observations underscore the dynamic nature of the film industry over time, marked by shifts in both quantity and quality of movie releases, reflecting the evolving preferences and cultural dynamics of audiences worldwide.

![alt text](picture6.png)

Upon analyzing the scatter plot depicting the relationship between the number of critic reviews and IMDB scores, several insightful observations come to light.

Initially, it becomes apparent that movies with a lower number of critic reviews exhibit a wide range of IMDB scores. This variance suggests that the quantity of critic reviews does not exert a significant influence on the IMDB score within this range. 

However, as the number of critic reviews increases, a discernible trend emerges. Specifically, there is a noticeable uptick in IMDB scores corresponding to higher numbers of critic reviews. Notably, movies with over 600 critic reviews consistently attain IMDB scores above 6.8. This pattern suggests a positive correlation between the volume of critic reviews and IMDB scores, implying that a greater number of critic reviews tends to elevate the perceived quality of a movie.

This finding underscores the importance of critical reception in shaping the perceived quality and success of a movie. As the number of critic reviews serves as a proxy for the level of attention and scrutiny a movie receives, a higher volume of reviews can enhance audience trust and confidence in a film's merits, thereby positively impacting its IMDB score.

In conclusion, the observed correlation between the number of critic reviews and IMDB scores highlights the significance of critical acclaim in influencing audience perceptions and contributing to the overall reception of a movie within the cinematic landscape.

![alt text](picture7.png)

In examining the scatter plot depicting the correlation between the number of user reviews and IMDB scores, a series of insightful patterns emerges.

Initially, the plot reveals a broad spectrum of IMDB scores associated with movies receiving a lower number of user reviews. Within this range, the impact of user feedback on IMDB scores appears to be relatively minimal.

However, as the quantity of user reviews increases, a distinct trend begins to manifest. Notably, there is a noticeable uptick in IMDB scores as the number of user reviews rises. Particularly noteworthy is the consistent performance of movies with over 1900 user reviews, which consistently achieve IMDB scores surpassing 6.2.

This consistent pattern underscores a positive correlation between the volume of user reviews and the perceived quality of movies. Consequently, it suggests that a higher volume of user feedback tends to elevate a movie's IMDB score, reflecting positively on its reception among audiences.

These observations underscore the significance of user engagement and feedback in shaping audience perceptions and influencing the overall reception of a movie. As such, the findings emphasize the pivotal role of user reviews in shaping the success and reputation of movies within the cinematic landscape.

![alt text](picture8.png)

After closely analyzing the bar chart depicting content ratings alongside their respective mean IMDB scores, significant patterns emerge, shedding light on how content classification impacts audience reception.Remarkably, movies classified under the "Approved" and "M" (Mature) ratings exhibit a notably higher average IMDB score, standing at an impressive 7.45 and above. This trend suggests a consistent preference among audiences for content within these categories, characterized by mature themes and content.

Conversely, movies categorized as "PG-13" and "PG" (Parental Guidance Suggested) demonstrate a comparatively lower average IMDB score, hovering around 6.29 and below. These ratings typically indicate content deemed suitable for older adolescents or those requiring parental guidance due to potentially inappropriate material for younger audiences.

The disparity in average IMDB scores between these rating categories underscores a distinct preference among audiences for content aligned with the "Approved" and "M" ratings, reflecting a higher likelihood of achieving a commendable IMDB score.

This observation underscores the critical role of content rating in shaping audience perceptions and preferences, highlighting the significance of aligning content with audience expectations to optimize viewer satisfaction and reception within the cinematic landscape.

# Insights

•	Genre Distribution: - there are two ways of doing this particular analysis, there are two types of genres, one is individual and the other is hybrid genres, I opted to work on individual genre. 
o	It is evident from the observations that Drama is the most common Genre in movies followed by comedy and thriller
o	While statistics suggest that “Film-noir” has the highest average Imdb_score but ther’s only one movie in that category( as we can see the table it has no Mode Variance and Standard deviation), the next highest is History with 7.148 Mean IMDB score and it falls under 150 movies from the dataset, and third is biography with 7.142 Mean IMDB score and it falls under 242 movies from the dataset.
o	Top 5 most common Genre’s are Drama, Comedy, Thriller, Action, Romance in its respective order.
•	Movie Duration Distribution: - most of the movies falls under 98minutes to 114 minutes in this data set , looking at the statistics of the duration Mean is 110.228 and median is 106 which falls under the above stated range, 
o	It is observed from the scatterplot that as the duration of movies increase the volume of movies is decreased which means there are limited movies with higher than 250 minutes duration in comparison to the dataset and IMDB Score seemed to increase with duration and at certain point it started dropping it which is an indication of a range of duration that is good for considering duration of movies.
•	Language Analysis: - it is very clear and evident from the observation that English language is dominating in most of movies (i.e over 95.79%) , followed by French and Spanish with movie counts of 34 and 23 respectively.
o	As seen in the chart by IMDB Score, if we do not consider the “None” category of language, the highest Average IMDB score of 8.13 is on “Persian” language followed by “Hebrew” language having 8.00 Average IMDB Score with movie counts 3 and 1 respectively.
o	Least average IMDB score of 6.0 is with Kazakh on 1 movie count
•	Director Analysis: - as observed from the leaderboard like table of Directors, top 10 directors ranked by Mean IMDB score ranges between 8.4 to 8.7 having 10th director on 99.4 percentile 
o	Top 10 directors were compared with their respective Mean IMDB Scores by overall mean IMDB Scores and all top 10 are evidently above average. 
o	Having a good director indeed leads the entire crew in a systemized manner and operations of that projects would be smooth given high experience of the said director.

•	Budget Analysis: - 
o	The Profit of Movies are calculated with Gross-Budget and the highest profit-making movie in the entire data set is “Avatar” (i.e 523505847)
o	Correlation coefficient is relatively poor here suggesting poor relation between the budget and gross earning which ultimately suggests that having more budget is not sufficient for success of movie
o	The word profit margin basically means finding percentage of the margins achieved, hence the best profit margin in % is “Paranormal Activity” that movie had a budget of $ 15000 only and it ended up making $107917283 giving a robust 719348.55% profit margin an unimaginable return.


# Results
•	A. Drama is the most common genre followed by comedy, thriller, action, romance
•	B. 110.228 and 106 are mean and median of duration column in minutes and highest number of movies falls under 98 to 114 minutes bracket 
•	C. English dominates all movies in this dataset over 95% of movies are in English and movies with higher mean IMDB scores are Persian and Hebrew 
•	D. Director with highest mean IMDB score of 8.7 is Akira Kurosawa.
•	E. Avatar is the highest Profit-making movie and Paranormal activity has the highest Profit margin (%).
