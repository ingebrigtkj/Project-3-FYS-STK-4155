Project 3 FYS-STK4155, 3 python code files, using a Standard Explicit Scheme, Recurrent Neural Network and Convolutional Neural Network to solve the PDE:

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

Features Shareable Links: Share your document securely by sending a custom link Python Code: Models and Analysis were performed using the programming language Python. Self-hosted, open-source

Teck Stack: Spyder --> https://www.spyder-ide.org/ - Program to write Python Jupyter Notebook --> https://jupyter.org/install - Online program to write Python Anaconda3 --> https://www.anaconda.com/download/ - Used Python distribution used in data science, machine learning applications, large-scale data processing, predictive analytics etc. to simplify package management and deployment Libraries - scikit-learn, install by typing "conda install -c conda-forge scikit-learn or pip- install scikit-learn" in anaconda3 command propmpt, numpy, install by "pip install numpy" and scipy, install by "pip install numpy"

Run the code w.: Spyder, Jupyter Notebook or another Python environment Read the report w. Microsoft Edge internet browser or Acrobat Reader
