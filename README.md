# Concept - Calculate Pi

Calculates pi given a number of random numbers between -1 and 1

[A video explaining this concept from Joma Tech](https://www.youtube.com/watch?v=pvimAM_SLic)

This firebase app demonstrates how to calculate π given a number of random pairs with x and y values between -1 and 1. With enough points, this should approach π. As π is a constant and irrational, this will never truly equal pi, however we can get a good estimation. 

We can do this by determining the area of the circle and the area of the square. 

Area of a circle = πr²

Area of a square = (2r)²

The ratio of points within the circle should be the same as the ratio of circle area within the square, which should be pi. That's to say

*πr²/(2r)² = circlepoints / totalpoints*

Given that r = 1 and isolating for π, we can simplify this to 

*π = 4 * circlepoints / totalpoints*


To determine if a point is within a circle, we can use the Pythagorean Theorem. 

a² + b² = c²


If the hypotenuse (c) is greater than our r² (1²), then this point falls outside of the area of the circle. To determine if it is within the circle, we simply add the pair of random numbers squared and determine if it's less than 1. 

You can see points generated on a graph with this application [here!](https://concept-calculatepifromx.web.app/)