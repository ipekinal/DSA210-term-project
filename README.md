# ☕️⚡️ Caffeine Intake & Sleep Duration vs. Studying Time 📚✍️

## Project Overview & Motivation 
The savior of students worldwide, enabling us to stay awake and study for long hours, is often caffeine, usually in the form of coffee or energy drinks.

Being a hardworking student while also being a chronic procrastinator is not for the faint of heart. Especially when deadlines and exams are right around the corner, I frequently find myself struggling to stay awake while simultaneously suffering from sleep deprivation.

Hence, I find myself questioning whether I should drink a coffee and continue studying, or get a good night's sleep and continue tomorrow.

This led me to question: Does caffeine truly enhance productivity, or is it merely a psychological boost that makes me believe I can study longer by the aid of an external energy source? Moreover, does the quality and duration of sleep play a larger role than caffeine intake alone?

At the end of this project, I hope to uncover whether caffeine compensates for sleep deprivation or if proper sleep habits contribute more effectively to increased productivity.

## Data Source: Where did I get this data? How did I collect it? ⏱
To track caffeine intake, I will use the HiCoffee - Caffeine Tracker app on iOS. This app allows users to log coffee and energy drink consumption while recording the exact time of intake. It includes a database of various beverages from brands like Starbucks, Nespresso, and Monster, along with an option to manually input drinks with their corresponding caffeine amounts, which are typically available on official brand websites.

To track my sleep duration and quality, I will use Apple's Health App together with Sleep Cycle app on iOS. Both of these apps have automatic and manual functions to measure sleep quality. I will log the time I go to sleep, the average time it takes for me to fall asleep, and the time I wake up. Sleep Cycle app also lets the user record sounds over the night to find out whether the user woke up during sleeping to measure the sleep quality.

To measure my study productivity, I will use a simple stopwatch (available on Google) to record the duration of my study sessions before and after consuming caffeine. Additionally, I will record:
- the time of caffeine intake
- the type and amount of caffeine consumed
- how long I studied before and after consumption
- the time I went to sleep compared to the proximity of consuming caffeine
- sleep duration compared to the amount of caffeine consumed that day

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
  - visualyzing trends using scatter plots - to ease identifying the relationships mentioned above and whether it is strong/weak/nonexistent

## Hypotheses to Test 📊
1) Caffeine affects study duration.
- 1st Null Hypothesis (H₀): There is no significant difference in study duration before and after caffeine consumption.
- 1st Alternative Hypothesis (H₁): Study duration increases after caffeine consumption.

2) Sleep duration influences study duration.
- 2nd Null Hypothesis (H₀): Sleep quality and duration have no significant effect on study efficiency.
- 2nd Alternative Hypothesis (H₁): Higher sleep quality and longer sleep duration contribute to increased study productivity.

3) The interaction of caffeine intake and sleep affects study efficiency.
- 3rd Null Hypothesis (H₀): There is no interaction effect between caffeine intake and sleep quality on study duration.
- 3rd Alternative Hypothesis (H₁): A combination of optimal sleep and moderate caffeine intake results in the highest study efficiency.
