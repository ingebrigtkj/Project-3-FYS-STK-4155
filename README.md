With inspirations taken from Machine Learning methods and Neural Networks, this project was motivated by the desire to solve a particular Partial Differential Equation with Machine Learning methods and comparing the results to the ones obtained by solving the same PDE with an analytical approach and a Standard Explicit Scheme Algorithm. In this project I am solving a PDE representing the temperature grid of a rod using Recurrent and Convolutional Neural Networks, which was chosen due to their current popularity in solving complex problems in Machine Learning, and a desire to test their flexibility and scope in using parameters and making modifications to fit specific problems while also evaluating the computational costs.

Specifically, this is Project 3 in the subject FYS-STK4155(University of Oslo), containing
3 python code files, using a Standard Explicit Scheme, Recurrent Neural Network and Convolutional Neural Network to solve the PDE:

The physical problem is the
temperature gradient in a rod of length L = 1 at x = 0 and x = 1. It is a 
one-dimensional problem
∂
2u(x, t)
∂x2
=
∂u(x, t)
∂t , t > 0, x ∈ [0, L]
or
uxx = ut,
with initial conditions, i.e., the conditions at t = 0,
u(x, 0) = sin (πx) 0 < x < L,
with L = 1 the length of the x-region of interest. The boundary conditions are
u(0, t) = 0 t ≥ 0,
and
u(L, t) = 0 t ≥ 0.
3
The function u(x, t) is the temperature gradient of a rod. As time increases,
the velocity approaches a linear variation with x.
Here I am looking at the so-called explicit forward Euler algorithm with
discretized versions of time given by a forward formula and a centered difference
in space resulting in
ut ≈
u(x, t + ∆t) − u(x, t)
∆t
=
u(xi
, tj + ∆t) − u(xi
, tj )
∆t
and
uxx ≈
u(x + ∆x, t) − 2u(x, t) + u(x − ∆x, t)
∆x
2
,
or
uxx ≈
u(xi + ∆x, tj ) − 2u(xi
, tj ) + u(xi − ∆x, tj )
∆x
2
.

The solution contains a discretization of the PDE (Spatial and time-discretized) using both the Euler's Forward Method and Implicit Euler's Method. It is solved by the Recurrent and Convolutional Neural Network by interpreting the input image you would expect for the Convolutional Neural Network as "patches" from the discretized PDE. The solutions are analyzed using RMSE and Loss and a prediction of the Temperature Gradient across time.

Features Shareable Links: Share your document securely by sending a custom link Python Code: Models and Analysis were performed using the programming language Python. Self-hosted, open-source

Teck Stack: Spyder --> https://www.spyder-ide.org/ - Program to write Python Jupyter Notebook --> https://jupyter.org/install - Online program to write Python Anaconda3 --> https://www.anaconda.com/download/ - Used Python distribution used in data science, machine learning applications, large-scale data processing, predictive analytics etc. to simplify package management and deployment Libraries - scikit-learn, install by typing "conda install -c conda-forge scikit-learn or pip- install scikit-learn" in anaconda3 command propmpt, numpy, install by "pip install numpy" and scipy, install by "pip install numpy"

The file "Project 3 Explicit Scheme and Analytical Solution" contains an analytical solution the PDE solved with Python, and a Standard Explicit Scheme Algorithm for solving the PDE using both the Euler's Forward Method and Implicit Euler's Method, at different time points for different values of Delta(T). The file "Project 3 Recurrent Neural Network" contains the solution of the PDE using a Recurrent Neural Network with different activation functions and parameters such as momentum, learning rates, l2-regularization, dropout and gradient clipping. The file "Project 3 Convolutional Neural Network" contains the solution of the PDE using a Convolutional Neural Network with different parameters. The file "Project 3.pdf" is a report over everything that has been done and the mathematical assumptions of the PDE and the models used along with an analysis of the results and a critical comparison of the methods.

Run the code w.: Spyder, Jupyter Notebook or another Python environment Read the report w. Microsoft Edge internet browser or Acrobat Reader
