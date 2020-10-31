# Hypothesis testing

In this exercise, I am going to do a lot of lying.  In the descriptions in the cell on the right, I will tell you how I generated the data in the input files by sampling from random variables.  On some occasions I will be telling you the truth in these descriptions and in others I will be lying my pants off.  Your task is thus to determine whether I am being truthful or not.

This is not an idle exercise.  We often need to be able to compare the results we get when we perform experiments with the predictions that our theories about the world make.  In the language above this sort of comparison amounts to determining whether or not I am lying when I tell you how the data was generated.  Furthermore, the methods used to make these sorts of determinations are the same as the methods that you will use to expose my duplicity.

Let's start by trying to determine why these formal methods are necessary.   I have generated 200 standard normal random variables for you and stored them in the array called samples.  To complete this exercise you must construct a histogram from this data.  The variable we have sampled is a continuous random variable.  Your histogram will thus be an estimate of the probability density function for the underlying random variable.

To pass the test your histogram should have 15 bins (`nbins`).  The first of these bins should start at -4 (`minv`) and the last of them should end at +4 (`maxv`).  The width of each bin should be equal to `delx`.  I have also created two numpy arrays for you:

1. `xvals` - will eventually hold the midpoints of all the bins
2. `counts` - will eventually hold the estimate of the probability density at the midpoint 

I have plotted the probability density function for this function on the graph for you.
