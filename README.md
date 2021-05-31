# School District Analysis with Pandas
Click here to view the Pandas file: [School District Analysis Program](https://github.com/sqrtofpi/School_District_Analysis/blob/78cf76d409f16a7ab2d65f3b8856b4917b1428d6/PyCitySchools_Challenge.ipynb)

## Project Overview

Having successfully submitted an analysis of school district performance and upon review of the analysis; the school board has notified Maria (and her supervisor), the students_complete.csv file shows evidence of "academic dishonesty". Specifically at issue are the reading and math grades for Thomas High School 9th grade class. The full extent of the "academic dishonesty" is unknown, but the remaining data is presumed accurate and will be utilized in the subsequent analysis excluding the Thomas High School 9th grade class information. To assure the original data remains intact for auditing purposes, Maria has enlisted the services of Scott MacDonald to programmatically analyze the original dataset with Pandas to assure the data in the students_complete.csv is not altered and a proper analysis can be performed. This analysis consists of two technical analysis deliverables, namely:

1. Replacing the Thomas High School 9th grade reading and math scores with "NaN" (Not a Number) values to be excluded for purposes of the new analysis
2. Repeating the School District Analysis with the following recreated metrics:
   - The district summary
   - The school summary
   - The top 5 and bottom 5 performing schools, based on the passing rate
   - The average math score for each grade level from each school
   - The average reading score for each grade level from each school
   - The scores by school spending per student, by school size, and school type

## Resources

- Data Sources: schools_complete.csv & students_complete.csv
- Software: Python version 3.8.5, Conda version 4.10.1

## Results

Upon removing the suspect reading and math data from Thomas High School's 9th grade class, the following results have been determined for the metrics of interest:

### The district summary affect

- Avg. math score decreased
- Avg. reading score increased
- Overall Passing decreased

![District Summary Original](https://github.com/sqrtofpi/School_District_Analysis/blob/2bf273cf566d2faa24ae52eed91ae7c19129cac9/Resources/District%20Summary%20Original.png)

![District Summary Updated](https://github.com/sqrtofpi/School_District_Analysis/blob/2bf273cf566d2faa24ae52eed91ae7c19129cac9/Resources/District%20Summary%20Updated.png)

### The school summary affect

- Over all the schools the impact was relatively minor to exclude the 9th grade data from Thomas High School, this is primarily because the number of 9th graders at that school compared with the entire dataset was small.

- The affect to Thomas High School's results were significant however. The % Overall passing went from 65.1% to 90.6% when the 9th graders information was excluded.

![Summary with Thomas High School 9th Grade](https://github.com/sqrtofpi/School_District_Analysis/blob/2bf273cf566d2faa24ae52eed91ae7c19129cac9/Resources/School%20Summary%20with%20Thomas%20HS%209th%20Grade.png)

![Summary without Thomas High School 9th Grade](https://github.com/sqrtofpi/School_District_Analysis/blob/2bf273cf566d2faa24ae52eed91ae7c19129cac9/Resources/School%20Summary%20without%20Thomas%20HS%209th%20Grade.png)

### Thomas High School performance compared to other Schools

-  Thomas went from 9th best to 2nd best relative to the overall performance of other schools in the district when the 9th grade students information was excluded from the results.

![Top 5 Performing Schools without Thomas High School 9th Grade Data](https://github.com/sqrtofpi/School_District_Analysis/blob/2bf273cf566d2faa24ae52eed91ae7c19129cac9/Resources/Top%205%20Performing%20Schools.png)

### Additional affects of removing the Thomas High School 9th grade data

- **Math and reading scores by grade:** Given the THS 9th grade data was significantly lower than the rest of the data set, removing the data will increase the Avg. of all the 9th grade results.
- **Scores by school spending:** There is no affect on school spending results from removing the 9th grade math and reading data from THS's results.
- **Scores by school size:** Thomas High School has a medium size population with relation to the other schools in the analysis. Removing the 9th grade results from THS will have little affect on the overall results of the analysis but will have a slightly bigger affect on Thomas High School's results since nearly 1/4 of the data was removed.
- **Scores by school type:** Removing Thomas High School's results for 9th grade math and reading will have a minor affect on the overall scores by school type for charter schools and no affect on the district school results as THS is a charter school.

## Summary

Four changes that have occurred since updating the school district analysis after excluding Thomas High School's 9th grade math and reading data:

1. The total number of results for 9th grade reading and math have decreased;
2. The percentages in various categories mentioned earlier in this analysis, were affected as a result of decreased data;
3. Thomas High School has an incomplete data record that will need to be accounted for to oversight review boards;
4. Thomas High School's performance based upon % Passing Overall increased it's position relative to the other schools.
