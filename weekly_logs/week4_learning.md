# [Week 4 - Learning](https://cs50.harvard.edu/ai/weeks/4/)

## Progress
- Completed lecture [2026-06-08]
- Completed project Shopping [2026-06-10]
- Completed project Nim [2026-06-15]

## Key Concept
- **Supervised Learning**: is a machine learning approach where a model learns from input-output pairs. After training, the model uses the learned relationship to predict outputs for new inputs.
    - **Classification**: it's a type of machine learning problem that aims to categorize the input data into different categories. For example: categorize the hand-written digit into 0 to 9.
    - **Regression**: this type of learning method aims to predict the output value based on the input data. For example, predict the housing price based on features like neighborhood, school district, size, facing direction, which floor it is, etc...
- **Reinforcement Learning**: an agent takes action and interact with the environment. It will receive rewards and updates its strategy to maximize the rewards its getting.
    - **Q-Learning**: the agent takes actions based on the current reward and estimated future rewards.
- **Unsupervised Learning**: a training method which is given known input data, then it will find some kind of hidden patterns or structures.
    - **Clusters**: a bunch of similar data points get to be grouped together without predefined labels.
- **Hypothesis Function**: it's the function h(x) that we human use to represent the real-life complex function f(x). We want the h(x) to try to perform like f(x) as much as possible so that we can use h(x) to predict the output based on the input.
- **Loss Function vs. Cost Function**: loss function is used to evaluate how the algorithm performs and cost function is the average or total loss over the entire process of training.
- **Explore vs. Exploit**: exploration refers to actions the favors the unknown, while exploitation refers actions that favors the known best.

## What I've learned...
I've taken optimization for machine learning, and in that course, the instructor introduced supervised learning and and I think specifically using optimization methods with these. So reinforcement learning and unsupervised learning was new concepts for me. I always wanted to learn about the concepts of clusters because I've been hearing this term in the machine learning projects somewhere else. And today I finally know what it is. I'm just sad the there's no cluster-related project in this lecture. However, I'll definitely play around skilearn package and clusters stuff.

## Challenges
There's actually not much of a challenge to the projects in this lectures. I think it's because this is an introduction to machine learning lecture and we didn't really dive into the mathematical part of the algorithms. We could just utilize the skilearn package to do machine learning project. The only mathematical part was Q-learning and the description in the project Nim was a little bit complicated for me to understand. And I think it was just hard for me to visualize how the agent learn through reinforcement learning with the rewards and q value thing. This part was new for me.

## Next Step
- Start Lecture 5 Neural Network.
- Additional reading from UC Berkeley CS188 textbook [section ml](https://inst.eecs.berkeley.edu/~cs188/textbook/ml/) and [section rl](https://inst.eecs.berkeley.edu/~cs188/textbook/rl/rl.html) for reinforcement learning.