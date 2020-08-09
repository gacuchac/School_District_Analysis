# School District Analysis
## Overview of the School District Analysis
Based on standarized math and reading tests results, we analyse the overall district's and schools' performance. Various statistical summaries are generated to show all the requested information. Given the fact that there is evidence of academic dishonesty; specifically in the reading and math grades for *Thomas High School* ninth graders (461 students, 1.2% of total students) we compare the results with and without those grades. It is important to highlight that since we are only setting as *null* the math and reading scores, the *Student ID* column is kept and therefore the amount of students in the school does not change.

## Results
When comparing the dataset with and without the *Thomas High School* ninth graders scores we get the following results:

- District Summary
We can see a small decrease of about a 1% in all scores when not considering *Thomas High School* 9<sup>th</sup> graders scores. This makes sense since it means that when we are no longer considering the altered scores, it goes down on the same amount, meaning that they are all above the mean as we can see in the table.

District Summary                               | Image
:---------------------------------------------:|:-------------------------------------:
District Summary Complete                      | ![](Resources/District_Summary_Complete.png)
District Sumary without 9<sup>th</sup> graders | ![](Resources/District_Summary_NaN.png) 
*Thomas High School* 9<sup>th</sup> graders    | ![](Resources/District_Summary_ths.png) 

- School Summary
When comparing the results obtained by *Thomas High Scholl* with and without the 9<sup>th</sup> graders scores, we see that the average does not change much. That is because the *pandas* library does not count the *NaN* values when calculating the mean of the column. What changes dramatically is the percentage of students passing the tests. That is because the percentage is calculated with the total amount of students and when setting the 9<sup>th</sup> graders scores to *NaN* we are failing them, so a drop in about 30% makes sense since we are failing a whole grade.
 
School Summary Complete                        | School Sumary without 9<sup>th</sup> graders
:---------------------------------------------:|:-------------------------------------:
![](Resources/School_Summary_Complete.png)     | ![](Resources/School_Summary_NaN.png)

- *Thomas High School* in relation to other schools
As seen in the following image, when ranking by *% Overall Passing*, *Thomas High School* drops from 2<sup>nd</sup> to 8<sup>th</sup> place. This is consistent with the previous analysis, where the important drop was in the *% Passing* columns due to the failing grades of the 9<sup>th</sup> graders.

School Summary Complete                        | School Sumary without 9<sup>th</sup> graders
:---------------------------------------------:|:-------------------------------------:
![](Resources/School_Summary_Complete_Sorted.png)     | ![](Resources/School_Summary_NaN_Sorted.png)