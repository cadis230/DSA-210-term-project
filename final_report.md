# Performance Analysis for Ultimate Frisbee through Error Rate and Training Data 

## Abstract 

This study examines how training content, training participation, and weekly throwing hours influence overall tournament performance in ultimate frisbee. Data on training participation, training type, and weekly throwing hours were collected across several weeks to assess whether these factors affect error rates during tournaments. The study also investigates the relationship between these training-related features and different types of errors. Using Python-based statistical analysis and data visualization, the project identifies key variables associated with performance and presents a data-driven approach to improving athletic outcomes.


## 1. Introduction
Tournament performance in ultimate frisbee is influenced by multiple training-related factors, including training content, training participation, and individual practice habits such as throwing frequency. In-game error rates offer a detailed and objective measure of player effectiveness. Understanding how training structure and workload relate to these errors is essential for improving performance in a systematic manner. 

The aim of this study is to evaluate how different aspects of training relate to tournament error patterns in ultimate frisbee. By focusing on error-based performance metrics, the study seeks to provide a clearer understanding of how training structure and individual practice habits influence competitive performance.

## 2. Methodology

### 2.1 Data Collection
Data was manually recorded after each of 23 training sessions and 3 tournaments. Attributes include:

- **Training Date**: The date of each training session  
- **Training type**: Whether it's fundamental or conditioning  
- **Weekly Throwing hours**: Self-rated sleep quality (scale: 1–10)  
- **Attendance(1/0)**: Participation status of training  
- **Match date**: The date of each tournament game 
- **Opponent level(low/medium/high)**:  Comparision of the opponent matching player  
- **Errors per match**: Total errors per game
- **Error types**: Type of error (drop, throwing, miscommunication)
- **Minutes played**: Play duration of me during each game

### 2.2 Data Processing 
All data were manually recorded in a structured and standardized format during the data collection phase. As a result, no additional data cleaning procedures such as handling missing values or removing duplicate entries were required.

To ensure temporal consistency, training participation, training content, and weekly throwing hours were aligned with tournament performance based on match dates. For each tournament game, only training and throwing data collected prior to the tournament date were included in the analysis. This approach prevented possible data leakage.

Training-related data were grouped according to tournament periods. Weekly observations leading up to each tournament were aggregated to represent the overall training profile associated with that tournament. Aggregated features included measures such as average weekly throwing hours, total training participation, and dominant training type during the pre-tournament period.

These processed features were then used as input variables for statistical analysis and performance evaluation.

### 2.3 Tools Used

- **Excel**: First data collection
- **Python**: Language for data processing  
- **Pandas**: Dataset manipulation  
- **Seaborn & Matplotlib**: Visualization  
- **Statsmodels & SciPy**: Statistical analysis
- **Statto**: For recording data, data preparation

## 3. Exploratory Data Analysis (EDA)
Exploratory Data Analysis (EDA) was conducted to understand the structure of the dataset and to identify preliminary relationships between training-related variables, match exposure, opponent characteristics, and error outcomes. The dataset contained training records (training participation and weekly throwing volume) and match-level performance metrics, including total errors, error subtypes, minutes played, and opponent level. Training attendance and training type is not included since there is no difference in data contribute to analysis. 

Initial descriptive analysis revealed substantial variation in both training load and match exposure across tournaments. Weekly throwing hours prior to tournaments varied notably, allowing for meaningful comparisons between low- and high-volume preparation periods. Similarly, minutes played differed considerably between matches, reflecting differences in game involvement and exposure to in-game decision-making situations.

Analysis of error composition showed that throwing-related errors constituted the largest proportion of total errors, followed by drops and miscommunication errors. This distribution suggests that technical execution, particularly under match pressure, plays a dominant role in overall performance variability.

Bivariate visualizations indicated a positive association between minutes played and total errors, suggesting that increased match exposure is associated with a higher likelihood of committing errors. In contrast, higher weekly throwing volume prior to tournaments appeared to be weakly associated with fewer throwing errors, implying a potential protective effect of consistent technical practice. Additionally, error distributions differed across opponent levels, with matches against higher-level opponents exhibiting higher median error counts and greater variability.

Overall, the EDA phase suggested that both training-related factors and contextual match factors may contribute to error occurrence, justifying the use of a multivariate statistical model to assess their relative influence while controlling for confounding effects.

## 4. Statistical Modeling: Results and Discussion
To quantify the relative impact of training load, match exposure, and opponent level on performance, a multivariate linear regression model was fitted with total errors as the dependent variable. Independent variables included weekly throwing hours prior to tournaments, minutes played, and opponent level, with medium-level opponents used as the reference category. All predictors were standardized prior to modeling to allow for direct comparison of effect sizes.

The results of the regression analysis indicated that minutes played was the strongest predictor of total errors. The positive standardized coefficient suggests that increased on-field exposure leads to higher error counts, likely due to accumulated fatigue, increased decision-making demands, and greater involvement in high-pressure situations. This finding aligns with the exploratory analysis and supports the interpretation that match exposure is a primary driver of error accumulation.

Weekly throwing volume prior to tournaments exhibited a negative association with total errors. Although its effect size was smaller than that of minutes played, the direction of the relationship suggests that consistent throwing practice may reduce error frequency by improving technical stability and execution under competitive conditions. This finding highlights the importance of sustained skill-specific training as a mitigating factor against in-game errors.

Opponent level also contributed meaningfully to model outcomes. Matches against high-level opponents were associated with increased error counts relative to medium-level opponents, indicating that higher competitive intensity and defensive pressure elevate the likelihood of mistakes. Conversely, matches against low-level opponents tended to be associated with fewer errors, reflecting reduced performance pressure and simpler in-game situations.

Taken together, the model demonstrates that total error occurrence is influenced by a combination of exposure-driven factors (minutes played), preparatory factors (weekly throwing volume), and contextual difficulty (opponent level). While the model does not capture all sources of performance variability, it provides a coherent and interpretable framework for understanding how different aspects of preparation and competition interact to shape error outcomes. These findings suggest that optimizing training volume and managing match exposure, particularly against high-level opponents, may be effective strategies for reducing performance errors.

## 5. Conclusion
This study examined the relationship between training load, match exposure, and contextual match factors in explaining error occurrence in ultimate frisbee tournaments. By integrating training records with match-level performance data, the analysis aimed to identify which aspects most strongly contribute to total errors during competition.

The findings indicate that minutes played is the most influential factor associated with total errors, suggesting that increased on-field exposure substantially elevates the likelihood of committing mistakes. This relationship highlights the role of accumulated fatigue, cognitive load, and repeated decision-making demands during extended match participation. In contrast, weekly throwing volume prior to tournaments demonstrated a protective effect, with higher throwing volumes associated with reduced error counts. This result underscores the importance of consistent technical preparation in stabilizing performance under competitive conditions.

Additionally, opponent level emerged as a meaningful contextual factor. Matches against higher-level opponents were associated with increased error rates relative to medium-level opponents, while matches against lower-level opponents tended to produce fewer errors. This finding emphasizes the impact of competitive difficulty and external pressure on performance outcomes.

Overall, the results suggest that performance errors in ultimate frisbee are not solely a function of individual skill, but rather the combined outcome of training preparation, match exposure, and competitive context. From a practical perspective, these findings imply that optimizing throwing-focused training volume and strategically managing playing time, particularly in high-level matches may help mitigate error occurrence and improve overall performance consistency.

## 6. Limitations
The analysis is based on a relatively small dataset derived from a single athlete, which limits the generalizability of the findings. In addition, training variables were self-reported and primarily quantitative, and therefore do not fully capture training quality, intensity, or recovery status. Finally, the use of a linear regression framework assumes linear relationships and treats error counts as continuous variables, which may not fully reflect the underlying structure of performance data.

## 7. Future Work
Future research could extend this analysis by incorporating larger datasets across multiple players and competitive levels to improve robustness and generalizability. Including additional variables such as training intensity, fatigue indicators, and recovery metrics may provide a more comprehensive understanding of performance dynamics.s