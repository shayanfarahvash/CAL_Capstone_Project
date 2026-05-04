### Optimal Design of a 3-stage Ladder LC Bandpass Filter with an Arbitrary Frequency Response 

Shayan Farahvash


<font color="blue">***Executive Summary***</span>


The objective of this Capstone projects is to design a 3-stage ladder LC filter to deliver a desired frequency response subject to the following conditions 

1- One band pass only. For this project we set it to be between 2300MHz to 2400MHz but it can be any arbitrary span in frequency domain.

2- Multiple stop bands with nonuniform rejection (see below graph for an example). 

The aim  of this work is start from a dataset of an analytically derived sub-optimal solutions, use that to train a ML/AI regressor, and then use regressor to predict what would be the solution to a real world multiple stopband problems.


<p align="center">
  <img src="/Images/Image1.png" width="600" title="Project Graph">
</p>
Figure 1: Desired piecewise continuous frequency response of a filter along with LC filter response. Goal: minimize the difference between the two

  
<font color="blue">***Rationale***</span>


Filters play a key role in wireless and wireline devices by passing a desired signal to subsequent systems while simultaneously—and most crucially—rejecting all unwanted ones. These unwanted signals (often referred to as blockers or interferers) cause a range of negative system impacts, such as desensitization, aliasing, intermodulation, and compression. The strength and frequency of such signals can vary widely, requiring a filter with a flexible rejection profile that changes as a function of frequency.
The synthesis of bandpass LC networks with a given passband is a classic problem for which semi-optimal solutions have existed for decades. However, traditional filter design techniques, although highly analytical and proven, cannot be applied to such arbitrarily shaped responses—even with the most flexible filter types (e.g., elliptical filters). While certain designs, such as the inverse Chebyshev, can provide secondary rejection levels by realizing deep notches, these levels cannot be moved around arbitrarily without compromising the filter's passband response.


Given that there is no analytical solution for the problem stated above, the current approach to filter design is often ad-hoc. Components are typically tailored by hand or using optimization algorithms, such as genetic algorithms, to provide an approximation of the desired response. This project is an attempt to apply deep learning to solve this synthesis problem.
