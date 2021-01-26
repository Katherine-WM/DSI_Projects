## Project 1: Standardized Testing, Statistical Summaries and Inference

### Problem Statement
ACT has been more popular than SAT test for many years. The new format for SAT was released in 2016 which cut down both Reading&Writing sections as well as Math sections. In this analysis, we will be going through the average scores and participation rates for 51 states in America in both year 2017 and 2018. This is to help us find out what are the possible strategies that College Board can use to improve the participation rates nation-wide.

### Executive Summary
#### Contents:
1. 2017 Data Import and Cleaning
2. 2018 Data Import and Cleaning
3. Exploratory Data Analysis
4. Data Visualization
5. Descriptive and Inferential Statistics
6. Outside Research
7. Conclusions and Recommendations

### Data Dictionary
Here is the list of features in this data set.

|Feature      |Type  |Dataset     |Description
|:------------|:-----|:-----------|:---------------------------------------------------------------------------
|state        |string|final.csv   |State names of America in this sample
|act17_part   |float |act_2017.csv|State average participation rates for ACT test in 2017(data range: 0%-100%)
|act17_eng    |float |act_2017.csv|State average ACT English scores(data range: 1-36)
|act17_math   |float |act_2017.csv|State average ACT Math scores(data range: 1-36)
|act17_reading|float |act_2017.csv|State average ACT Reading scores(data range: 1-36)
|act17_sci    |float |act_2017.csv|State average score ACT Science scores(data range: 1-36)
|act17_final  |float |act_2017.csv|State average ACT final scores(data range: 1-36)
|sat17_part   |float |sat_2017.csv|State average participation rates for SAT test in 2017(data range: 0%-100%-36)
|sat17_rw     |float |sat_2017.csv|State average SAT Reading&Writing scores(data range: 200-800)
|sat17_math   |float |sat_2017.csv|State average SAT Math scores(data range: 200-800)
|sat17_final  |float |sat_2017.csv|State average SAT final scores(data range: 400-1600)
|act18_part   |float |act_2018.csv|State average participation rates for ACT test in 2018(data range: 0%-100%)
|act18_eng    |float |act_2018.csv|State average ACT English scores(data range: 1-36)
|act18_math   |float |act_2018.csv|State average ACT Math scores(data range: 1-36)
|act18_reading|float |act_2018.csv|State average ACT Reading scores(data range: 1-36)
|act18_sci    |float |act_2018.csv|State average score ACT Science scores(data range: 1-36)
|act18_final  |float |act_2018.csv|State average ACT final scores(data range: 1-36)
|sat18_part   |float |sat_2018.csv|State average participation rates for SAT test in 2018(data range: 0%-100%-36)
|sat18_rw     |float |sat_2018.csv|State average SAT Reading&Writing scores(data range: 200-800)
|sat18_math   |float |sat_2018.csv|State average SAT Math scores(data range: 200-800)
|sat18_final  |float |sat_2018.csv|State average SAT final scores(data range: 400-1600)

### Conclusions and Recommendations
Based on the analysis above, it is noticed partnership with state government to give discount on test fee and also the subsequent fee waiver policy given by state government is the major reason for significant increase in participation rate in 2018. With fees waived, students in the from low-income families now have chance to take the test and show their academic capabilities to colleges. In addition, students who took the test under fee waiver policy will go to an express College application channel which makes application for loans and grants easier.

Apart from partnership, it is studied that families with college-educated parents are likely to ask their children to pursue a college degree as well. In addition, income level for such families are generally higher and they can financially support their children to take the test multiple times to boost up their score and slso to give them enough support during their college time. Therefore, College Board should advertise more in wealthier states to boost participation rates.

Therefore, based on above analysis, we can choose South Dakota to implement state policy to mandate SAT test. Among the five staets with the lowest participation rates, only South Dakota does note have a preferencebetween SAT and ACT test while the rest of the states require ACT exam[1].

The above conclusion are drawn based on the data given. However, the datasets given are not a good representation of the entire student population. More information on sample size and student demographics should be given to have a better conclusion.