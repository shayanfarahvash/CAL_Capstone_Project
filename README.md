### Optimal Design of a 3-stage Ladder LC Bandpass Filter with an Arbitrary Frequency Response 

Shayan Farahvash


<font color="blue"> ***Executive Summary***</span>


The objective of this Capstone projects is to design a 3-stage ladder LC filter to deliver a desired frequency response subject to the following conditions 

1- One band pass only. For this project we set it to be between 2300MHz to 2400MHz but it can be any arbitrary span in frequency domain.

2- Multiple stop bands with nonuniform rejection (see below graph for an example). 

The aim  of this work is start from a dataset of an analytically derived sub-optimal solutions, use that to train a ML/AI regressor, and then use regressor to predict what would be the solution to a real world multiple stopband problems.


<p align="center">
  <img src="/Images/Image1.png" width="600" title="Project Graph">
</p>

<center>Figure 1: Desired piecewise continuous frequency response of a filter along with LC filter response. Goal: minimize the difference between the two</center>
