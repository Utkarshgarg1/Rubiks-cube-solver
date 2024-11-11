# Rubik's Cube Solver Using IDA* and DFS

A fully implemented Rubik's Cube that allows you to make all possible moves with the functionality of 
solving the Rubik's Cube using the IDA* (Iterative Deepening A Star) algorithm and DFS (Depth First Search).

Cube solver created using the IDA* (Iterative Deepening A Star) algorithm 
involving DFS (Depth First Search), heuristic value calculation (using the Manhattan Distance) and optimized 
using pruning techniques such as preventing the algorithm from iterating over the same cube state again.

<img width="400" alt="Screenshot 2024-03-17 at 5 37 20 PM" src="https://github.com/Jai0212/Rubiks-Cube-Solver-Using-IDA-Star/assets/86296165/80c9c474-bff0-4d90-a1ec-457727b8f134">

## Features
- Solves the Rubik's Cube extremely fast using the IDA* algorithm coupled with DFS and perform all the moves
required to reach the solution 
- Heuristic value generated using the Manhattan Distance for accurate results and preventing overestimation
- Optimized by adding functionality such as preventing iteration over the same cube state again

### Algorithms

**Depth Limited Search Algorithm (DLS Algorithm)**

In AI we have 2 main methods of searching: **Informed and Uninformed searching**. In an Uninformed search, we don’t know how far or close are we to the goal, so with checking of reach a goal or not, we continue our move in all possible directions, but in Informed search, we know where our goal is and how far or close we are to the goal, so we define a heuristic which determines which move to choose.

The **DLS** search algorithm is one of the uninformed search methods in Artificial Intelligence so that the goal is not clear and we must reach the goal through uninformed moves of the target.

Every state of the agent (cube in this example) is called a node. Each of these nodes can produce a new node (they are called parent nodes which produce child nodes) by moving to its next state, so all possible modes are available. These newly made nodes would be a new parent node to new nodes that could be produced by them.

The DLS algorithm determines the depth to extend in various nodes and determines how deep the initial node goes. The final non-goal solution returns to the previous state that it can be checked. This algorithm is graphical as follows:

<p> <img src="https://user-images.githubusercontent.com/47852354/147795209-a0e981ac-1659-4079-946b-d27003b527b4.png" width="400"> </p>

If the desired solution is reached, the algorithm will ignore the rest of the nodes returns the answer.The pseudo-code of this method (DLS) will be as the following.

<p> <img src="https://user-images.githubusercontent.com/47852354/147795210-73aef91f-ac6c-433e-96bd-72757de971b6.png" width="450"> </p> 

*DLS will equal Depth-First-Search (DFS) if we set depth to infinity.*

**Iterative Deepening Depth-First Search Algorithm (IDS Algorithm)**

**IDS** is a graph search strategy in which a depth-limited version of depth-first search is run repeatedly with increasing depth limits until the goal is found. IDS, or more specifically **IDDFS** is **optimal** like breadth-first search but uses much less memory; at each iteration, it visits the nodes in the search tree in the same order as depth-first search, but the cumulative order in which nodes are first visited is effectively breadth-first.

*In this project, I have implemented both algorithms to find the optimal solutions.*  

## Author and Date
Utkarsh Garg.












