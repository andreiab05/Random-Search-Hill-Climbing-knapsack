# Metaheuristic Optimization for the Knapsack Problem

## Overview
This project implements and analyzes metaheuristic algorithms for solving the 0/1 Knapsack problem.

Two optimization strategies are implemented and compared:
- Random Search
- Hill Climbing

The goal is to evaluate how different parameters influence the quality of the obtained solutions.

## Problem Description
The 0/1 Knapsack problem consists of selecting a subset of items such that:

- the total weight does not exceed the knapsack capacity
- the total value of the selected items is maximized

Each item has:
- weight
- value

The problem is NP-hard, making metaheuristic approaches useful for large instances.

## Implemented Algorithms

### Random Search
Random solutions are generated and evaluated.  
The best solution found during the search is kept.

### Hill Climbing
Starts from a random solution and iteratively moves to a better neighbor solution if one exists.

## Experiments

The algorithms were tested on two datasets:

- `knapsack-20.txt` – small instance
- `knapsack-200.txt` – large instance

Each algorithm was executed multiple times with different parameters.

The results include:
- best solution value
- average solution value across runs

## Example Results

| Instance | Runs | k | Best Value | Average Value |
|---------|------|----|-----------|--------------|
| knapsack-20 | 100 | 100 | 755 | 674.01 |
| knapsack-200 | 100 | 100 | 97479 | 96733.11 |

## Technologies
- Python
- Jupyter Notebook
- Markdown documentation
