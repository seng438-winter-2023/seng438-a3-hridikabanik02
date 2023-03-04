**SENG 438 - Software Testing, Reliability, and Quality**

**Lab. Report #3 – Code Coverage, Adequacy Criteria and Test Case Correlation**

| Group \#:      |  16   |
| -------------- | --- |
| Student Names: |     |
|        Hridika Banik        |     |
|           Radia Jannat     |     |
|        MD Shaherier Khan        |     |
|        Syed Mohammed Abbas Kazmi        |     |

(Note that some labs require individual reports while others require one report
for each group. Please see each lab document for details.)

# 1 Introduction

In this assignment we were asked to asked to implement white-box testing for the Range and Datautilities class. We measured various coverage metrics like Statement coverage , branch coverage and method coverage using coverage tools like Eclemma and Code Cover. We also drew the data flow diagrams to better understand the variable usage in te various methods. Finally we compared the results from our previous assignments to understand how the changes affected the coverage of the program

# 2 Manual data-flow coverage calculations for X and Y methods

Text…

# 3 A detailed description of the testing strategy for the new unit test

To start off this lab, we started  by reading through the new DataUtilities and Range files given to us. Then we identified methods,differences and similarities between the files in DataUtilities and Range in Assignment2 and Assignment3.  Then we set up our eclipies according to the instructions given on github. 
Here are few steps we did 

Step1) We checked the coverage we achieved with the previous tests we made in assignment 2 to check how much scope of the code was covered. 
Step2) We listed out methods that need more coverage, code with no coverage.
Step 3) Then we divided the work in a team of two, where one pair worked on DataUtilities and the other worked on Range.
Step4) Then we decided to exponentially  increase the coverage by working on the Method coverage metrics first and then work with the branch coverage metrics . 


# 4 A high level description of five selected test cases you have designed using coverage information, and how they have increased code coverage


DATA UTILITIES 

Function:Equals which is used to ensure two 2d Arrays are similar so for this function we used the branch coverage metrics to check if all the branches are covered. Initially only had 0 percent coverage later we add come test case like where a is null or b = null which increased it to 50 percent and with the help of Eclemma we determined the branch that was not checked and then made the respective test case to have 100 percent coverage.

Function: Clone which is used to ensure 2d Array is cloned. With the help of Eclemma we figured that we had not written a test for it initially as it was a new function but after writing a test it went from 0 percent line coverage to 100 percent. Overall, a 5 percent increase in line coverage and 3 percent in branch coverage

Function: static double calculateRowTotal(Values 2D data, int row). This function is used to compute the row total based on the row number. We used Eclemma to identify a case that will never be able to be executed as the case where the column is 0 or negative  is not possible in an  2D array or array in general.

Range

Function: shiftWithNoZeroCrossing(double value, double delta). This was a private function so it was not possible to write a function that would be able to test it so we had to find cases where this function was getting called. This function was getting called by a function called Shift(Range base, double delta, boolean allowZeroCrossing). So we made test cases where shiftWithNoZeroCrossing is called and all the possible branches are covered.

 Function: hashCode(). This function also had zero coverage initially but with the help of Eclemma. We wrote test and increase the overall  line coverage from 78 percent to 82 percent 


# 5 A detailed report of the coverage achieved of each class and method (a screen shot from the code cover results in green and red color would suffice)

Text…

# 6 Pros and Cons of coverage tools used and Metrics you report

Text…

# 7 A comparison on the advantages and disadvantages of requirements-based test generation and coverage-based test generation.

Text…

# 8 A discussion on how the team work/effort was divided and managed

Text…

# 9 Any difficulties encountered, challenges overcome, and lessons learned from performing the lab

Text…

# 10 Comments/feedback on the lab itself

Text…
