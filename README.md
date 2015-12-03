Autograder Leaderboard for STAT 429 in Fall 2015
================================================

Problem 2
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 6       |  0.0812| 15169edd00594987 |                     32|
|         2| 12      |  0.0948| 15169f16cfad8d35 |                     32|
|         3| 1       |  0.1882| 15168a2904506adb |                     52|
|         4| 2       |  0.2113| 15168888ffdd1f5d |                     12|
|         5| 4       |  0.2130| 151654139af4f930 |                     15|
|         6| 11      |  0.2197| 151545605ad01306 |                      6|
|         7| 9       |  0.2281| 15167d06aee72353 |                     34|
|         8| 10      |  0.2316| 1516274e1bcecbe3 |                     28|
|         9| 8       |  0.2370| 15163b5d36202dc6 |                      8|
|        10| 5       |  0.2424| 15163c20867d24d6 |                     14|
|        11| 7       |  0.2517| 15165e6caeed4987 |                     20|
|        12| 3       |  0.2664| 151659e5c4d73f1d |                     18|

Problem 3
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 1       |  0.0073| 151651ebf5b99372 |                      6|
|         2| 6       |  0.0074| 151647155d43e02b |                     23|
|         3| 2       |  0.0075| 15168528c4c15ec2 |                     13|
|         4| 11      |  0.0078| 151610c99ac345ca |                     16|
|         5| 5       |  0.0086| 151601762e0604c0 |                     12|
|         6| 7       |  0.0093| 15166160f7ba0ffc |                     15|
|         7| 10      |  0.0096| 15169c5d1d90ccae |                     26|
|         8| 12      |  0.0097| 15165e832caaa1d3 |                     25|
|         9| 4       |  0.0098| 1516a0b07b2d1054 |                     34|
|        10| 3       |  0.0101| 1515bc76a3d77f75 |                      8|
|        11| 8       |  0.0167| 1513781f7e0d6768 |                      9|
|        12| 9       |  0.0170| 15165b9092a388b4 |                      5|

Problem 4
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 12      |  0.2723| 1516891e2b6873a5 |                     71|
|         2| 4       |  0.2962| 151643f9ab4b9131 |                      9|
|         3| 6       |  0.2963| 15166bc3438a6ff2 |                     55|
|         4| 7       |  0.3148| 1516968193eb5f2a |                     28|
|         5| 1       |  0.3174| 15169e7b3a2c8915 |                     12|
|         6| 9       |  0.3220| 151674e72505509d |                     26|
|         7| 8       |  0.3256| 151658aaf79ae880 |                      9|
|         8| 11      |  0.3264| 15165a42c8e91df0 |                     22|
|         9| 10      |  0.3451| 1516096a9d3bd4b0 |                     14|
|        10| 5       |  0.3467| 1516112adde56fb1 |                     12|
|        11| 2       |  0.3588| 151698d5c6aba8c0 |                     15|
|        12| 3       |  0.3798| 1515aca51e743585 |                      6|

Autograder Submission Statistics
================================

Below are submission statistics regarding the current state the Autograder is in.

Overall Submissions
-------------------

| Team ID |  Total Submissions|
|:--------|------------------:|
| 1       |                 70|
| 10      |                 68|
| 11      |                 44|
| 12      |                128|
| 2       |                 40|
| 3       |                 32|
| 4       |                 58|
| 5       |                 38|
| 6       |                111|
| 7       |                 63|
| 8       |                 26|
| 9       |                 65|

Submissions by problem
----------------------

| Problem ID |  Total Submissions|
|:-----------|------------------:|
| 2          |                271|
| 22         |                  1|
| 3          |                192|
| 4          |                279|

Problem State Status
--------------------

| Assignment Code |  Total|
|:----------------|------:|
| ERROR           |    132|
| RAN             |    514|
| STORE           |     58|
| TIMEOUT         |     39|

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
