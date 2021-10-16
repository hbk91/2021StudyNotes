---
title: "Numerical Methods for Engineers by HKUST (Coursera)"
author: "Aman Jindal"
---

<a href='https://www.math.hkust.edu.hk/~machas/numerical-methods-for-engineers.pdf' target="_blank">This is the book</a> being followed in this course. The course is taught by <a href ='https://www.math.hkust.edu.hk/~machas/' target="_blank">Professor Jeffrey R. Chasnov</a>.


### A. Matlab Notes:

1. A good place to get an understanding of Matlab is <a href='http://www.math.ucsd.edu/~bdriver/21d-s99/matlab-primer.html' target="_blank">this</a>. Matlab is generally case-sensitive. More on case sensitive <a href="https://www.mathworks.com/matlabcentral/answers/442925-is-matlab-case-sensitive-in-all-aspects" target="_blank">here</a>
2. Several expressions, separated by comma or semicolons, can be placed on a single line.
3. Semi-colon at the end of the line suppresses the value of the expression in that line. Else, the value is displayed.
4. Ax = b; x is solved using the backslash operator as: x = A\b;
5. A = LU; LU decomposition of a matrix is obtained as: [L, U] = lu(A)
6. Ax = L(Ux) = b; x is solved as : x = U\(L\b)
7. Eigenvalues: lambda = eig(A)
8. Eigenvalues & Eigenvectors: [V, D] = eig(A). V is matrix of Eigenvectors and D is the matrix of Eigenvalues. The eigenvalues are on the leading diagonal of D. The first eigenvalue corresponds to the first column eigenvector in V and so on and so forth.
9. <a href="https://www.mathworks.com/help/matlab/ref/fzero.html" target="_blank">**fzero**</a> is the matlab function that is used to find root of a non-linear function.
10. <a href="https://www.mathworks.com/help/matlab/ref/interp1.html" target="_blank">**interp1**</a> is the matlab function that is used for 1-D interpolation including cubic spline interpolation.
11. 11. <a href="https://in.mathworks.com/help/matlab/ref/ode45.html" target="_blank">**ode45**</a> is the matlab function that is used for integrating ODEs. 

### B. Week 1:

1. Learnt how to use MATLAB. 
2. Understood the concept of <a href="https://en.wikipedia.org/wiki/Logistic_map" target="_blank">logistic map</a>. <a href='https://www.youtube.com/watch?v=ovJcsL7vyrk' target="_blank">This video by Veritasium</a> provides a good explanation. 
3. Mathematically, Logistic Map is written as **x<sub>n+1</sub> = rx<sub>n</sub>(1-x<sub>n</sub>)**. 
4. **x<sub>n</sub>** is a number between zero and one, that represents the ratio of existing population to the maximum possible population.
5. **r** is the growth rate of the population.
6. Computed & presented the bifurcation diagram for the logistic map in MATLAB. 


### C. Week 2:

1. Learnt three methods for finding roots viz. Bisection method, Newton method & Secant method.
2. Newton's method is the fastest (speed of convergence), followed by Secant method and then Bisection method. 
3. The order of convergence for the three methods are: Bisection: **1**, Secant: **1.6**, Newton: **2**. The order of convergence signifies with what power the error decreases.
4. Bisection method would always provided a solution, while the Newton method will only provide  solution when an analytical derivative for the function exists. 
5. Secant method is a way for resolving the above shortcoming of Newton method. It approximates the derivative when the derivative for the function doesn't exist.
6. A fractal is a geometrical object that looks similar on all scales. The Newton Fractal is explained in <a href='https://www.youtube.com/watch?v=TOR37v5GV5o' target="_blank">this video</a>.
7. Period doubling route to chaos.
8. Computed the Feigenbaum Delta by solving the logistic map until the period 11 cycle of r. 


### D. Week 3:

1. Gaussian elimination without pivoting may lead to wrong answers while solving a system of linear equations due to round-off error.
2. Partial Pivoting means row interchange. Complete Pivoting means both row and column interchange.
3. Gaussian elimination with partial pivoting generally obviates the problem of wrong answers due to round-off errors. This was one of the greatest discoveries in Numerical Analysis.
4. LU decomposition of a matrix using partial pivoting. Post LU Decomposition, we can use backward and forward substitution to solve a system of linear equations. <a href="https://www.math.ucdavis.edu/~linear/old/notes11.pdf" target="_blank">This link</a> explains the LU decomposition.
5. LU decomposition is superior to Gaussian elimination, when the right hand side of the equation keeps on changing (for instance in PDEs). Thus, we can do the LU decomposition once, and then used backward & forward substitution repeatedly as the right hand side keeps on changing. Gaussian elimination scales as **O(N<sup>3</sup>)**. Forward and Backward substitutions scale as **O(N<sup>2</sup>).**  
6. Computed & Plotted the fractal by solving the Lorenz Equations.

### E. Week 4:

1. Quadrature is numerical integration. 
2. Learnt the Midpoint Rule, Trapezoidal Rule & Simpson Rule. Learnt Quadrature rules viz. Composite, Gaussian and Adaptive. Matlab uses Adaptive Quadrature.
3. Learnt interpolation methods viz. linear, polynomial. Cubic Spline is a cubic polynomial spline interpolations between different points on the curve.
4. In the project computed the first five positive roots of the first six Bessel Functions.

### F. Week 5:

1. Euler Method is a first order method of solving ODE. Let the differential equation be **dx/dt = f(t,x)**, with the initial condition **X(t<sub>0</sub>) = X<sub>0</sub>**
2. Euler's Method can be summarized as marching forward from an initial condition in this fashion: **x<sub>n+1</sub> = x<sub>n</sub> + t<sub>delta</sub> f(t<sub>n</sub>, x<sub>n</sub>)**
3. Learnt the Runge-Kutta (RK) the method. Learnt the Modified Euler Method and its expression as a Second order Runge-Kutta Method. Also, the General Second order, Third Order Runge-Kutta Method. Further, an example of Fourth order Runge-Kutta Method. 
4. Matlab uses Adaptive Runge-Kutta (RK) methods where itself figures appropriate t<sub>delta</sub>. We need to specify only the error tolerance. Smaller the error tolerance, smaller will be t<sub>delta</sub> and more expensive the computation.
5. **ode45** (Matlab Function) uses Dormand Prince Method which is a six stage (fifth order) Runge-Kutta method.
6. Solved the <a href="https://en.wikipedia.org/wiki/Two-body_problem" target="_blank"> two body problem</a> (predict the motion of two massive objects which are abstractly viewed as point particles. The problem assumes that the two objects interact only with one another; the only force affecting each object arises from the other one, and all other objects are ignored) using **ode45**.

### F. Week 6:
   