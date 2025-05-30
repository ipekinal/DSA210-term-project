# 🎥💸 Movie Budgets vs. Genres & IMDb Ratings 🎬🍿

## Project Overview & Motivation 
Although it has been quite some time since I went to a movie theater, the film industry is still one of the largest and most dynamic sectors in the global economy. Yet, the relationship between a movie’s financial details, genre, and its critical reception is often complex. 

As a Letterboxd enthusiast, this project was driven by a motivation to explore what factors actually influence a movie’s success, both in terms of financial performance and audience ratings.

By examining real-world data from the 21st century, I aimed to find out whether high budgets guarantee high ratings, whether some genres are more profitable than others, and if we can reliably predict revenue from basic features like budget and genre. The ultimate goal was to bridge storytelling with data, revealing patterns that could be useful to both movie enthusiasts and industry analysts.

## Data Source: Where did I get this data? How did I collect it? 🌐
IMDb has a website called “IMDb developer” and it has non-commercial datasets. From there, I downloaded 2 datasets. The first one was a huge dataset named “title basics” which consists of the unique alphanumeric identifier, title type, popular title, original title, release year, and genres of movies. The second one was called “title ratings” and had information about the unique alphanumeric identifier, weighted average of all the individual user ratings, and number of votes of movies.

From the first dataset, I filtered the movies in the last 25 years (since otherwise I failed to see the end of my code’s execution after several hours of trying to keep the runtime connected). Then, I matched the unique identifier of movies in “title basics” to the unique identifiers in “title ratings” since not all the movies in the first set was included in the second one. After merging them, I had to get the data about budget and revenue.

The Movie Database offers an extensive API service for free. I created an account and managed to get a personalized API key for access. With the help of ChatGPT, I pulled the information of budget and revenue from TMDB that once again corresponded to the titles that I merged earlier with movie names, genres and ratings. At last, I successfully got a file named “movies_after_2000” with 1000 entries that had the following attributes: title, release year, IMDb rating, genre, budget, revenue.

## Data Analysis: Techniques and Stages of Analysis 🔍
After finishing up with data cleaning and preprocessing, I then calculated a key financial metric: Return on Investment (ROI), to better assess profitability.

The analysis proceeds in several stages:
- Correlation Analysis: Using genre-level aggregates, I built a correlation matrix to assess how average budget, revenue, rating, and ROI relate across genres.
- Statistical Testing: A Chi-square goodness-of-fit test was conducted to evaluate whether movie genres are evenly distributed, revealing significant genre dominance.
- Visualizations: I created scatter plots, bar charts, and heatmaps to visually compare metrics across genres and over budget/revenue scales.
- Machine Learning Models: I trained a Random Forest Regressor and K-Nearest Neighbors (KNN) to predict a movie’s revenue using budget and one-hot encoded genre data, evaluating performance using R² and Mean Squared Error.

Each of these steps helped build a multidimensional understanding of the film dataset, using both statistical inference and predictive modeling.

## Hypotheses to Test 📊
1) Budget and IMDb ratings
   - Null: Budget and IMDb ratings do not have a significant correlation.
   - Alternative: Budget is positively correlated with IMDb rating.
Tested using Pearson’s correlation and scatter plots with trendlines.

 2) Revenue and IMDb ratings
   - Null: Revenue and IMDb ratings do not have a significant correlation
   - Alternative: Revenue is positively correlated with IMDb rating.
Tested with Pearson’s correlation.

 3) Among genres
  - Average IMDb ratings, budgets, and revenues differ significantly between genres.
Tested using ANOVA (Analysis of Variance) across genre groups.

 4) Genre distribution
  - Genres are equally represented in the dataset.
Tested using a Chi-square goodness-of-fit test.

  5) Revenue prediction
  - Budget and genre information of movies can reliably predict revenue.
Evaluated using Random Forest and KNN models, judged by R² and MSE.

## Acknowledgement
Assistance with specific technical components like Markdown formatting, hypothesis layout, and certain analysis details was provided using ChatGPT by OpenAI (2024), based on user-generated data and user-generated context.
