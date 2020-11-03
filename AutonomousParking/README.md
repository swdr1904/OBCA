# OBCA - Autonomous Parking
Optimization-Based Collision Avoidance - an application towards autonomous parking

Paper describing the theory can be found [here](http://arxiv.org/abs/1711.03449).

## How to run the Parking code:

**WARNING:This code seems to be working on Julia v1.5.2, but with the current configuration, the solver cannot find any solutions. Therefore, this code may contain a bug.**

If you just want to try Hybrid-A\*, use the following repositories: https://github.com/AtsushiSakai/HybridAStarTrailer

### First steps

1. Change to the directory

2. Install Julia from https://julialang.org/downloads/ (code tested on Julia v1.5.2) 

3. Open Julia in terminal and enter the Pkg REPL by pressing `]` from the Julia REPL

4. Install Julia package JuMP using `add JuMP`

5. Install Julia package Ipopt using `add Ipopt`

6. Install Julia package PyPlot using `add PyPlot`

7. Install Julia package NearestNeighbors using `add NearestNeighbors`

8. Install Julia package DataStructures using `add DataStructures`

9. Install Julia package  DataFrames using `add DataFrames`


### Running the parking example 

1. Start Julia in terminal

2. Type in terminal: include("setup.jl")

3. Type in terminal: include("main.jl")


### modifying the code 

1. To play with start points, change x0 in main.jl and run 
the code by include("main.jl")

2. If you change anything in one of the collision avoidance
problems, you need to activate the changes by running 
include("setup.jl")


### Note
1. This code is tested on Julia v1.5.2. Packages of the test environment are following:
    * JuMP v0.21.5
    * Ipopt v0.6.3
        * The original code has been tested on Julia 0.5 and 0.6, and might not run on any other Julia versions.

2. For best results, run code in Julia terminal
