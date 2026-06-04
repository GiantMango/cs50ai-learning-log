# [Week 2 - Uncertainty](https://cs50.harvard.edu/ai/weeks/2/)

## Progress
- Completed lecture [2026-06-01]
- Completed pagerank project [2026-06-02]
- Completed heredity project [2026-06-03]

## Key Concept
- **Probability**
    - **Bayes' Rule**: $P(b|a) = \frac{P(b)P(a|b)}{P(a)}$
    - **Joint Probability**
    - **Conditional Probability**
    - **Compound Joint Probability**
    - **Probability Rules**: A set of rules used to derive, simplify, and compute probability expressions, including the negation rule, inclusion-exclusion, marginalization, and conditioning.

- **Bayesian Network**: A data structure that represents dependencies among the network of connected random variables (nodes). It's a directed diagram with arrows pointing from parent nodes to child nodes. Each node has a probability distribution. If a node has parents then it's conditional no the parent nodes, if not then it's unconditional.
    - **Inference by Enumerate**: $P(X|e) = \alpha P(X, e) = \alpha \sum_y{P(X, e, y)}$. Where $X$ is the query, $e$ is the evidence, $\alpha$ is the normalization term for probabilities, and $y$ is the hidden variables we have no access to.
    - **Sampling ($N$)**: A way to approximate the probability distribution by using a random number generator to randomly pick states based on their likelihoods and run it thousands of times. Then, we use the final distribution as the approximate probability distribution. For conditional probability, rejection sampling discards samples that do not match the evidence and estimates the distribution using only the remaining samples.
    - **Likelihood Weighting**: A sampling method used when the evidence is rare and rejection sampling would discard too many samples. Instead of sampling the evidence variables and rejecting mismatched samples, we fix the evidence variables to their observed values and weight each sample by the likelihood of that evidence.

- **Markov Model**: A Markob Model represents probability distributions over states across time. Assume that the current state ONLY depends on a finite fixed number of previous states.
    - **Markov Chain**: $X_t$ would represent the state of the time $t$
    - **Transition Model**: How does state transition from one day to the next day (from $X_t$ to $X_{t+1}$)

- **Hidden Markov Model**: A Hidden Markov Model contains hidden states and observed evidence. The transition model describes how hidden states change over time, while the sensor model or emission model describes how observations ($E_t$) are generated from hidden states ($X_t$).
    - **Hidden State ($X$)**: What we wanna know but it's not obvious to the sensor/robot.
    - **Observations ($E$)**: Physical things that the sensor/robot can measure or observe.


## What I've learned...
This lecture is a bit friendly because it's mainly talking about probabilities, and with a little bit background in statistics, the materials are not that hard for me. However, The pagerank project made the fundamental part of search ranking much more vivid to me. I can't imagine how big of a computation it must be for a huge scale liek Google to rank all the webpages out there, when I am there struggling with figuring out maybe just 6 pages. And I'm also so excited to learn that the Hidden Markov Model is what we can use on robotic sensors, which might be super helpful for me in the future! Besides these, I think it's also fascinating to learn the simplified version of how the weather forecast predict the weather using Markov chain. I really appreciate and enjoy that Brian gives these really daily basic examples to illustrate these AI concepts. 

## Challenges
The most challenging part in this week's projects are the joint probability part in the heredity and the iterative algorithm in the pagerank project. Because in contrast, sampling is easy to understand and implement. The main mindset I needed to have for the iterative algorithm is that $PR(p) = P(random_jump) + \sum{P(other_page_to_this page)}$. When I put the problem this way, it's easier for me to break it down on my code. And for the heredity part, it's important that we need to consider if the person has parents or not. I think the problem become easier after I used variables to store the probability of the gene being passed by mother and by father. 

## Next Step
Start Lecture 3 Optimization.