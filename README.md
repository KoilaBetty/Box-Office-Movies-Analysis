# Box Office Movies Analysis

![text](Images/premium_photo-1683740129124-0b4aac921cc1.avif)
 By [Unsplash+](https://unsplash.com/photos/a-group-of-people-sitting-in-a-movie-theater-Mffxo3DG5cw)

# Introduction

In today's dynamic film industry, staying abreast of emerging trends is paramount for any studio looking to make a mark. As requested by stakeholders, this report looks into an analysis of recent film trends to provide valuable insights for the launch of the new studio. By examining the types of films that have been performing well, we aim to equip stakeholders with actionable information to guide strategic decision-making

## Overview

The primary objective of this report is to identify and analyze recent trends in the film industry, particularly focusing on the types of films that have garnered success. Through data-driven analysis, we aim to provide stakeholders with a comprehensive understanding of audience preferences and market dynamics, thereby informing the strategic direction for the launch of a new studio.


# 1.1 Explore the tmdb movies dataset with Pandas

## 1.0 Data Understanding

Each record (row) in this dataset represents movies that were aired on box office.

Each feature (column) in this dataset is some attribute of the movies.

We are going to focus on the following features:

**original_title**: `The title of the movies`

**popularity**: `The percentage of how the movies are popular among box office users`

**Vote_average**: ` average rating given to a movie by viewers from a scale of 0 to 10`

**vote_count**: `The number of individual votes or ratings that a movie has received from viewers.Total number of people who have rated the movie`

## Geting Started

### 1.4 Correlation


To understand more about what features of these movies that lead to them getting more popular, let's look at some correlations.

We'll only check the correlations with some kind of numeric data type.
 Explore Correlations

To understand more about what features of these movies that lead to them getting more popular, let's look at some correlations.

We'll only check the correlations with some kind of numeric data type.

![alt text](Images/image-1.png)

![alt text](Images/image-2.png)


#### Interprate the Correlations

As shown above we can note that the correlation between the diffrent variables:

- The correlation coefficient between popularity and vote_average is 0.057. Since it is close to zero this suggests a very weak positive relationship between these two variables. Since the correlation is weak, it suggests that there isn't a strong tendency for movies with higher popularity ratings to have higher vote_average ratings, or vice versa.

- The correlation coefficient between popularity and vote_count is 0.69. Its is relatively high, indicating a noticeable positive linear relationship  between these two variables.Since the correlation is moderately strong, it suggests that there is a tendency for movies with higher popularity ratings to have higher vote_counts, and vice versa. In other words, movies that are more popular tend to have received more votes.

- The correlation coefficient  between vote average and vote_count is 0.079.Suggests a very weak positive relationship,indicating that there is little to no linear relationship between these two variables.Shows there isn't a strong tendency for movies with higher vote counts to have higher average ratings, or vice versa.


![alt text](Images/image-3.png)

## 2.4 Profitable Movies

In order to determine the profitability of the movies produced.We get to look at the net profit of the movies both Domestic and Worldwide and determine which movies made the most income.


![alt text](Images/image-4.png)


## 2.5 Return on Investment for the movies 

By establishing the return per investment of every movie and then establish the top ten movies with the highest return per investment.This is determined by analysing the cost of production againist the total gross income and this is displayed as percentage of the profit over the cost used to peoduce the movie


![alt text](Images/image-5.png)

## Most profitable movies Studios.

#### Display the top 10 most profitable movies and the years they were produced and the respective studios that produced the movies.
We first calculate the total gross for each movie by adding the domestic and foreign gross.
Then, we sort the DataFrame based on total gross in descending order to identify the most profitable movies.
Optionally, we select the columns 'title', 'total_gross', 'year', and 'studio' to display the top 10 most profitable movies along with their shooting dates and studios.


![alt text](Images/image-6.png)

# Recommendation

### 1. Diversify Genre Selection: 
Consider diversifying the genre selection for the new studio's film productions. While analyzing profitable movies, identify genres that have consistently performed well in terms of profitability and return on investment. By diversifying the genre selection, the studio can mitigate risks associated with relying too heavily on a single genre and appeal to a broader audience base.

### 2.Focus on Audience Engagement: 
Given the moderate correlation between popularity and vote count, prioritize strategies that focus on increasing audience engagement and interaction with the studio's films. This could include leveraging social media platforms, interactive marketing campaigns, and community-building initiatives to foster a loyal fan base and drive word-of-mouth promotion.

### 3.Invest in High-Quality Productions: 
While analyzing the most profitable movies, pay attention to factors contributing to their success, such as production quality, storytelling, and star power. Allocate resources to produce high-quality films that resonate with audiences and differentiate the studio from competitors. Investing in top-notch talent, innovative storytelling techniques, and state-of-the-art production technology can elevate the studio's brand reputation and attract audiences.

### 4. Data-Driven Decision Making:
 Continue leveraging data-driven insights and analytics to inform decision-making processes across all aspects of studio operations. Regularly monitor industry trends, audience preferences, and market dynamics to adapt strategies and optimize resource allocation effectively. Invest in robust data analytics tools and talent to streamline data collection, analysis, and reporting processes, enabling agile decision-making and continuous improvement

 # Conclusion

 In conclusion, our analysis of the box office movies dataset has provided valuable insights to guide strategic decision-making for the launch of our new studio. By examining recent trends, understanding audience preferences, and analyzing the factors contributing to the success of profitable movies, we have identified key opportunities and recommendations to position the studio for success in the dynamic film industry.