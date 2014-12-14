Distance Based Point Clustering Tests
============

##Objectives

The goal of our project was to create python versions of distance-based point clustering tests. This inclues the mean nearest neighbor test, the G, F, and J functions, and the K and L functions. 

##Implementation

We used iPython Notebook and the NumPy, SciPi, and MatPlotLib libraries to build our functions. Due to time restraints we were unable to build functions for all of the cluster tests. We made progress on the G function, and have a working mean nearest neighbor test.

Our first step was to build a function that created a distance matrix. This function, (NAME), was then nested within the "mean-nn-test" function, which finds the average nearest neighbor for the user's inputted data, and then compares that value to a normal distribution. The function creates 9999 random distance matrixes by shuffling the X values randomly. The mean nearest neighbor is calculated for each random dataset to create the normal distribution. These results are then plotted using MatPlotLib so that the user gets a visual represenation of thier mean nearest neighbor versus a normal distribution. The tool also reports a p value, which tells the user whether or not the results are statistically significant. 

The G function analyzes the data a bit differently. Using the pair-wise nearest neighbor distances for each point from the distance matrix, the function plots the cumulative number of nearest neighbor pairs against distance length. The resulting shape of the graph give you insight into the distribution of nearest-neighbor distances. If the graph rises very quickly, it means there is a high number of short nearest-neighbor distances, indicating clustering. While we were able to create a function that runs the G function on user inputted data and plots the result, we have not been able to get code working that compares the G function results to a normal distribution.

Examples of our functions can be seen in the above Dist2.ipynb.

##Conclusion

We were limited as a team by a lack of understanding of the distance-based clustering test functions. None of us have a statistical or mathematical background, and we struggled to translate the equations into geocomputational python-based tools. We were also limited as beginning python and git-hub users. No one had written tools beyond simple brute force functions, and we lacked knowledge of optimization techniques. Most of the code was given to us by our collaborator Serge Rey.

We had hoped to incorporate KD-trees to speed up the creation of our distance matrixes, but again, as beginning programmers we were unable to get the code working. With more time a practice with Python, tools for the remaining functions can be created. 
