# School District Analysis using Pandas Library and Jupiter notebook

## **Overview of Project**
The objective of this analysis was to assist the chief data scientist, Maria, for a city school disctrict. Maria provided standardized test data for analysis, reporting, and presentation to provide insights about school performance trends and patterns. These insights could be used to inform discussions and strategic decisions at the school and district level. Specifically, she was interested in analyzing data on school funding and students' standardized test scores. Data source for this analysis contained every student's math and reading scores, as well as various information on the schools they attend. The major task was to aggregate the data and showcase trends in school performance.

### Purpose
Specifically, the purpose of this analysis is to use Pandas library along with Jupiter Notebook to automate and simplify the data analysis.


## **Analysis**
Softwares: Pandas Library and Jupiter Notebook 6.4.12

Data source can be found here as a *.csv file: [new_full_student_data](https://github.com/MSF2141/school-district-analysis/blob/fbc0fa4f61a10710b2871d1655e5a3699e1d7506/new_full_student_data.csv).

Complete code can be found here: [Student_Data_Challenge_Starter_Code_MSF](https://github.com/MSF2141/school-district-analysis/blob/0654552ec9349385122775e6bd36f06aa37009be/Student_Data_Challenge_Starter_Code_MSF.ipynb).

First, collected data were imported from a *.csv file to pandas library to be able to work with them. Second, data were prepared for analysis by inspecting and dealing with missing, duplicate, and other messy data. Third, data were analyzed using a three-way approach,i.e., (i) summerization, (ii) targeted analysis, and (iii) aggregated analysis.


## **Results**
Results are printed here as a *.pdf file: [election_analysis](https://github.com/MSF2141/election-analysis/blob/3066d208893af15b7448dfd2b48e40b37a8ce9c4/analysis/election_analysis.txt).


## **Summary**
Preparation for the analysis show that data source contains 1968 empty cells in reading_score column and 982 empty cells in math_score column. There are also 1836 duplicate cells in the data source. In addition, grade column in data source is present as object(string) rather than an integer. After fixing these issues in the initial part of the code "Deliverable 2", the prepared data set contains 14831 row entries and nine columns.

Summerization of the data set show that average value for reading_score, math_score, and school_budget is 72.357865, 64.675733, and 893742.749107, respectively. The min and max values for reading_score is 10.500000 and 100.000000, respectively. The min and max values for math_score is 3.700000 and 100.000000, respectively. Both reading_score and math_score have mean values similar to median values suggesting that the data set has a symmetrical distribution. The same is observed for school_budget. The min and max values for budget_school is 817615.000000 and 991918.000000, repsectively.

Targeted analysis examining the min reading_score (10.5) show the results are from the charter school Dixon High School. Interestingly, students at this school scored much better in math (58.4), which is within the 25th percentile of the school disctrict math results. This school received a below average school funding of 870334 (average: 893742.749107). These results suggest that there may be another factor affecting the test_scores at the school than the school_funding. It would be worth examining further the relationship between fund distribution at a school level and test_score.

Aggregated analysis comparing school funding based on a school type show that public schools on average received more funding than the charter schools, 911195.558251 versus 872625.656236, respectively. Comparing schools based on average math_score show difference among grades and schools. The best mean math_scores are observed at the Fisher High School and Richard High School (both scored 77). Interstingly, both schools belong to schools with the least amount of students attending them. It would be thus worth examining the relationship between fund amount per student and test_score.
