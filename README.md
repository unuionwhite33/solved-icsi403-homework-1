Download Link: https://assignmentchef.com/product/solved-icsi403-homework-1
<br>
The objective of this programming assignment is to implement two different algorithms for the closest pair problem and experimentally compare their computation times.




In the closest pair problem, we are given a set of n points in the plane. Each point is specified by its x and y coordinates, which are real numbers. Recall that given two points p = (x<sub>p</sub>, y<sub>p</sub>) and q = (x<sub>q</sub>, y<sub>q</sub>), the (Euclidean) distance d(p, q) between them is given by the formula




The goal of the closest pair problem is to find the shortest distance between any pair of points in the set.




A simple (brute-force) method of computing the shortest distance is to compute the <em>n </em>(<em>n</em> – 1)/2 distances between all pairs of points and take the smallest of these distance values. Clearly, this algorithm runs in Θ(<em>n</em><sup>2</sup>) time. For this problem, there is a divide-and-conquer algorithm that runs in O(<em>n</em> log <em>n</em>) time. A description of this algorithm was presented in class (see lecture slides, also Chapter 33.4 of the book). You are required to implement both the brute-force algorithm and the divide-and-conquer algorithm and determine the actual times used by these two algorithms on test inputs. There are two parts to this assignment.




<strong><u>Part (a):</u></strong> Implement the <em>Brute Force</em> and <em>Divide-And-Conquer</em> algorithms. Use the ClosetPair.java file to hold your methods. Consult the lecture slides for the pseudocode and analysis justifying the Θ(<em>n</em><sup>2</sup>) and O(<em>n</em> log <em>n</em>) growth rates respectively. Beyond compilable, all tests should be defined in the driver class should pass with success. Please document your justification of the test you used in comments.




<strong><u>Part (b):</u></strong> In this part, you are required to experiment with inputs of sizes 10,100,1000 and 10000 by employing the random point generator that you should implement in ClosestPairDriver.java. To do this analysis, you should implement a runnningTimeComparison() method in the ClosestPairDriver.java. Report the computation times of the two algorithms as discussed below.




Using the outputs produced by your algorithms, you should prepare a table with four rows (one corresponding to each size) and three columns labeled <strong><em>No. of points</em></strong>, <strong><em>Time used by Brute Force</em></strong> and <strong><em>Time used by Divide-and-Conquer</em></strong>. Plot this table (using MS Excel or any other software for plotting) in a line chart with x axis the number of points and y axis: time taken by an algorithm. You will have two curves: one for each of the algorithm. Plot also in the same figure the <em>f(n) = c<sub>1</sub>n<sup>2</sup></em> and <em>g(n) = c<sub>2</sub>n </em>log<em> n</em> functions for the same range of number of points n = (10, 100, 1000, 10000), by choosing appropriate constants c1 and c2 to fit visually your observed running times. Discuss what you observe about those constants. Do they matter for small <em>n</em>? How about, large <em>n</em>?




The table, your explanation and plots and plots should be submitted as a separate PDF or MS word file