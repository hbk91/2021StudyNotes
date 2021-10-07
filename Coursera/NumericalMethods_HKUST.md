---
title: "Numerical Methods for Engineers by HKUST (Coursera)"
author: "Aman Jindal"
---

<a href='https://www.math.hkust.edu.hk/~machas/numerical-methods-for-engineers.pdf' target="_blank">This is the book</a> being followed in this course. The course is taught by <a href ='https://www.math.hkust.edu.hk/~machas/' target="_blank">Professor Jeffrey R. Chasnov</a>.


### A. Matlab Notes:

1. A good place to get an understanding of Matlab is <a href='http://www.math.ucsd.edu/~bdriver/21d-s99/matlab-primer.html' target="_blank">this</a>
2. Several expressions, separated by comma or semicolons, can be placed on a single line.


### B. Week 1:

1. Learnt how to use MATLAB. 
2. Understood the concept of <a href="https://en.wikipedia.org/wiki/Logistic_map" target="_blank">logistic map</a>. <a href='https://www.youtube.com/watch?v=ovJcsL7vyrk' target="_blank">This video by Veritasium</a> provides a good explanation. 
3. Mathematically, Logistic Map is written as ***x<sub>n+1</sub> = rx<sub>n</sub>(1-x<sub>n</sub>)***. 
4. ***x<sub>n</sub>*** is a number between zero and one, that represents the ratio of existing population to the maximum possible population.
5. ***r*** is the growth rate of the population.
6. Computed & presented the bifurcation diagram for the logistic map in MATLAB. 


### C. Week 2:

1. Learnt three methods for finding roots viz. Bisection method, Newton method & Secant method.
2. Newton's method is the fastest (speed of convergence), followed by Secant method and then Bisection method. 
3. The order of convergence for the three methods are: Bisection: ***1***, Secant: ***1.6***, Newton: ***2***. The order of convergence signifies with what power the error decreases.
4. Bisection method would always provided a solution, while the Newton method will only provide  solution when an analytical derivative for the function exists. 
5. Secant method is a way for resolving the above shortcoming of Newton method. It approximates the derivative when the derivative for the function doesn't exist.
6. A fractal is a geometrical object that looks similar on all scales. The Newton Fractal is explained in <a href='https://www.youtube.com/watch?v=TOR37v5GV5o' target="_blank">this video</a>.
7. Period doubling route to chaos.
8. Computed the Feigenbaum Delta by solving the logistic map until the period 11 cycle of r. 


### D. Week 3:

