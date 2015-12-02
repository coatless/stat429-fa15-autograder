Autograder Leaderboard for STAT 429 in Fall 2015
================================================

Problem 2
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 12      |  0.1944| 15138444b9c40212 |                      3|
|         2| 2       |  0.2113| 151609e745c5509f |                      6|
|         3| 11      |  0.2197| 151545605ad01306 |                      6|
|         4| 10      |  0.2318| 15160957c935093d |                     20|
|         5| 1       |  0.2418| 151565f47f878195 |                     39|
|         6| 5       |  0.2424| 151604572f194c92 |                     13|
|         7| 6       |  0.2436| 1515b45c86df876a |                     11|
|         8| 4       |  0.2522| 1516095a0d7f5ca1 |                     13|
|         9| 7       |  0.2592| 1515fac83085605b |                      9|
|        10| 3       |  0.2671| 1515c3f16bc13156 |                     14|
|        11| 8       |  0.2691| 1515ef4974ebaf58 |                      4|
|        12| 9       |  3.2716| 151508cb3ca868ff |                      6|

Problem 3
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 11      |  0.0078| 151610c99ac345ca |                     15|
|         2| 5       |  0.0086| 151601762e0604c0 |                     11|
|         3| 7       |  0.0093| 1516036e7a1c3fc9 |                      9|
|         4| 12      |  0.0098| 15161d983a3bee10 |                     18|
|         5| 4       |  0.0098| 1515b8e0a858fd6c |                     21|
|         6| 3       |  0.0101| 1515bc76a3d77f75 |                      8|
|         7| 6       |  0.0101| 15160c47404f35f0 |                     15|
|         8| 1       |  0.0145| 1515659b50bf3f0c |                      4|
|         9| 10      |  0.0146| 151574e9bfe6f212 |                     13|
|        10| 8       |  0.0167| 1513781f7e0d6768 |                      5|
|        11| 9       |  0.0177| 1515fcd27fc61e96 |                      2|
|        12| 2       |  1.9291| 15141e80e68af1d9 |                      6|

Problem 4
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 6       |  0.2968| 1516186a4efaa5a4 |                     27|
|         2| 12      |  0.3004| 1515effcca10d08f |                     41|
|         3| 4       |  0.3122| 1515ab73caaa8519 |                      8|
|         4| 7       |  0.3271| 15160100da530edd |                     21|
|         5| 11      |  0.3317| 15159ba3f7bcb49f |                     15|
|         6| 8       |  0.3342| 1516113a4488e03e |                      7|
|         7| 1       |  0.3361| 151611b09d34fd9d |                      5|
|         8| 10      |  0.3451| 1516096a9d3bd4b0 |                      6|
|         9| 5       |  0.3467| 1516112adde56fb1 |                     10|
|        10| 3       |  0.3798| 1515aca51e743585 |                      6|
|        11| 2       |  0.9939| 15161097a2d0f595 |                      3|
|        12| 9       |     Inf| 1516218ccc8b5311 |                      5|

Autograder Submission Statistics
================================

Below are submission statistics regarding the current state the Autograder is in.

Overall Submissions
-------------------

| Team ID |  Total Submissions|
|:--------|------------------:|
| 1       |                 48|
| 10      |                 39|
| 11      |                 36|
| 12      |                 62|
| 2       |                 15|
| 3       |                 28|
| 4       |                 42|
| 5       |                 34|
| 6       |                 53|
| 7       |                 39|
| 8       |                 16|
| 9       |                 13|

Submissions by problem
----------------------

| Problem ID |  Total Submissions|
|:-----------|------------------:|
| 2          |                144|
| 3          |                127|
| 4          |                154|

Problem State Status
--------------------

| Assignment Code |  Total|
|:----------------|------:|
| ERROR           |     86|
| RAN             |    268|
| STORE           |     41|
| TIMEOUT         |     30|

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
