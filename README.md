# School_District_Analysis
## Overview of the school district analysis:
The purpose of this analysis was to use collected data on students and schools within a district in order to present it to the school board. By turning the data into data frames using the pandas library in python, the data is easy to organize and sort for the needs of this analysis. That being said, the math and reading grades for ninth graders at Thomas High school have evidence of academic dishonesty and needed to be replaced. This analysis includes the original goal of the school district analysis while replacing the Thomas High School ninth graders scores to NaN. Replacing these scores means that the previous code may not work properly and changes had to be made.

## Results:
### How is the district summary affected?
- In order for the district summary to work, the number of students in ninth grade at Thomas High School had to be found and subtracted from the district summary.
- This was done by using the loc method on the school_data_complete_df data frame to find the count of the ninth graders. After getting the count, it was then subtracted by the total student count.
![updated_student_count](https://user-images.githubusercontent.com/107213807/177870677-8c06c6f3-b713-4053-9de7-83da9362a583.png)


### How is the school summary affected?
- In order for the school summary to work, the ninth graders from Thomas High School needed to be removed from the count of Thomas High School students, leaving only tenth through twelfth grade. Along with that, the percentages of students passing math, reading, and overall passing percentage needed to be updated to reflect the updated data.
- This was done by finding the count of tenth through twelfth graders and the count of Thomas High School students passing. Using these counts, updated percentages for math, reading, and overall passing were calculated, which then replaced the values in the school summary data frame.
![updated_percentages_thomas](https://user-images.githubusercontent.com/107213807/177870749-b08ac4eb-3433-4d73-88c9-19f47706630e.png)
![replace_percentages](https://user-images.githubusercontent.com/107213807/177870764-93cce090-5e17-4029-ae1a-dc82522e6eae.png)


### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- After replacing the Thomas High School ninth grade scores, the percent of passing in all categories increased and made it to the top two schools

### How does replacing the ninth-grade scores affect the following:
- Math and reading scores by grade
  - The average math and reading scores of ninth graders was replaced with NaN for Thomas High School 
- Scores by school spending
  - The percentages for passing math, passing reading, and overall passing went up for the $631-645 scores.
- Scores by school size
  - The percentages for passing math, passing reading, and overall passing went up for medium school sizes.
- Scores by school type
  - The percentages for passing math, passing reading, and overall passing went up for charter schools. 


## Summary:
Replacing the reading and math scores for ninth graders at Thomas High School led to some changes to the analysis. First off, the math and reading percentages for Thomas High School increased after replacing the values. This is because of the change in student count in relation to the scores from the other grades when calculating the percentages. Since the student count doesn't have ninth graders the percentages increase. This led to changes in the average scores and percentages for scores by school spending, scores by school size, and scores by school type. For all of these, the percentage of overall passing increased for the category Thomas High School falls into for each table ($631-645, Medium, Charter).


