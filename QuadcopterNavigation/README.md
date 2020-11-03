# OBCA - Quadcopter Path Planning
Optimization-Based Collision Avoidance - an application in quadcopter path planning

Paper describing the theory can be found [here](http://arxiv.org/abs/1711.03449).

## How to run the code:

### First steps

1. Change to the directory

2. Install Julia from https://julialang.org/downloads/ (code tested on Julia v1.5.2) 

3. Open Julia in terminal and enter the Pkg REPL by pressing `]` from the Julia REPL

4. Install Julia package JuMP using `add JuMP`

5. Install Julia package Ipopt using `add Ipopt`

6. Install Julia package PyPlot using `add PyPlot`

7. Install Julia package NearestNeighbors using `add NearestNeighbors`

8. Install Julia package DataStructures using `add DataStructures`

### Running the parking example 

1. Start Julia in terminal

2. Type in terminal: include("setupQuadcopter.jl")

3. Type in terminal: include("mainQuadcopter.jl")


### modifying the code 

1. To play with start points, change xF (or x0) in mainQuadcopter.jl and run 
the code by include("mainQuadcopter.jl")

2. If you change anything in one of the collision avoidance
problems, you need to activate the changes by running 
include("setupQuadcopter.jl")


### Note

1. This code is tested on Julia v1.5.2. Packages of the test environment are following:
    * JuMP v0.21.5
    * Ipopt v0.6.3
        * The original code has been tested on Julia 0.5 and 0.6, and might not run on any other Julia versions.

1. Time measurement code in distance calculation of the original code is invalidated. If you have any idea, please make an issue or a pull request to fix this problem.

1. For best results, run code in Julia terminal
