# An Analysis of A List of Schools in A Single School District

### Jupyter Notebook File:
[PyCitySchools_Challenge](PyCitySchools_Challenge.ipynb)

### School District CSV Files:
- [schools_complete](Resources/schools_complete.csv)
- [students_complete](Resources/students_complete.csv)
- [clean_students_complete](Resources/clean_students_complete.csv)

## **Overview**:

The purpose of this analysis was to present the most descriptive conclusions about the school district's list of schools and the performance of their students. The analysis involves two different instances of analyzing the district's data, one that analyzed all of the data included in the CSV files from the schools in the district and a second instance where all data involving the 9th grade student records from Thomas High School was removed due to concerns about the data's accuracy and integrity. This analysis carried out using Pandas with Python code in the Jupyter Notebook application to read and analyze two CSV file datasheets. Through the Jupyter Notebook file, code blocks were constructed to yield specific summaries of the data analysis and each summary was built upon for increasingly narrowed conclusions from the data.

## **Results**:
Overall, following the removal of the invalid 9th grade data of Thomas High School from the various analyses, the conclusions seem to have been only slightly impacted. Though the numbers with more precise results show an impact in the decimal values, with respect to each relevant section of the tables created, the change of dropping the invalid data seemed to only sometimes make an impactful change to the formatted values that were rounded to be easier to read. Some of the key conclusions are presented below along with screenshots of the summaries from both analyses to give a clear idea of how the adjusted data impacted the subsequent calculations for the school district.

### District Summary:
The values in the district's summary, for the most part, have each been slightly decreased - with an exception for the "Average Reading Score", which remained the same.
- Original Summary (Left) / Updated Summary (Right)
![district_summary](Resources/district_summary.png)
	
### School Summary:
The values in the individual schools summary have, obviously, remained the same for all other schools except Thomas High School. Most of the concusions to the updated analysis have decreased slightly, the exception being the "Average Reading Score", which increased slightly. For the values that are impacted by the updated data for Thomas High School the changes were:
  - Average Math Score: -0.067 points	- Average Reading Score: +0.047	points	- % Passing Math: -0.0865 %	- % Passing Reading: -0.29 % 	- % Overall Passing: -0.318 %
- Original Summary (Left) / Updated Summary (Right)
![school_summary](Resources/school_summary.png)
		
### Thomas High School Performance Changes:
For the most part, though the removal of the 9th grade data from the Thomas High School analyses has led to lower values in most of the results, Thomas High School has remained the second best school in the district by the "% Overall Passing" value. The updated analysis has caused the best-performing school of Cabrera High School to stand out more with a greater percentage of overall passing students. Despite this, the difference between Thomas High School's initial value in the column and the updated value was less than half a percentage point, making the rounded whole number result for the section the same in both cases for Thomas High School and the same as Cabrera High School's rounded performance value.
- Original Summary (Left) / Updated Summary (Right)
![top_lower_performing_schools](Resources/top_lower_performing_schools.png)

### Changes in Math and Reading Scores by Grade:
By removing the 9th grade data for Thomas High School, one of the two values tied for second-best in the "9th Grade Average Math Scores" category is removed - meaning the overall performance of "9th Grade Average Math Scores" across the schools is slightly worse than when the invalid data was included.
- Original Summary (Left) / Updated Summary (Right)
![school_math_scores_by_grade](Resources/school_math_scores_by_grade.png)

Unlike the impact of removing the 9th grade data from the "9th Grade Average Math Scores", the performance of the 9th grade in Thomas High School's "9th Grade Average Reading Scores" was slightly closer to the median of the other values in 9th grade reading scores, meaning there wasn't as big of an impact from removing the data from Thomas High School.
- Original Summary (Left) / Updated Summary (Right)
![school_reading_scores_by_grade](Resources/school_reading_scores_by_grade.png)
  
### Scores:
1. With Thomas High School's Per-Student Budget value of $638.00, it falls under the $630-644 per student range, and the impact of removing the 9th grade data made no impact on the results when combined with the other schools in its spending per student range and formatted to round off the numbers.
- Original Summary (Left) / Updated Summary (Right)
![score_per_student_spending](Resources/score_per_student_spending.png)
2. Similarly, with the student population of 1,635 for Thomas High School, it falls under the "Medium (1000-2000)" school size, and the removal of the 9th grade data made no impact in the resulting analyses when Thomas High School's performance is included with the rest of the data from other schools of similar size and the values are formatted to round off the decimal points.
- Original Summary (Left) / Updated Summary (Right)
![school_scores_by_size](Resources/school_scores_by_size.png)
3. Once again, when the data for Thomas High School is updated and an analysis is done with its data included with schools of similar type, the results were not different enough to change the values once they were formatted to round off the decimals. For this summary, instead of presenting the rounded values, the unformatted values presented show that there is indeed an impact made from changing the 9th grade values for Thomas High School, but it is indeed very rarely noticable with the final formatting across each analysis.
- Original Summary (Left) / Updated Summary (Right)
![school_scores_by_type](Resources/school_scores_by_type.png)

## **Summary**:
With the removal of the 9th grade scores, the results for each analysis involving this data were impacted very slightly and often to an extent too small to notice when the numbers were formatted for better presentation. Though the changes that came from the adjusted data values were small, they were not insignificant in several cases shown from this updated analysis. The most clear cases of this updated data changing the results of an analysis were:

1. The "Average Reading Score" value for the school actually improved after the 9th grade's data was removed, marking the only case of a clear improvement for the school by removing an entire grade's data values. In addition to this case being an exception to other changes in the results of this analysis without the invalid data, the change was large enough to impact the formatted values, since this result reflected the school itself instead of factoring in other school's data and making the impact from removing this data less clear.
2. Another clear change in the results of these analyses was the drop in students passing reading, with the change being 0.29% less than the initial analysis. This means that while 9th grade students performed at a lower level than the other grades in reading, they had a larger number of passing grades that was able to lift the number of passing students in reading when the invalid data was still included in this analysis.
3. As was shown in the previous case of the reading scores at Thomas High School and the percentage of students that passed reading, the number of passing students present in the invalidated 9th grade data was able to raise Thomas High School's "% Overall Passing" value around 0.30% and bring it to a middle ground between the highest performing school in the district and the third-best performing school in the district. Without the 9th grade data, Thomas High School's overall performance was brought closer the other schools below it in the list of top schools and left the top-performing school seeming slightly more exceptional among the other schools listed.
4. A fourth change that was noticed when analyzing the two different data sheets was the District Summary that included the performances from all of the different schools in the district. The changes were mostly a slight drop that amounted to a loss of nearly .1 to each resulting value, with the exception of two sections: the "% Passing Reading" and the "Average Reading Score". The "% Passing Reading" took a drop of around .3 percentage points by removing the 9th grade data from Thomas High School - which was the largest change among any of the data sections in this summary. At the same time, the "Average Reading Score" section did not change at all after removing the 9th grade data from Thomas High School, which means the reading score data that was dropped was close to the average among the other schools in the district which boosted the number of students with a passing grade.
