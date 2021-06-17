# Standardized Test Analysis

### Problem Statement

As a private tuition center with a mission of providing SAT and ACT immersive programs to help and support more students to achieve a better score so that they can enter their desired college, the aim of this project is to identify the trends and find out which states to choose to set up the SAT/ACT immersive programs to help students to improve their score.

---
### Background

ACT and SAT standardized tests are tests which students have to undergo for college admissions. The idea behind these tests is to examine the student's readiness for college and these tests are required by a majority of the colleges admissions. As the grade-point average (GPA) is tabulated differently between schools, school district, country and state, ACT and SAT has been used as a standardized test for college readiness. [[source]](https://www.usnews.com/education/best-colleges/articles/2018-11-30/what-students-should-know-about-the-gpa-scale). 

Both ACT and SAT tests are generally accepted by most states although they differ in structure.[[source]](https://magoosh.com/hs/act/act-scores/) [[source]](https://blog.prepscholar.com/what-is-a-good-sat-score-a-bad-sat-score-an-excellent-sat-score) Interestingly, there are state policy that mandates the adoptation of a certain test, which affects both the participation rate and states average scores. [[source]](https://medium.com/@james.dargan/self-selection-drives-state-averages-8e5b53be0c17) [[source]](https://www.edweek.org/teaching-learning/sat-scores-rise-as-number-of-test-takers-tops-2-million/2018/10) [[source]](https://blog.prepscholar.com/which-states-require-the-act-full-list-and-advice) [[source]](https://blog.prepscholar.com/which-states-require-the-sat).As SAT has recently change its format since 2016, we will be looking into the data from 2017 to 2019.[[source]](https://collegereadiness.collegeboard.org/sat/inside-the-test/compare-old-new-specifications!). The data source are obtained as followed. [[source]](https://research.collegeboard.org/programs/sat/data/2020-sat-suite-annual-report) [[source]](https://www.act.org/content/act/en/search.html#stq=report) For the analysis of these tests, the scores are compared with the national scores with their respective years (ACT 2017 & 2018 [[source]](https://nces.ed.gov/fastfacts/display.asp?id=897), 2019) [[source]](https://nces.ed.gov/programs/digest/d19/tables/dt19_226.60.asp?current=yes)) (SAT 2017,2018 & 2019 [[source]](https://nces.ed.gov/programs/digest/d19/tables/dt19_226.30.asp))

---
### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|ACT/SAT|State in United States| 
|act_participation_2017 |float|ACT|Participation rate of high school graduates taking ACT test in the particular state in 2017| 
|act_english_2017 |float|ACT|State mean score for ACT english in 2017| 
|act_math_2017 |float|ACT|State mean score for ACT math in 2017| 
|act_reading_2017 |float|ACT|State mean score for ACT reading in 2017|
|act_science_2017 |float|ACT|State mean score for ACT science in 2017|
|act_composite_2017 |float|ACT|State mean composite score for ACT in 2017|
|act_participation_2018 |float|ACT|Participation rate of high school graduates taking ACT test in the particular state in 2018| 
|act_composite_2018 |float|ACT|State mean composite score for ACT in 2018|
|act_participation_2019 |float|ACT|Participation rate of high school graduates taking ACT test in the particular state in 2019| 
|act_composite_2019 |float|ACT|State mean composite score for ACT in 2019|
|sat_participation_2017 |float|SAT|Participation rate of high school graduates taking SAT test in the particular state in 2017| 
|sat_ebrw_2017 |float|SAT|State mean score for SAT Evidence-Based Reading and Writing test in 2017| 
|sat_math_2017 |float|SAT|State mean score for SAT math test in 2017| 
|sat_total_2017 |float|SAT|State mean total score for SAT in 2017| 
|sat_participation_2018 |float|SAT|Participation rate of high school graduates taking SAT test in the particular state in 2018| 
|sat_ebrw_2018 |float|SAT|State mean score for SAT Evidence-Based Reading and Writing test in 2018| 
|sat_math_2018 |float|SAT|State mean score for SAT math test in 2018| 
|sat_total_2018 |float|SAT|State mean total score for SAT in 2018| 
|sat_participation_2019 |float|SAT|Participation rate of high school graduates taking SAT test in the particular state in 2019| 
|sat_ebrw_2019 |integer|SAT|State mean score for SAT Evidence-Based Reading and Writing test in 2019| 
|sat_math_2019 |integer|SAT|State mean score for SAT math test in 2019| 
|sat_total_2019 |integer|SAT|State mean total score for SAT in 2019| 


---
### Brief summary of your analysis

The findings of the analysis are as followed:-
1. Approximately one third of the states in USA have 100% participation rate in ACT tests from 2017 to 2019.
2. Approximately one third of the states in USA have less than 10% participation rate in SAT tests from 2017 to 2019.
3. The relationship between ACT and SAT participation rate is negatively correlated. This is observed when a high participation rate in one test, results in a low participation rate in the other tests.
4. There is a significant proportion of states adopting and implementing a mandatory tests resulting in both ACT and SAT tests having both very high and very low participation rates.
5. Almost all of the states in USA have an average composite score more than 50% of the ACT composite scores.
6. High proportion of the states in USA having an average of more than 58.9% SAT total scores
7. There is a negatively correlation between high ACT composite score with low ACT participation rate and high SAT participation rate. 
8. There is a negatively correlation between low ACT composite score with high ACT participation rate and low SAT participation rate.

With the findings that illustrates the non-symmetrical distribution of participation rate and test scores due to the mandatory implementation by the states, we identify a total of 5 states that have more than 50% participation rate across the 2017 to 2019 in both ACT and SAT tests.The states include Florida, Hawaii, North Carolina, South Carolina and Georgia.

**These 5 states serves as a potential state to set up the SAT and ACT immersive program due to the high participation rate in both tests**

---

### Conclusions

In USA, ACT and SAT tests are used as a standardized tests for college admissions with the idea behind to measure the college readiness of the students. Many states have adopted and implemented one of the tests mandatory in their states, which results in a non-symmetrical distribution of the participation rates in both ACT and SAT tests. As a significant proportion of the states prefer or mandates one of the tests, the other test might have a low participation rate in that same state. This holds true with our findings that the states that have strong full participation across the three years have an observation of low SAT participation rate with less than 10% in the same state. Interestingly, the states that have low participation rate in the other test have a high average scores for the other test. However, the states score a low average scores for the test that they have high participation rate in. As a result, there is a non-symmetrical distribution of participation rate and test scores for each test across the states in USA.


---

### Recommendations

As SAT and ACT tests are one of the determined criteria for the college admission, it is critical for the students to score a high score for these tests. As a private tuition center that aims to provide SAT and ACT immersive programs to help and support the students to achieve a better score in these tests, we aim to identify the states to set up this programs. Due to the resource constraint, the private tuition centre plans to set up centers in states which can help students in both ACT and SAT tests. 

With the findings that illustrates the non-symmetrical distribution of participation rate and test scores due to the mandatory implementation by the states, we aim to identify the states that have more than 50% participation rate in both ACT and SAT tests. From the data analysis, there are 4 states that meet this criteria, which is Florida, Georgia, North Carolina and South Carolina. Although Hawaii meet this criteria, however due to the population size and geographic location, it will be ideal to set up the program in the mainland.

These four states are ideal as there are a significant proportion of students around a minimum of 30 000 test-takers, the states have a policy for taking either SAT or ACT tests except for North Carolina, which mandates an ACT test in their states. However, North Carolina can also be a choice due to its high participation rate (more than 50%) in both tests in 2018 and 2019. In addition, both ACT composite score and SAT total score lies about 25th to 50th percentile of the states scores, which further supports the need of SAT and ACT immersive programs to support the students to achieve a better grades in these tests. Thus, the state recommendation for the private tuition center to set up this program is Florida, Georgia, North Carolina and South Carolina.

---

