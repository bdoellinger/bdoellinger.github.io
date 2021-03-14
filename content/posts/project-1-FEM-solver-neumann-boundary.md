---
date: 2021-03-01T10:00:59-04:00
description: "An implementation of a finite element method to solve a difficult PDE problem in python."
featured_image: "/images/project_1_FEM_project_image.png"
title: "Project 1: FEM solver with Neumann boundary conditions"
---

* libraries: numpy, pandas, matplotlib, mpl_toolkits, tkinter, PIL

Generally, solving partial differential equations (PDE's) is one of the practically most relevant mathematical problems (e.g. fluid mechanics, heat and mass transfer, wave propagation and electromagnetic theory is model with PDE's).
However for non trivial examples there are usually only unfeasible formulas for a solution (if there is even a known formula for solutions or a solution at all).
Hence, in practice we have to model our real life problem in a way that the problem has exactly one unique solution (i.e. choose the right boundary conditions) and use numerical methods to approximate the solution.

This project is an example of a python implementation of a finite element method (FEM) to solve the following PDE with Neumann boundary conditions:
{{< figure src="/images/project_1_FEM_project_image_of_problem.png" >}}
Here we use the 2 dimensional unit square as a test domain, however it is possible to generalize to more complex domain geometries and/or 3 dimensions (albeit the implementation would be more complex).
The FEM implementation is done in 3 steps:
* **1. Preprocessing:** For a given mesh parameter n, divide the domain into triangles using a Friedrich-Keller triangulation and enumerate the nodes and elements
* **2. Assembling:** Use a Ritz-Galerkin method with triangle wise construction of a system matrix A and system vector b, such that the solution u of Au = b numerically approximates the solution of the PDE in the nodes
* **3. Solving:** Solve the system Au = b using numpy to get the numerical solution u

To get user input, this application utilizes a GUI made with Tkinter. The mesh parameter n, the inhomogeneities f,g and the real parameter a_0 can be specified. Using the parameters the user can get a plot and .csv file of the numerical solution. The mesh parameter n can be chosen from 1 to 100. Choosing n=100 generates a mesh with 10201 nodes, which results in a system of 10201 equations with 10201 variables. Even in this case the computation time is only a few seconds with RAM usage below 2 GB, since the implementation is designed to be computational efficient.

{{< figure src="/images/project_1_FEM_project_screenshot.png" >}}

[Link to GitHub Repository](https://github.com/bdoellinger/01_FEM_project)
