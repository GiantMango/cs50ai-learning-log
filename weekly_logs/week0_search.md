# Week 0 - Search

## Progress

- Completed Lecture 0 over two sessions.
- Completed Project 0 over two sessions.
- Submitted Project 0 successfully with optional Alpha-Beta Pruning implemented.

## Key Concept
- **Depth-First Search vs Breadth-First Search**: DFS will exhausts the entire depth of a branch and then go on to the next one, while BFS will explore all the shallowest layer of actions then go on to one level deeper. DFS uses `Stack` (Last-in-first-out) data structure. BFS uses `Queue` (First-in-first-out) data structure.
- **Greedy Best-First Search and A\* Search**: Adding heuristic function $h(n)$ to help agent making decisions. In maze problem, it could be the Manhattan distance between the current cell to the goal cell. In A\* search, $h(n)$ represents estimated cost to goal and $g(n)$ is the cost to reach the current node. It makes decisions based on minimising $g(n) + h(n)$
- **Minimax and Alpha-Beta Pruning**: It's used in *adversarial search*, in which I make a move and the opponent makes a move trying to make me fail. One player is the max player, trying to maximise the outcome, while the other player is the min player, trying to minimise the outcome. Alpha-Beta Pruning is the "I've seen enough" strategy. It carries the history record of the best score and skipped the branches that will not be selected by the opponent.

## Terminology
- **Search Problem**: Maze, corresponds to route finding in map
- **Agent**: An agent is a thing that observes the environment and makes decision based on the observations.
- **State**: A configuration.
- **State Space**: A set of all the states we can get from the initial state.
- **Actions**: Choices that agent can make in this current state. Represented by `actions(s)`, returns a set of actions.
- **Transition Model**: The process of transitioning from $s_1$ to $s_2$ through action. Represented by `result(s, a)`.
- **Goal Test**: To determine if the current state is the goal state. In adversarial search it will be represented by `terminal(s)`, returns boolean. In other cases, will be represented as `is_goal(s)`.
- **Path Cost**: A numerical value that represents how expensive it is to get to goal state.
- **Optimal Solution**: The solution with the lowest path cost.
- **Frontier**: A data structure that contains all the states we have discovered but have not yet explored.


## What I Learned...
Google Maps route generating is a search problem and the simplified problem is maze solving. I've learn how to realize the concepts of actions, goal test, transition model, etc... in Python.

## Challenges
Finishing Project 0 was easy, but implementing Alpha-Beta Pruning was hard. On top of that, `min_value()` and `max_value()` is mutual recursion, so it takes a while for me to actually understand the mechanism. 

## Next Step
- Start week 1 lecture, knowledge.