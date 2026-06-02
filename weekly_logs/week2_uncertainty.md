# [Week 1 - Knowledge](https://cs50.harvard.edu/ai/weeks/2/)

## Progress
- Completed lecture [2026-06-01]

## Key Concept
- **Probability**
    - **Bayes' Rule**: $P(b|a) = \frac{P(b)P(a|b)}{P(a)}$
    - **Joint Probability**
    - **Conditional Probability**
    - **Compound Joint Probability**
    - **Probability Rules**: Rules: A set of rules used to derive, simplify, and compute probability expressions, including the negation rule, inclusion-exclusion, marginalization, and conditioning.

- **Bayesian Network**: A data structure that represent dependencies among the network of connected random variables (nodes). It's a directed diagram with arrows pointing from parent nodes to child nodes. Each node has a probability distribution, usually conditional on its parent node.
    - **Inference by Enumerate**: $P(X|e) = \alpha P(X, e) = \alpha \sum_y{P(X, e, y)}$. Where $X$ is the query, $e$ is the evidence, $\alpha$ is the normalization term for probabilities, and $y$ is the hidden variables we have no access to.
    - **Sampling ($N$)**: A way to approximate the probability distribution by using a random number generator to randomly pick states based on their likelihoods and run it thousands of times. Then, we use the final distribution as the approximate probability distribution. For conditional probability, rejection sampling discards samples that do not match the evidence and estimates the distribution using only the remaining samples.
    - **Likelihood Weighing**: A sampling method used when the evidence is rare and rejection sampling would discard too many samples. Instead of sampling the evidence variables and rejecting mismatched samples, we fix the evidence variables to their observed values and weight each sample by the likelihood of that evidence.

- **Markov Model**: A Markob Model represents probability distributions over states across time. Assume that the current state ONLY depends on a finite fixed number of previous states.
    - **Markov Chain**: $X_t$ would represent the state of the time $t$
    - **Transition Model**: How does state transition from one day to the next day (from $X_t$ to $X_{t+1}$)

- **Hidden Markov Model**: A Hidden Markov Model contains hidden states and observed evidence. The transition model describes how hidden states change over time, while the sensor model or emission model describes how observations ($E_t$) are generated from hidden states ($X_t$).
    - **Hidden State ($X$)**: What we wanna know but it's not obvious to the sensor/robot.
    - **Observations ($E$)**: Physical things that the sensor/robot can measure or observe.


## What I've learned...


## Challenges


## Next Step
Start Lecture 3 Optimization.