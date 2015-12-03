Autograder Leaderboard for STAT 429 in Fall 2015
================================================

Problem 2
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 1       |  0.1882| 1516520310a8179d |                     47|
|         2| 12      |  0.1944| 15138444b9c40212 |                      3|
|         3| 2       |  0.2113| 151609e745c5509f |                      6|
|         4| 4       |  0.2130| 151654139af4f930 |                     15|
|         5| 11      |  0.2197| 151545605ad01306 |                      6|
|         6| 10      |  0.2316| 1516274e1bcecbe3 |                     23|
|         7| 8       |  0.2370| 15163b5d36202dc6 |                      6|
|         8| 5       |  0.2424| 15163c20867d24d6 |                     14|
|         9| 6       |  0.2436| 1515b45c86df876a |                     12|
|        10| 9       |  0.2470| 151645965b914840 |                     15|
|        11| 7       |  0.2517| 151652c9c1dfd536 |                     16|
|        12| 3       |  0.2671| 1515c3f16bc13156 |                     17|

Problem 3
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 1       |  0.0073| 151651ebf5b99372 |                      6|
|         2| 6       |  0.0074| 151647155d43e02b |                     19|
|         3| 11      |  0.0078| 151610c99ac345ca |                     15|
|         4| 5       |  0.0086| 151601762e0604c0 |                     11|
|         5| 7       |  0.0093| 1516036e7a1c3fc9 |                     10|
|         6| 10      |  0.0096| 151652aff2e26bd5 |                     21|
|         7| 12      |  0.0097| 15164c2618d539ef |                     21|
|         8| 4       |  0.0098| 1515b8e0a858fd6c |                     26|
|         9| 3       |  0.0101| 1515bc76a3d77f75 |                      8|
|        10| 8       |  0.0167| 1513781f7e0d6768 |                      6|
|        11| 9       |  0.0177| 1515fcd27fc61e96 |                      3|
|        12| 2       |  1.9291| 15141e80e68af1d9 |                      8|

Problem 4
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 4       |  0.2962| 151643f9ab4b9131 |                      9|
|         2| 6       |  0.2968| 151649b3c8cbf3db |                     31|
|         3| 12      |  0.3004| 1515effcca10d08f |                     44|
|         4| 11      |  0.3264| 1516513a56ca64ad |                     20|
|         5| 7       |  0.3271| 15160100da530edd |                     21|
|         6| 1       |  0.3307| 15164a54c5069cba |                      6|
|         7| 8       |  0.3333| 151654869bb550b7 |                      8|
|         8| 10      |  0.3451| 1516096a9d3bd4b0 |                      8|
|         9| 5       |  0.3467| 1516112adde56fb1 |                     12|
|        10| 3       |  0.3798| 1515aca51e743585 |                      6|
|        11| 2       |  0.9434| 15164322107f054c |                      4|
|        12| 9       |  1.0000| 1516514560b4c741 |                      8|

Autograder Submission Statistics
================================

Below are submission statistics regarding the current state the Autograder is in.

Overall Submissions
-------------------

| Team ID |  Total Submissions|
|:--------|------------------:|
| 1       |                 59|
| 10      |                 52|
| 11      |                 41|
| 12      |                 68|
| 2       |                 18|
| 3       |                 31|
| 4       |                 50|
| 5       |                 37|
| 6       |                 62|
| 7       |                 47|
| 8       |                 20|
| 9       |                 26|

Submissions by problem
----------------------

| Problem ID |  Total Submissions|
|:-----------|------------------:|
| 2          |                180|
| 3          |                154|
| 4          |                177|

Problem State Status
--------------------

| Assignment Code |  Total|
|:----------------|------:|
| ERROR           |    106|
| RAN             |    325|
| STORE           |     45|
| TIMEOUT         |     35|

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
