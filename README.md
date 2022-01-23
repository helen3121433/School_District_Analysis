# School_District_Analysis

## Overview: 

The purpose of this analysis is to use Panda and Jupyter Notebook to analyze student funding and students' standardized test score. According to Maria, we'll also need to replace the math and reading scores of 9th graders at Thomas high School with NaNs, then repeat the school district analysis.

For student data, We will first clean student names that make sure the student dataset contains no prefixes(such as Dr, Mr, Ms, etc) and suffixes(such as MD, Ph.D., DDC, etc). Then we start filtering out a list of 9th graders in Thomas High School and replace both math and reading score as NaNs.

Secondly, we will merge both student data and school data into one data frame so that we can repeat the school district analysis. When asking the system to calculate all the count, average, and percentage, the number of 9th graders in Thomas High School will be subtracted from the total amount. We will only be using the student who has the score.


## Resource
Data Resources: 
student_complete.csv
school_complete.csv


## Results: 

Using bulleted lists and images of DataFrames as support, address the following questions.

- District summary was effected that average and % on math score was decreased, and lead overall passing % was decreased.

    Orginal district summary: 
        Average Math score is 79.0
        Average Reading score is 81.9
        % Passing Math is 75%
        % Passing Reading is 85.8%
        % Overall Passing is 65.2%
    
    New district summary (Thomas High school 9th grader score in NaN):
        Average Math score is 78.9
        Average Reading score is 81.9
        % Passing Math is 74.8%
        % Passing Reading is 85.7%
        % Overall Passing is 64.9%

- How is the school summary affected?


- How does replacing the ninth graders’ math and reading 
scores affect Thomas High School’s performance relative to the other schools?
    As mentioned above, if we analyze a report of the total average and percentage passing rate of all 15 school, there's a slight decrease in the total average of math score, and % of passing math rate. However, does not affect the ranking of performing school, Thomas High school still in the second place of top five performing school. 

- How does replacing the ninth-grade scores affect the following:
    Math and reading scores by grade:
        When we run the analysis, it will shows "nan" 9th math and 9th reading score on Thomas High School row. 

    Scores by school spending
        There is not much effect on school spending, even though we're not counting the math and reading scores of all 9th graders in Thomas high school. As the district summary shows above, the overall score was only dropped by 0.3%, so there was not a big change in overall school spending. 

    Scores by school size
        We have a tiny effect when comparing school size vs test scores. The score was decreased on Median school size. But if we round up the result to zero or one decimal, we can't see the difference. We only replace the score of the 9th grader as NaN value but did not replace all names and IDs as NaN.

    Scores by school type
        We have a tiny effect on school type compared with test scores as well. Thomas High School was a Charter school type, so the average and % of test score was decreased. Again, if we round up the result to zero or one decimal place, we can't see the difference. 

## Summary

Overall, there was not much change in the updated school district analysis. The average test score was decreased, the % of test scores was decreased, and this caused the overall % score was decreased. If compared school spending per student vs test score, the test score calculations on spending range at $630-644 was changed. If compared school size vs test score, test score calculations on Median range school was decreased. If compared school type vs test score, calculations on row Charter school type was decreased.