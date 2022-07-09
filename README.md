# School_District_Analysis
#### Utilizing Jupyter Notebook, Python, Pandas and Anaconda to clean School District and Student Data

## Overview/Purpose
  Academic dishonesty was shown by data within the students_complete.csv file, though the extent is unknown. To maintain state-testing standards, we've been asked to re-evaluate the data without Thomas High School 9th Graders math & reading test scores and compare the impact of the removal of altered data from the set. 

## Results
  It was important to 'clean' the data to remove the unnecessary prefix & suffixes added to student names initially. After doing this, the data was easier to work with and showed only student names we wanted to evaluate/work with to match School District files. The importance of this could be recognized when attempting to join or combine databases using student names as a key, if the student names in this data don't match the School District's files, it may result in messy, inaccurate data.
  
![CleanPic](/Resources/CleanedStudentData.png)
    
  The instruction given was to replace the ninth grade test scores for math and reading with a 'NaN' value, in order to remove their stats from the overall calculations due to potentially inaccurate numbers reported for Thomas High School. After replacing the data with NaN the results returned were utilized for a repeated analysis. 
  
![NaNPic](/Resources/Thomas9NaNReplace.png)
  
  After removing the inaccurate ninth graders' data from the district's reported data, the overall and average scores showed a minor, almost negligible decrease compared to the original analysis that was run including the potentially falsified scores. 
  
![SummaryPic](/Resources/UpdatedDistrictSummary.png)
  
  The next analysis completed was specific to Thomas High School, to narrow down the impact on the school's data specifically. If the NaN 9th Grader values are included, the averages and overall passing percentages are significantly lower. 
  
 ![IncludeNaNPic](/Resources/StudentDataIncludingNans.png)
  
  If the data is altered to exclude the 9th Graders and combined for 10th-12th Graders, scores, averages, and percentages overall increase dramatically. 
  
 ![10Thru12Pic](/Resources/StudentData10thThru12thNoNaNs.png)
  
  Rerunning the data while excluding the 9th grader data had no significant impact on the top and bottom 5 performing schools, as Thomas High remained in spot number two regardless. 
  
 ![topbottompic](/Resources/TopBottomSchools.png)
  
  Next the data was evaluated to show the comparison of math and reading scores for all schools, separated by grade. (Math on the left, Reading on the right below)
 
![scoresbygradepic](/Resources/MathScoresByGrade.png) ![scoresbygradepic](/Resources/MathScoresByGrade.png)

  Finally the scores of each student/school were evaluated by three different criteria for comparison: school spending, school size, and school type. 
  
![scoresby](/Resources/ScoresBySchoolSpending.png)
![scoresby](/Resources/ScoresBySchoolSize.png)
![scoresby](/Resources/ScoresBySchoolType.png)

## Summary
  After replacing the 9th Grade scores with NaN values, the math and reading scores by grade were mildly altered. The differences were so minor, they would be unnoticed when rounded to the 1st decimal place. Similar notes can be made in regards to the scores by school spending, school size and school type. The main difference noted was the comparison between the scores, percentages and averages in regards specifically to Thomas High School. Because of the low impact on overall data, we can conclude that removing or changing the falsified data from 9th graders at one school has a small impact on the overall outcomes for the School District as a whole. 
