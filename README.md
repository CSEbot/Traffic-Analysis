# Traffic-Analysis
This GitHub repository contains the Python implementation of a city planning simulator for reducing traffic congestion and journey time in a stochastic environment.

# City Planning Simulator
This GitHub repository contains the Python implementation of a city planning simulator for reducing traffic congestion and journey time in a stochastic environment. This project aims to assist city planners in determining optimal new road constructions by simulating traffic volumes across an existing road network. The simulator utilizes NetworkX, a Python-based toolkit for graph operations.

# Purpose
Gain a comprehensive understanding of agent-based navigation in a stochastic environment akin to real-world scenarios. Collaborate with a partner or work individually, reading the project specification thoroughly to comprehend requirements. Develop a strategy, document functional requirements, and assumptions before coding in Python.

# Environment Description
The city's road network is modeled as a graph, with nodes representing locations and edges as roads connecting them bidirectionally. The objective is to identify new road constructions to minimize journey time and traffic congestion.

# Simulator Overview
The simulator, based on NetworkX, runs simulations to estimate traffic volumes across the road network. Due to time constraints, data collection occurs over a single day of simulation time. Every clock tick represents one second, generating 100 trips between randomly selected start and end locations.

# Traffic Analysis
After data gathering, the algorithm recommends new roads for construction based on a weighted measure of traffic volume and road length. For example, a simple benefit calculation considers trip counts and road lengths to prioritize new road constructions.

# Simulation Parameters
N: Fixed at 60 for the number of locations (nodes) in the network.
p: Average connectivity of nodes, with a fixed value of .05.
L: Road length parameter ranging from 5 to 25.
T: Default value of 100 trips generated at each clock tick.
k: Budget parameter, defaulting to 3 new roads.
f: Shrinkage factor for new road lengths, with values of 0.6 or 0.8.
