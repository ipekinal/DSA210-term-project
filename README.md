# 🎥💸 Movie Budgets vs. Genres & IMDb Ratings 🎬🍿

## Project Overview & Motivation 


## Data Source: Where did I get this data? How did I collect it? 🌐
IMDb has a different website called “IMDb developer” and it has non-commercial datasets. From there, I downloaded 2 datasets. The first one was a huge dataset named “title basics” which consists of the unique alphanumeric identifier, title type, popular title, original title, release year, and genres of movies. The second one was called “title ratings” and had information about the unique alphanumeric identifier, weighted average of all the individual user ratings, and number of votes of movies.

From the first dataset, I filtered the movies in the last 25 years (since otherwise I failed to see the end of my code’s execution after several hours of trying to keep the runtime connected). Then, I matched the unique identifier of movies in “title basics” to the unique identifiers in “title ratings” since not all the movies in the first set was included in the second one. After merging them, I had to get the data about budget and revenue.

The Movie Database offers an extensive API service for free. I created an account and managed to get a personalized API key for access. With the help of ChatGPT, I pulled the information of budget and revenue from TMDB that once again corresponded to the titles that I merged earlier with movie names, genres and ratings. At last, I successfully got a file named “movies_after_2000” with 1000 entries that had the following attributes: title, release year, IMDb rating, genre, budget, revenue.

## Data Analysis: Techniques and Stages of Analysis 🔍
- Data Collection - throughout March and April, maintaining:
  - the same student (me)
  - amounts measured in the same unit (mg) across different drinks
  - sleep durations measured in the same unit (hours and minutes)
  - study session durations measured in the same unit (hours and minutes)
- Data Cleaning
  - identifying and considering external factors that may hinder my studying duration such as:
    - serious sleep deprivation - lack of sleep may inevitably reduce long durations of studying regardless of caffeine intake after a certain point
    - distractions - my friends inviting me for a break outside IC may impede my productivity regardless of caffeine intake
- Correlation Analysis
  - calculating the correlation coefficient - to determine if there is a positive/negative correlation or no relationship between the amount of caffeine consumed and the sleep duration vs. how productive I was while studying 
  - visualizing trends using scatter plots - to ease identifying the relationships mentioned above and whether it is strong/weak/nonexistent

## Hypotheses to Test 📊
1) Caffeine affects study duration.
- 1st Null Hypothesis (H₀): There is no significant difference in study duration with and without caffeine consumption.
- 1st Alternative Hypothesis (H₁): Study duration increases with caffeine consumption.

2) Sleep duration influences study duration.
- 2nd Null Hypothesis (H₀): Sleep duration has no significant effect on study efficiency.
- 2nd Alternative Hypothesis (H₁): Longer sleep duration contributes to increased study productivity.

3) The interaction of caffeine intake and sleep affects study efficiency.
- 3rd Null Hypothesis (H₀): There is no interaction effect between caffeine intake and sleep duration on study duration.
- 3rd Alternative Hypothesis (H₁): A combination of optimal sleep and moderate caffeine intake results in the highest study efficiency.

## Acknowledgement
Assistance with specific technical components like Markdown formatting, and hypothesis layout was provided using ChatGPT by OpenAI (2024), based on user-generated data and user-generated context.
