# School_District_Analysis
School District Analysis Assigment

## Overview of Project
    The project is to evaluate different schools in the dataset across different attributes of the data to provide insights into the overall testing results and the results for the different segments in the analysis. The performance analysis in the different segments

### Summary
    The purpose of the assignment is to apply the items we're presented in the online learning, while creating a challenge that uses those same steps to remove some certain records and recalculate the earlier results. Evaluating the differences before and after the changes to the data allow us to examine the differences in the values and how the results are affected without going futher into statistical outlier analysis of the results.

## Deliverables
    1.  Deliverable 1: Replace Ninth-Grade Reading and Math Scores
        a.  I used the loc and np.nan to change the Thomas High School Ninth-Grade test results to NaN
    2.  Deliverable 2: Repeat the School District Analysis
        a.  Repeat the school district analysis you did in this module, and recreate the following metrics:
            i.  The district summary
            ii. The school summary
            iii.The top 5 and bottom 5 performing schools, based on the overall passing rate
            iv. The average math score for each grade level from each school
            v.  The average reading score for each grade level from each school
            vi. The scores by school spending per student, by school size, and by school type
    
### Challenges and Difficulties Encountered
    1.  Converted the Thomas High School 9th grade math and reading scores to NaN values by converting the values to np.nan then convert them from objects to numeric values
    2.  Calculating the average overall scores with the NaN values presented issues, which is why I removed those values from the dataset, this made updating the values redundant because the values matched the values it replaced.

### Results
    1.  How is the district summary affected?
        a.  The Math District Average for Math dropped from 79% to 78.9% (-.1%) showing that the students' average was highter, not significantly higher than the overall average. The Math Passing Percentage increased, 75% to 75.7% (+.7%), partly due to the reduced number of the overall number of students and speaks to the wide range in Thomas High School nineth-grader math scores since the proportion passing math was lower than the other schools in the district.
        b.  The Reading District Average for Reading was unchanged, showing the Average Reading Scores for Thomas High school nineth-graders wasn't significantly higher or lower to affect the overall average. Simlar to Passing Math Percentage, there was an improvement in the Reading Passing Percentage, 86% to 86.7% (.7%).
        c. The Overall Passing Percent (both Math and Reading) improved, 65% to 65.6% (.6%), much like the trends seen in both the Math and Reading Passing Percentages

    2.  How is the school summary affected?
        a.  The number of students was different because I excluded the NaN records from the count, from 1,635 to 1,174. As a result the spending per student increased proportionately.
        b.  The average math scores declined by .07% and the math passing percentage decreased by .09%.
        c.  The average reading scores declined by .05% and the reading passing percentage decreased by .28%.
        d.  The overall passing percentage declined by .31%

    3.  How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
        a.  Overall the Thomas High School remained ranked second for the best Overall Passing Percentage, eventhough it went down, from 90.95% to 90.63% (-.32%).

    4.  How does replacing the ninth-grade scores affect the following:
        a.  Math and reading scores by grade
            i. The only difference is the Thomas High School nineth graders show as NaN, instead of the original result. The other values are unchanged from the original version of the report.
        b.  Scores by school spending
            i.The method I used to remove the number of students resulted in the number of students for Thomas High School, causing the spending per student to increase. This skewed the distribution and resulting precentages.
        c.  Scores by school size
            i.Thomas High School remainded in the same size category, and with the rounding of the percentages, the values remained the same.
        d.  Scores by school type
            i. Thomas High School is a Charter School, and with the rounding of the percentages, the values remained the same.

### Resources
    https://www.statology.org/pandas-replace-values-in-column-based-on-condition/
    https://datatofish.com/create-nan-values-pandas-dataframe/