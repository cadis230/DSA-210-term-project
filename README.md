# DSA-210-term-project

## Project Overview
In this project, I will be investigating how my training content, training participation and weekly throwing hours affect my overall tournament performance in ultimate frisbee. For this purpose, I will be collecting data of my trainings (content, participation), throwing sessions and also my tournament performance data (error type, frequency). By the end of this project, I aim to identify which factors have the major effect on my performance. This project will involve data collection, data cleaning, exploratory analysis and statistical modeling. Eventually, I hope to determine whether there is a correlation between training and tournament performance. 

The plan is to:
Analyze data from practice, throwing sessions and games in tournaments to understand key performance indicators.
Categorize in-game errors (drops/ throwing errors/ miscommunication etc.)
Model the relationship between my training habits and error type/ frequency
Develop insights into which aspects of training most improve tournament performance


## Objectives
### The Training Content
Analyzing what I have been trained for every week. Also, what I have been focused mostly in throwing sessions.

### Identification and Categorization of the Errors
Analyzing every point I have played in tournaments and categorizing my errors. After categorizing, calculating the percentages of my errors.

### Updating My Training Plan
In order to have a better understanding of effects of throwing sessions, I plan to change my throwing hours and investigate whether there is a major chance in my performance.

### Modelling of Training - Performance Relationship
Using statistical and machine learning methods to determine whether training aspects have significant effect on tournament performance.

### Apply Data Science Skills
Applying data analysis and statistical techniques to investigate real-life applications in a systematic way.


## Motivation
This project combines my personal experience as a frisbee player and my interest in data science.
Let's emphasise them one by one:

**Personal Growth**

Understanding the weakest part of my game is very important for me as an athlete and captain. 

**Real-Life Application**

This project is a chance for me to apply concepts that I have been learn in Data Science course while get a chance to improve my athletic statement.

**Long-Term Impact**

By the end of the project, I'll gain a better understanding of both statical modeling and athletic insights. Furthermore, I can apply this technique to the team.

## Dataset
The dataset will be self-collected throughout the trainings and torunamnets. Observation will include followings:

- **Training Date**: The date of each training session  
- **Training type**: Whether it's fundamental or conditioning  
- **Weekly Throwing hours**: Self-rated sleep quality (scale: 1–10)  
- **Attendance(1/0)**: Participation status of training  
- **Match date**: The date of each tournament game 
- **Opponent level(low/medium/high)**:  Comparision of the opponent matching player  
- **Errors per match**: Total errors per game
- **Error types**: Type of error (drop, throwing, miscommunication)
- **Minutes played**: Play duration of me during each game

  ## Tools and Technologies

- **Python**: For data processing, cleaning and analysis
- **Pandas**: For data manipulation
- **Matplotlib/Seaborn**: To generate visualizations
- **Statsmodels**: For regression and model evaluation
- **Excel**: For structured data collection
- **Statto**: For recording data, data preparation

 ## Analysis Plan

 ### Data Collection & Cleaning
 - Record training, throwing and torunmanet data weekly.
 - Standardize variables and handle missing or inconsistent entries.

 ### Data Exploration
 - Visualize the frequency of each error type.
 - Explain trends between throwing session hours and total errors.
 - Compare error distribution.

 ### Hypothesis Testing
 - **H₀:** None of the measured aspects have a major affect on performance  
 - **H₁:** At least one aspect have an affect on performance

 ### Visualization
 - Showing weekly changes in error rate vs. throwing hours by line plots
 - Comparing errors accross training types by using boxplots
 - Coefficient plots for model interpretation

 ### Example Analysis
  - Analyze whether weeks with higher throwing hours correspond to lower error rates in the following tournament matches.
  - Analysis of a scatter plot of weekly throwing hours and total match error rate.
  - A before / after analysis around a targeted period of time to understand if performance is affected significantly.

## Conclusion


