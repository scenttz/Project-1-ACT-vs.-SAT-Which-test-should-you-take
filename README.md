# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: ACT vs. SAT: Which test should you take?


### Problem Statement

Whether a student should concentrate on the ACT or the SAT is one of the frequently asked questions an experienced ACT and SAT has encountered. Although colleges claim to treat both tests equally, is that really the case?


### Background

The SAT and ACT are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university.

They have different score ranges, which you can read more about on their websites or additional outside sources.
* [SAT](https://collegereadiness.collegeboard.org/sat) has two sections of the test: Evidence-Based Reading and Writing and Math ([*source*](https://www.princetonreview.com/college/sat-sections)).
* [ACT](https://www.act.org/content/act/en.html) has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section([*source*](https://www.act.org/content/act/en/products-and-services/the-act/scores/understanding-your-scores.html)).

Standardized tests have long been a controversial topic for students, administrators, and legislators. Since the 1940's, an increasing number of colleges have been using scores from students' performances on tests like the SAT and the ACT as a measure for college readiness and aptitude ([*source*](https://www.minotdailynews.com/news/local-news/2017/04/a-brief-history-of-the-sat-and-act/)). Supporters of these tests argue that these scores can be used as an objective measure to determine college admittance. Opponents of these tests claim that these tests are not accurate measures of students potential or ability and serve as an inequitable barrier to entry. Lately, more and more schools are opting to drop the SAT/ACT requirement for their Fall 2021 applications ([*read more about this here*](https://www.cnn.com/2020/04/14/us/coronavirus-colleges-sat-act-test-trnd/index.html)).

---

### Datasets

* [`act_2019.csv`](../data/act_2019.csv): 2019 ACT Scores by State
* [`sat_2019.csv`](../data/sat_2019.csv): 2019 SAT Scores by State
* [`SAT_to_ACT_Conversion_Chart.csv`](../data/SAT_to_ACT_Conversion_Chart.csv): SAT to ACT Conversion Chart
* [`sat_act_by_college.csv`](../data/sat_act_by_college.csv): Ranges of Accepted ACT & SAT Student Scores by Colleges
* [`cwuData.csv`](../data/cwuData.csv): World University Rankings

---

### Additional Data

* https://www.kaggle.com/datasets/mylesoneill/world-university-rankings : World University Rankings
* https://www.studypoint.com/ed/sat-act-concordance/ : SAT to ACT Conversion Chart: Convert Your SAT Scores to ACT Scores
* https://www.collegefinancinggroup.com/choosing-a-college/act-vs-sat-test-right/ : ACT vs. SAT: Which test should you take?
* https://www.goodschoolsguide.co.uk/university/usa/the-sat-and-act-and-tips-for-taking-them : The SAT and ACT - and tips for taking them
---

#### Data Dictionary for SAT and ACT score by State, 2019

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state_us |object|act_2019 and sat_2019 from prepscholar.com|The name of the State of US |
|sat_parti_rate |float|sat_2019 from prepscholar.com|The SAT participation rate for eligible students in each State of US|
|sat_total|int|sat_2019 from prepscholar.com|The average SAT total score (EBRW + Math) in each State of US|
|act_parti_rate|float|act_2019 from prepscholar.com|The ACT participation rate for eligible students in each State of US||
|act_total|float|act_2019 from prepscholar.com|The average ACT composite in each State of US|
|act_score_form_sat|int|ACT/SAT Concordance Tables|The equivalent ACT composite score for each State of US average SAT score|

#### Data Dictionary for SAT/ACT Scores by College


|Feature|Type|Dataset|Description|
|---|---|---|---|
|university|object|sat_act_by_college from Compass Prep|University name in US|
|test_optional|object|sat_act_by_college from Compass Prep|Describes whether or not the college is test optional|
|policy_details|object|sat_act_by_college from Compass Prep|Detailed test-optional of each university|
|number_of_applicants|int|sat_act_by_college from Compass Prep|The number of applicants to the college|
|accept_rate|float|sat_act_by_college from Compass Prep|The rate of acceptance for applicants|
|sat_25_percentile|float|sat_act_by_college from Compass Prep|The 25th percentile SAT total score (EBRW + Math) for accepted students|
|sat_75_percentile|float|sat_act_by_college from Compass Prep|The 75th percentile SAT total score (EBRW + Math) for accepted students|
|act_25_percentile|float|sat_act_by_college from Compass Prep| The 25th percentile ACT composite for accepted students|
|act_75_percentile|float|sat_act_by_college from Compass Prep| The 75th percentile ACT composite for accepted students|
|world_rank|float|World University Rankings from Kaggle|World University Rankings of university in US|

### Conclusions and Recommendations

According to the mentioned insights, it can be concluded that ACT score was more popular among students for their entrance exam than SAT score corresponding to the participation rate. Moreover, the distribution of ACT score tends to be compact while SAT score tends to have an outstanding score.

Then, the test scores were investigated in different universities including top 15 universities and other universities. The world top 15 universities appeared to require high score of ACT test comparing to SAT test. Therefore, if the students have a short preparation time, it is better to choose SAT test due to their lower score. However, ACT score was more effective for entering top 100 universities when focusing on accept rate more than 90%. In contrast, SAT score did not have any impacts on top 100 universities entrance.

Therefore, ACT score should be more focus when student's target was top rank universities. But if the rank of universities was not concerned, the students can choose SAT score for their entrance exam.
