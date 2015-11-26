Autograder Leaderboard for STAT 429 in Fall 2015
================================================

Problem 2
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 12      |  0.1944| 15138444b9c40212 |                      3|
|         2| 6       |  0.2607| 1513fc24f584760a |                      4|
|         3| 4       |  0.2627| 1513b8967db2e1da |                      2|
|         4| 10      |  0.2644| 1513de715f7055f7 |                      2|
|         5| 1       |  0.2860| 151423488cd1f795 |                      8|
|         6| 3       |     Inf| 1513f914b249c93c |                      3|

Problem 3
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 4       |  0.0118| 1513cb744367631d |                      5|
|         2| 1       |  0.0153| 1514217d34a3e900 |                      3|
|         3| 6       |  0.0162| 1513babfceec3ac2 |                      5|
|         4| 8       |  0.0167| 1513781f7e0d6768 |                      1|
|         5| 11      |  0.0168| 1513ba0acf0cea95 |                      2|
|         6| 5       |  0.0173| 1513cd5540ca1307 |                      2|
|         7| 10      |  0.0209| 151410441542ea3a |                      3|
|         8| 7       |  0.0531| 151425d9f4eba870 |                      2|
|         9| 2       |  1.9291| 15141e80e68af1d9 |                      1|
|        10| 12      |     Inf| 15140d6e2cf96957 |                      1|
|        11| 3       |     Inf| 1513cc7553ca73a4 |                      2|

Problem 4
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 12      |  0.3188| 15142b12dc321b84 |                      9|
|         2| 11      |  0.3390| 1513fc20217d92ba |                      2|
|         3| 4       |  0.3546| 1513b89e3c55ca2e |                      3|
|         4| 6       |  0.3697| 1513b8750f6b0178 |                      4|
|         5| 5       |  0.3746| 151415169d4b5f53 |                      3|
|         6| 3       |  0.3889| 1513bf398bc58870 |                      3|
|         7| 7       |  0.4970| 1513f7e220000e06 |                      2|

Autograder Submission Statistics
================================

Below are submission statistics regarding the current state the Autograder is in.

Overall Submissions
-------------------

| Team ID |  Total Submissions|
|:--------|------------------:|
| 1       |                 11|
| 10      |                  5|
| 11      |                  4|
| 12      |                 13|
| 2       |                  1|
| 3       |                  8|
| 4       |                 10|
| 5       |                  5|
| 6       |                 13|
| 7       |                  4|
| 8       |                  1|

Submissions by problem
----------------------

| Problem ID |  Total Submissions|
|:-----------|------------------:|
| 2          |                 22|
| 3          |                 27|
| 4          |                 26|

Problem State Status
--------------------

| Assignment Code |  Total|
|:----------------|------:|
| ERROR           |     21|
| RAN             |     40|
| STORE           |     10|
| TIMEOUT         |      4|

-   **STORE**: If multiple submissions for a given problem occur within the collection window, the autograder evalutes the newest and sends the oldest to storage.
-   **RUN**: The code is in the Autograder's grading queue.
-   **ERROR**: The Autograder encountered an error when attempting to run the code.
-   **RAN**: The code has been evaluated and the results have been sent.
-   **TIMEOUT**: The runtime of the code has exceeded the allotted amount of processing time given to each submission.

Details of the Autograder
=========================

The results obtained above were generated by a script written to autograde R code written by James Joseph Balamuta (balamut2 [at] illinois [dot] edu). The script was deployed in Prof. Stephane Guerrier's STAT 429 Time Series Analysis course in Fall 2015 at the University of Illinois at Urbana-Champaign (UIUC). The hope is to increase the adoption of this script across all modeling or programming method courses within the Statistics department at UIUC.

The script takes in a team's code submission to create a model and then evaluates the model's effectiveness using a 1-step forward prediction aided by a hidden testing data set. The teams are then assessed based on their MAPE Score. The lower the MAPE score, the better the team's score.

[MAPE](https://en.wikipedia.org/wiki/Mean_absolute_percentage_error) is defined to be:

``` r
mean(abs((Y - Y_hat)/Y))
```

After the competition is over, a post will detail the intricacies of the system and provide guidance on how to replicate it.
