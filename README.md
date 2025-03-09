# ☕️⚡️ Daily Caffeine Intake vs. Studying Time 📚✍️

## Project Overview & Motivation 
The savior of students worldwide, enabling us to stay awake and study for long hours, is often caffeine, usually in the form of coffee or energy drinks.

Being a hardworking student while also being a chronic procrastinator is not for the faint of heart. Especially when deadlines and exams are right around the corner, I frequently find myself struggling to stay awake while simultaneously suffering from sleep deprivation.

The most common and seemingly effective solution? Caffeine consumption.

However, I dislike drinking coffee out of obligation. This led me to question: Does caffeine truly enhance productivity, or is it merely a psychological boost that makes me believe I can study longer by the aid of an external energy source?

Through this project, I aim to determine whether caffeine (sadly) has a real positive impact on my study efficiency or if the perceived benefits are simply a placebo effect.

## Data Source: Where did I get this data? How did I collect it? ⏱
To track caffeine intake, I will use the HiCoffee - Caffeine Tracker app on iOS. This app allows users to log coffee and energy drink consumption while recording the exact time of intake. It includes a database of various beverages from brands like Starbucks, Nespresso, and Monster, along with an option to manually input drinks with their corresponding caffeine amounts, which are typically available on official brand websites.

To measure my study productivity, I will use a simple stopwatch (available on Google) to record the duration of my study sessions before and after consuming caffeine. Additionally, I will record:
- The time of caffeine intake
- The type and amount of caffeine consumed
- How long I studied before and after consumption
- My subjective focus level (on a scale from 1 to 10)

This data will help me determine if caffeine affects study efficiency and whether the timing of intake plays a role.

## Data Analysis: Techniques and Stages of Analysis 🔍
- Data Collection - throughout March and April, maintaining:
  - the same student (me)
  - amounts measured in the same unit (mg) across different drinks
  - study session durations measured in the same unit (minutes or hours)
- Data Cleaning
  - identifying and considering external factors that may hinder my studying duration such as:
    - serious sleep deprivation - lack of sleep may inevitably reduce long durations of studying regardless of caffeine intake after a certain point
    - distractions - notifications from social media or my friends inviting me for a break outside IC may impede my productivity if it occurs frequently
- Correlation Analysis
  - calculating the correlation coefficient - to determine if there is a positive/negative correlation or no relationship between the amount of caffeine consumed and how productive I was while studying
  - visualyzing trends using scatter plots - to ease identifying the relationship mentioned above and whether it is strong/weak/nonexistent

## Hypotheses to Test 📊
1) Caffeine increases study duration.
- 1st Null Hypothesis (H₀): There is no significant difference in study duration before and after caffeine consumption.
- 1st Alternative Hypothesis (H₁): Study duration increases after caffeine consumption.

2) The timing of caffeine intake affects productivity.
- 2nd Null Hypothesis (H₀): The time at which caffeine is consumed has no effect on study efficiency.
- 2nd Alternative Hypothesis (H₁): Caffeine consumed earlier in the day results in longer study sessions compared to consumption later in the day.
