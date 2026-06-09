# [Week 3 - Optimization](https://cs50.harvard.edu/ai/weeks/3/)

## Progress
- Completed lecture [2026-06-04]
- Completed project [2026-06-08]

## Key Concept
- **Local Search**: Prone to converge to local maxima or minima. Suitable for applications that don't require the best outcome, but are okay with outcome being good enough.
    - **Hill Climbing**
    - **Simulated Annealing**
- **Linear Progression**: Problems with linear objective functions and constraints .
- **Constraint Satisfaction Problem (CSP)**: Problems defined by variables and their corresponding domains, and constraints. The goal is to assign all the variables with a value selected from their corresponding domains and comply with all constraints at the same time. 
    - **Unary vs. Binary Constraint**: Unary constraint refers to the constraint between a variable and its corresponding domain, while binary constraint refers to the constraint between two variables.
    - **arc**: an arc in the csp is the binary constraint, it's the line/arc connecting one variable to another in the constraint graph and it's directional.
    - **ac3**: an algorithm to enforce arc consistency by removing inconsistent values in the domains to reduce search space.
    - **backtracking**: a recursive depth-first search algorithm to assign values to variables.

## What I've learned...
I've taken optimization for machine learning when I'm getting my master's, and in that course, it's essential to know which cost function is it that we are trying to optimize. But to be honest, it's actually hard for me to connect the concepts that I've learnt from this lecture to optimizing. It's hard to separate the idea of "machine learning is to find a solution through learning" to "machine learning is to find the best solution through learning and optimization". Because in the end, people are just going to take the best solutions. However, there are times when we are okay to just take the good enough solutions, and I guess that is when we don't need optimization maybe? But also, there are optimizing everywhere, not necessarily of the solutions, but of the algorithm itself. In CSPs, the final answer is either valid or invalid. The optimization is often about improving the search process, such as reducing domains, choosing variables more intelligently, and avoiding unnecessary recursive branches. In the crossword project, techniques like node consistency, least-constraining value, degree heuristic are optimizing the process not the results.

## Challenges
Implementing the crossword project is pretty fun. First of all, we will have to really take a look at the data structure of the objects. What are stored in `Crossword` what are store in the `CrosswordCreator`, it's a good way to familiarize ourselves with the OOP again. Next would be plan which function to implement first. For me personally, I did backtracking and ac3 last, because I wanna make sure all the helper functions are functional correctly first before I put the blocks together. There's not much difficulties in the logic itself, the thing I spent most of my brain juice on is keeping track what data structure the variable is and what data structure do I need to use for the algorithm etc.

## Next Step
Start Lecture 4 Learning.
Additional reading from UC Berkeley CS188 textbook [section csp](https://inst.eecs.berkeley.edu/~cs188/textbook/csp/).