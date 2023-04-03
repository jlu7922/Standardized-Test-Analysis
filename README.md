# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis

### Problem Statement

Between the SAT and ACT, many students have a preference of one exam to the other, to play to their academic strengths. Traditionally, the ACT has been recommended to students who have a stronger math/science background, while the SAT has been more suited for individuals with stronger reading comprehension and writing skills. We wish to see if there is a difference in performance between the two exams for certain areas of aptitude.


---

### Datasets

* [`act_2019.csv`](./data/act_2019.csv): 2019 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`sat_2019.csv`](./data/sat_2019.csv): 2019 SAT Scores by State ([source](https://blog.prepscholar.com/average-sat-scores-by-state-most-recent))
* [`sat_2019_by_intended_college_major.csv`](./data/sat_2019_by_intended_college_major.csv): 2019 SAT Scores by Intended College Major ([source](https://web.archive.org/web/20220426162357/https://reports.collegeboard.org/pdf/2019-total-group-sat-suite-assessments-annual-report.pdf))


#### Additional Data

* [`act_2020_by_intended_college_major.csv`](./data/act_2020_by_intended_college_major.csv): 2020 ACT Scores by Intended College Major ([source](https://www.act.org/content/dam/act/unsecured/documents/2020/2020-National-ACT-Profile-Report.pdf))

Taken from *Table 4.1. Distribution of Planned Educational Majors for All Students by College Plans

---

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|<center>sat_2019/act_2019</center>|The name of the state for each data point| 
|participation|float|<center>sat_2019/act_2019<center>|The participation rate of students per given state| 
|Avg SAT Score|float|<center>*All Datasets*<center>|The average SAT score per state or intended major| 
|Avg ACT Score|float|<center>*All Datasets*<center>|The average ACT score per state or intended major|
|Avg ACT Score Scaled|float|<center>act_2020_by_intended_college<center>|The average ACT score per state or intended major scaled to match the SAT scoring system|
|Intended Major|object|sat_2019_by_intended_college/act_2020_by_intended_college|Selection of preferred major by student taking exam|

---

    
### Conclusion

The data highlights that students with a strong foundation in the STEM field do better on the ACT than the SAT. Conversely, students with a background and aptitude for humanities do better on the SAT. However, there are a few groups that score equally high on both exams, which may suggest that the difference between the exams is not a major contribution to benefitting certain aptitudes.

Additionally, the average score of tests correlate negatively with the popularity of the test within certain states. This is understood as that students who choose the less popular test within a state have a preference for it, whether it be for aptitude or otherwise. These students are likely to score better because they are likely more informed about the exam, having deliberately chosen it to suit their skills.
    
Further analysis of different data over multiple years is required, especially data revolving around individual preferences rather than assumed aptitudes. 
