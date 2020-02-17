This week's practical exercises aim to get you familiar with Java and IntelliJ IDEA via basic programming exercises.

# Hello World!

Open `HelloWorld.java` and modify the code such that the program prints "Hello World!" when run.

# Debugging a summation program

This exercise will give you practice using IDEA's debugger. Open `Summation.java`. This program is meant to calculate the sum of the natural numbers in a given range. The range is expressed by constants for the starting and finishing numbers, inclusive. Recall, for instance that the sum of `i` over 1<=`i`<=5 is 15.

**(a)** Run the program with a `START` value of 1 and an `END` value of 5. Is the answer what you expected? In the `add()` method click in the grey bar just to the left of the __`for`__ loop statement (in the space between the line numbers and the code). This adds a _breakpoint_ to the application. Now 'debug' rather than 'run' the program. You will be able to control the program's execution using the various debugging buttons ![various debugging icons](imgs/debugbtns.png "various debugging icons"). Step through the program and watch how variables `index` and `total` change. By doing this you should be able to spot and fix the coding error.

**Note:** If you hover the cursor over a variable when the program is stopped the variable's value is displayed.

**(b)** Having corrected the error in the program, now change the value of constant `END` to 1000. Run the program. Does the answer look correct? Debug the program again and see if you can identify and fix this new problem. (This may require some patience!)

# Footy Score

This exercise will give you experience at developing a simple (concrete) _class_ in Java. In Australian Rules Football, teams earns _points_ by kicking _goals_, worth six points each, and _behinds_, worth one point each. Your job is to create `FootyScore.java` which keeps track of the score earned by a particular team. This class needs to:

* declare a private data structure sufficient to keep track of the team's score;
* declare a parameterless public method called `getPoints` that returns the team's total score in points;
* declare a parameterless public method called `kickGoal` that records the fact that the team has kicked a goal;
* declare a parameterless public method called `kickBehind` that records the fact that the team has kicked a behind;
* declare a parameterless public method called `sayScore` that returns a character string representing the way Australian Football League commentators traditionally say AFL scores, as three numbers, consisting of the number of goals kicked, the number of behinds kicked, and the total number of points earned, in that order; and
* declare a predicate (boolean-valued function) called `inFrontOf` which accepts a `FootyScore` object as its parameter and returns true if and only if (iff) this team's score exceeds that of the team provided as an argument.

To help you assess your solution the file `FootyTester.java` contains a 'main' program that simulates a (rather low scoring) AFL match between traditional rivals
Collingwood and Richmond. It prints the breathless commentary of a typically rabid AFL announcer. If your solution works correctly, the test program will print the following
commentary on the console. Note that your `sayScore` method should return the three numbers separated by a comma and a space.

    At the end of the first quarter, it's Collingwood, 0, 2, 2 and Richmond 1, 0, 6.
    Richmond lead by 4 points!
    At the end of the second quarter, it's Collingwood, 2, 3, 15 and Richmond 3, 0, 18.
    Richmond lead by 3 points!
    At the end of the third quarter, it's Collingwood, 3, 3, 21 and Richmond 3, 2, 20.
    Collingwood lead by 1 point!

(We leave the final score in doubt to avoid offending any Collingwood or Richmond
supporters in the class.)

