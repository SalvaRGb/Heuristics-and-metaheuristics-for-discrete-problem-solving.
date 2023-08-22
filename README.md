# Heuristics and metaheuristics for discrete problem solving.
Navigating the TSP problem using heuristic algorithms and metaheuristic techniques

The Traveling Salesman Problem (TSP) is a well-known combinatorial optimization problem. The objective is to find the shortest route that visits a set of cities and returns to the starting point, visiting each city exactly once.

Formally, the problem is defined as follows:

Given a set of cities and the distances between each pair of cities, the goal is to find the shortest route (cycle) that visits all cities and returns to the starting city, minimizing the total distance traveled.

The TSP is an NP-hard problem, which means that there is no known efficient algorithm to solve it in polynomial time for all cases. However, there are various approaches and heuristic algorithms that can provide approximate solutions. Some common methods to address the TSP include:

1. **Exact Methods:** Although not efficient for large instances, there are dynamic programming and branch and bound algorithms that can solve small instances of the TSP.

2. **Heuristic Algorithms:** These are algorithms that attempt to find good but not necessarily optimal solutions. Examples include the nearest neighbor algorithm, the cheapest insertion algorithm, and the minimum spanning tree algorithm.

3. **Local Search Algorithms:** These algorithms iteratively improve an initial solution using local exchanges and movements to enhance the length of the tour.

4. **Metaheuristics:** More advanced methods like simulated annealing, tabu search, and genetic algorithms, which explore the solution space for high-quality solutions.

The Traveling Salesman Problem has applications in various real-life scenarios such as logistics, route planning, circuit design, DNA sequencing, and more. Due to its significance and complexity, the TSP has been extensively studied in combinatorial optimization and algorithm theory.

In this repository you will find a notebook with all the details on how to develop python functions using some heuristics and metaheuristics techniques to “solve” the TSP problem and an html with an interactive graph representing the complexity of this problem.

Here are the solutions found during the exploration of these methodologies (including the construction of the visualitazions in matplotlib and htm!): 

### Random Search:
Random search algorithms are heuristic methods that utilize randomness to explore the solution space in search of acceptable or even optimal solutions for a given problem. Unlike deterministic algorithms that follow a predefined strategy, random search algorithms introduce random elements into their search process to try to avoid getting stuck in local minima and explore different regions of the solution space. Random search algorithms do not guarantee finding the best solution in every run, as their performance can vary depending on random factors and the problem's structure. However, they can be effective in complex problems where exact methods are inefficient or impractical due to the large number of possible solutions.

  . ![](multimedia/Local_search_anim.gif)


### Nearest Neighbor:
The nearest neighbor algorithm is a heuristic method used to solve optimization problems, particularly the Traveling Salesman Problem (TSP). In this algorithm, a starting point is chosen, and then at each step, the nearest unvisited city is added to the tour. This process continues until all cities are visited. The algorithm may not always find the optimal solution but tends to provide relatively quick solutions.

  . ![](multimedia/Nearest_Neighbor_anim.gif)

### Local search:
Local search is a heuristic optimization approach that starts with an initial solution and iteratively explores neighboring solutions to find an improved solution within a local region of the solution space. It involves making small changes to the current solution and evaluating whether those changes lead to better outcomes. If a better solution is found, the process continues from that point, exploring further improvements in the nearby solution space. Local search algorithms aim to find solutions that are better than the starting point, but they might get stuck in local optima if the exploration is limited to a small region.

  . ![](multimedia/Local_search_anim.gif)

### Multistart Algorithm with local search:
The multistart technique is an optimization strategy that involves running a heuristic algorithm, such as a local search, multiple times with different initial solutions. Instead of relying on a single starting point, the algorithm is executed several times, each time beginning from a different initial solution. The goal is to explore a broader portion of the solution space and increase the likelihood of finding a better or even optimal solution.

  . ![](multimedia/Multistart_Algorithm_with_local_search_anim.gif)
  
### Greedy Algorithm:
The Greedy Algorithm is a heuristic approach used in optimization and decision-making problems. It involves making locally optimal choices at each step of the algorithm with the goal of achieving a global optimum. At each decision point, the algorithm selects the best available option based on the current information, without considering the potential long-term consequences.Basically the Greedy Algorithm focuses on immediate gains without considering how those choices might affect future decisions. While this strategy often leads to quick solutions, it doesn't guarantee the best overall result in all cases, especially for problems with complex dependencies or constraints.

  . ![](multimedia/Greedy_anim.gif)

### Grasp Algorithm:
GRASP (Greedy Randomized Adaptive Search Procedure) is a metaheuristic algorithm used to solve combinatorial optimization problems. It combines the greedy approach with randomization to enhance solution quality. In each iteration, GRASP constructs a list of potential candidates based on a greedy criterion and then randomly selects one of them. This balance between exploitation (greedy approach) and exploration (randomization) aids the algorithm in escaping local optima and discovering better solutions. The process is iteratively repeated to progressively refine the solution.

 . ![](multimedia/GRASP_anim.gif)
