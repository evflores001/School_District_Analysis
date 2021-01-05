# School_District_Analysis
---

## Overview

The purpose of this analysis was to find trends in both school and student performance based on specified parameters. Using Python and the pandas library within jupyter notebook, two different CSV files containing both student and school information were analyzed, merged, and modified. Both these datasets were merged using the pandas merge function, allowing the information of a student and their respective school to live within the same dataset. Using this initial dataset paved way into finding datasets containing the total school count, total students, total school budget, average math and reading score, as well as the percentage of students passing math, reading, and both; similarly, the dataset containing the breakdown of the aforementioned values for school was found in the school summary dataframe. Some other key datasets that were derived were the top and bottom five performing schools, the average reading and math scores per grade for each school, and student scores based on school spending per student, by school size, and by school type. 

For the purposes of this analysis, some of the values in the student_complete.csv file were modified. The reading and math scores for all 9th grade students attending Thomas High School were assigned NaN values using NumPy. This resulted in changes to the several forenamed datasets. 

## Results 
### Changes to Disctrict and School Summary Dataframes
The results from altering the grades for the students attending Thomas High are compareable to the dataframes initially obtained. The first change can be observed when comparing the original district summary dataframe with that of the dataframe containing the altered grades
![](https://github.com/evflores001/School_District_Analysis/blob/master/Resources/DataFrameShots/district_summ_init.png)
![](https://github.com/evflores001/School_District_Analysis/blob/master/Resources/DataFrameShots/district_summary_shot_mod.png)
The dataframe containing the altered grades sees a drop for the average math score as well as all percent passing scores.

The school summary dataframe also saw a change in some of the values regarding Thomas High school. The following dataframes present the original school summary dataframe and altered school summary, respectively.
![](https://github.com/evflores001/School_District_Analysis/blob/master/Resources/DataFrameShots/school_summ_init.png)
![](https://github.com/evflores001/School_District_Analysis/blob/master/Resources/DataFrameShots/school_summary_shot_mod.png)
Similarly to the district summary dataframe, the average math and overall passing grades drop slightly; only the average reading score sees a slight increase.

Although replacing the grades for students attending Thomas High School drop some of the average and percentage of students passing, compared to other schools, Thomas High School holds the second place for the top-five schools in the district.

### Other changes
Removing all math and reading scores for ninth graders attending Thomas High School caused the average math and reading scores by grade to be replaced with *"nan"* as can be seen in the following [math](https://github.com/evflores001/School_District_Analysis/blob/master/Resources/DataFrameShots/math_scores_by_grade_shot_mod.png) and [reading](https://github.com/evflores001/School_District_Analysis/blob/master/Resources/DataFrameShots/reading_scores_by_grade_shot_mod.png) score by grade, respectfully.

There were no changes to the scores by [school spending](https://github.com/evflores001/School_District_Analysis/blob/master/Resources/DataFrameShots/scores_by_school_spending_shot_mod.png), [scores by school size](https://github.com/evflores001/School_District_Analysis/blob/master/Resources/DataFrameShots/scores_by_school_size_shot_mod.png) or the [scores by school type](https://github.com/evflores001/School_District_Analysis/blob/master/Resources/DataFrameShots/scores_by_school_type_shot_mod.png) dataframes.

## Summary
After the reading and math scores for the ninth graders at Thomas High School were replaced with NaNs, the major changes to the school district analysis are as follows:

- Both the distric summary and school summaty dataframes saw a slight drop in average math and percent passing scores
- Those same dataframes saw an increase in the average reading scores
- Both the math and reading scores by grades dataframes had an *"nan"* for 9th grade students at Thomas High School

Overall, Thomas High School held its place as the second best performing school based on the percent of overall passing.

