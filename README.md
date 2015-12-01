Autograder Leaderboard for STAT 429 in Fall 2015
================================================

Problem 2
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 12      |  0.1944| 15138444b9c40212 |                      3|
|         2| 11      |  0.2197| 151545605ad01306 |                      5|
|         3| 10      |  0.2322| 1515aa8631d56b34 |                     17|
|         4| 1       |  0.2418| 151565f47f878195 |                     32|
|         5| 6       |  0.2436| 1515b45c86df876a |                      8|
|         6| 4       |  0.2578| 151596cefc0bd603 |                      8|
|         7| 5       |  0.2607| 1515bcec4b77996c |                      9|
|         8| 3       |  0.2671| 1515c3f16bc13156 |                     11|
|         9| 2       |  0.2701| 1515b60921cc415f |                      4|
|        10| 8       |  0.2724| 1515c0873ee809cd |                      3|
|        11| 9       |  3.2716| 151508cb3ca868ff |                      3|
|        12| 7       |     Inf| 1515a7aa0839b9b8 |                      1|

Problem 3
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 11      |  0.0080| 15153abd492bf71b |                     13|
|         2| 4       |  0.0098| 1515b8e0a858fd6c |                     16|
|         3| 12      |  0.0099| 1515909dd7bc322f |                      8|
|         4| 3       |  0.0101| 1515bc76a3d77f75 |                      6|
|         5| 5       |  0.0134| 1514afccc0177813 |                     10|
|         6| 1       |  0.0145| 1515659b50bf3f0c |                      4|
|         7| 10      |  0.0146| 151574e9bfe6f212 |                     13|
|         8| 6       |  0.0162| 1513babfceec3ac2 |                      9|
|         9| 8       |  0.0167| 1513781f7e0d6768 |                      3|
|        10| 7       |  0.0530| 1515c05a0e3a6fe5 |                      5|
|        11| 9       |  0.1570| 1515afe061505314 |                      1|
|        12| 2       |  1.9291| 15141e80e68af1d9 |                      6|

Problem 4
---------

|  Position| Team ID |    MAPE| Submission ID    |  Number of Submissions|
|---------:|:--------|-------:|:-----------------|----------------------:|
|         1| 12      |  0.3117| 1515caa40ad9903e |                     34|
|         2| 4       |  0.3122| 1515ab73caaa8519 |                      6|
|         3| 11      |  0.3317| 15159ba3f7bcb49f |                     15|
|         4| 10      |  0.3451| 1515aa8d2163101e |                      3|
|         5| 1       |  0.3585| 1515697e0faeaff8 |                      3|
|         6| 8       |  0.3610| 1515b33a4ef6966c |                      5|
|         7| 7       |  0.3671| 1515e8bd8c26753a |                     13|
|         8| 6       |  0.3697| 15155607f21055cc |                     10|
|         9| 5       |  0.3746| 151415169d4b5f53 |                      6|
|        10| 3       |  0.3798| 1515aca51e743585 |                      6|
|        11| 9       |     Inf| 1515b098b9e8751c |                      2|

Autograder Submission Statistics
================================

Below are submission statistics regarding the current state the Autograder is in.

Overall Submissions
-------------------

| Team ID |  Total Submissions|
|:--------|------------------:|
| 1       |                 39|
| 10      |                 33|
| 11      |                 33|
| 12      |                 45|
| 2       |                 10|
| 3       |                 23|
| 4       |                 30|
| 5       |                 25|
| 6       |                 27|
| 7       |                 19|
| 8       |                 11|
| 9       |                  6|

Submissions by problem
----------------------

| Problem ID |  Total Submissions|
|:-----------|------------------:|
| 2          |                104|
| 3          |                 94|
| 4          |                103|

Problem State Status
--------------------

| Assignment Code |  Total|
|:----------------|------:|
| ERROR           |     68|
| RAN             |    186|
| STORE           |     24|
| TIMEOUT         |     23|

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
