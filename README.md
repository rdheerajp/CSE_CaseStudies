# Case Studies HS 2021 (as a part of MSc CSE program at D-MATH, ETH Zurich)
## Topic: Cellular Automaton theory to simulate pedestrian dynamics

This repository serves to be a supplement to a presentation on the application of CA theory for efficient and quicker simulation of pedestrian dynamics.

Disclaimer: All of the work and results are directly derived from the work of Andreas Schadschneider [mailto:as@thp.uni-koeln.de], which are reported in the papers cited apropos.

# Section 1: Introduction

## Motivation
It is relatively clear from the title that we are interested in simulations of pedestrians and the dynamic evolution of their movement through complex spaces.

**Why, right?**

However, I firmly believe that one as a human, in the capacity of an engineer/scientist or any profession, should be aware of the impact (positive/negative) that follows. And that should motivate one to solve problems. That's my seven cents.

One such potential impact area of this work is the following: Consider you are to approve a building plan. How do you predict possible blockades during evacuations? How do you account for the effect of panic during the process?

Well, that's enough pep talk.

## The Real Problem
Now that we are passionate(?) about simulating pedestrian movement, Cellular Automata theory provides an excellent framework for such a problem.

- Firstly, we are dealing with a discrete system. Computers used for such simulations are also discrete systems. Hence, no particular discretisation scheme used in methods such as FVM/FEM is necessary.
- Consequently, there is no discretisation error as the governing rules/dynamics do not assume any continuum criterion.
- We are not limited to deterministic tools anymore, such as in classical models with differential equations. Using stochastic components improves the fidelity of our simulation as it accommodates inherent randomness. However, we would be required to average over several executions to arrive at a generic solution.

